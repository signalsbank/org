---
title: "KB-REU-01 — Componente de autenticación"
id: KB-REU-01
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - reutilizables
  - autenticacion
  - seguridad
---

# KB-REU-01 — Componente de autenticación

**Qué resuelve:** login con usuario y contraseña, sesión con token y control de acceso por rol.

## Requisitos

- Contraseñas con hash y sal; nunca en texto plano.
- Token con expiración corta y renovación controlada.
- Roles definidos por configuración, no por código disperso.
- Registro de intentos fallidos y bloqueo temporal.

## Cómo se reutiliza

1. Copiar el módulo desde el repositorio de referencia o instalarlo como dependencia interna.
2. Configurar las variables de entorno (clave de firma, expiración, origen permitido).
3. Definir los roles del proyecto en la configuración.
4. Documentar en el `README` del proyecto qué roles existen y quién los asigna.

## Limitaciones

- No incluye registro público de usuarios ni recuperación autónoma de credenciales.
- No reemplaza la revisión de permisos por endpoint: cada proyecto la define.

## Lecciones asociadas

- `LESSON-003`: centralizar la validación de roles evita controles duplicados y inconsistentes.

## Documentos relacionados

- [[../05-seguridad/KB-SEC-01-gestion-de-secretos|KB-SEC-01 — Gestión de secretos]]
- [[../04-plantillas/TPL-ADR|TPL-ADR]]
