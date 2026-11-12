---
title: "KB-IA-01 — Prompt de revisión de PR"
id: KB-IA-01
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - ia
  - prompt
  - calidad
---

# KB-IA-01 — Prompt de revisión de PR

**Ámbito:** asistencia en la revisión de pull requests. No reemplaza la aprobación humana.

## Prompt

```text
Actuá como revisor de código de este repositorio.
Recibís el diff del PR y el enlace a la documentación afectada.

Revisá, en este orden:
1. Correctitud: ¿el cambio hace lo que describe? ¿cubre casos borde?
2. Pruebas: ¿hay tests para la lógica nueva o modificada?
3. Seguridad: entradas validadas, permisos verificados, sin secretos ni datos personales.
4. Legibilidad: nombres, duplicación, funciones largas.
5. Documentación: ¿se actualizó el documento afectado en el mismo PR?

Devolvé:
- Hallazgos ordenados por severidad (bloqueante, importante, sugerencia).
- Para cada hallazgo: archivo, línea, problema y corrección propuesta.
- Qué NO pudiste verificar por falta de contexto.

No inventes hallazgos. Si el diff no alcanza, decilo.
```

## Uso responsable

- El resultado se contrasta con el código; no se aplica a ciegas.
- No se pegan credenciales, datos personales ni fragmentos confidenciales en la herramienta.
- La aprobación final es humana y queda registrada en el PR.

## Documentos relacionados

- [[../02-procesos/KB-PRO-02-revision-de-codigo|KB-PRO-02 — Revisión de código]]
- [[../05-seguridad/KB-SEC-01-gestion-de-secretos|KB-SEC-01 — Gestión de secretos]]
