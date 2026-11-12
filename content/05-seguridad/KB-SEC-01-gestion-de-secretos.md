---
title: "KB-SEC-01 — Gestión de secretos"
id: KB-SEC-01
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - seguridad
  - secretos
---

# KB-SEC-01 — Gestión de secretos

**Objetivo:** que ninguna credencial quede en el código, en la wiki ni en los registros.

## Reglas

1. Los secretos viven en variables de entorno o en el gestor de secretos del entorno. Nunca en el
   repositorio.
2. `.env` se ignora en Git; se versiona `.env.example` con valores vacíos o de ejemplo.
3. Cada entorno tiene sus propias credenciales: no se reutilizan las de producción.
4. Un secreto expuesto se considera comprometido: se rota de inmediato y se registra el incidente.
5. Los registros y mensajes de error no muestran tokens, claves ni datos personales.

## Rotación

| Tipo                           | Frecuencia sugerida | Responsable        |
| :----------------------------- | :------------------ | :----------------- |
| Clave de firma de token        | Cada 6 meses        | Líder técnico      |
| Credencial de base de datos    | Cada 6 meses        | Líder técnico      |
| Credencial de servicio externo | Según el proveedor  | Dueño del servicio |

## Si se filtra una credencial

1. Rotar la credencial.
2. Revisar los accesos de las últimas 24 horas.
3. Registrar el incidente con identificador `ERR-<n>`.
4. Si hubo exposición de datos, aplicar [[KB-SEC-02-privacidad-y-datos|KB-SEC-02]].

## Documentos relacionados

- [[../03-reutilizables/KB-REU-01-componente-autenticacion|KB-REU-01 — Autenticación]]
- [[../02-procesos/KB-PRO-02-revision-de-codigo|KB-PRO-02 — Revisión de código]]
