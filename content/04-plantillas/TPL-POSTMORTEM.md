---
title: "TPL-POSTMORTEM — Plantilla de post-mortem"
id: TPL-POSTMORTEM
owner: PM
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - plantillas
  - postmortem
  - lecciones
---

# TPL-POSTMORTEM — Plantilla de post-mortem

> Se usa después de un incidente grave. El objetivo es aprender, no buscar culpables.

## Resumen

| Campo       | Valor                                     |
| :---------- | :---------------------------------------- |
| Incidente   | `ERR-000`                                 |
| Fecha       | `dd/mm/aaaa`                              |
| Duración    | Tiempo desde la detección hasta el cierre |
| Impacto     | Usuarios o procesos afectados             |
| Responsable | Rol que coordina el análisis              |

## Línea de tiempo

| Hora  | Qué pasó    |
| :---- | :---------- |
| 00:00 | Detección   |
| 00:00 | Diagnóstico |
| 00:00 | Mitigación  |
| 00:00 | Cierre      |

## Causa raíz

Qué falló y por qué. Se puede usar la técnica de los cinco porqués.

## Qué funcionó y qué no

- Funcionó: …
- No funcionó: …

## Acciones

| Acción | Dueño | Fecha límite | Estado  |
| :----- | :---- | :----------- | :------ |
| …      | …     | `dd/mm/aaaa` | Abierta |

## Lecciones

Se registran como `LESSON-<n>` y se enlazan desde el índice del proyecto.

## Documentos relacionados

- [[../02-procesos/KB-PRO-01-gestion-de-cambios|KB-PRO-01 — Gestión de cambios]]
- [[../00-gobierno/KB-GOB-02-ciclo-de-revision|KB-GOB-02 — Ciclo de revisión]]
