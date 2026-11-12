---
title: "KB-PRO-02 — Revisión de código"
id: KB-PRO-02
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - procesos
  - calidad
  - pull-request
---

# KB-PRO-02 — Revisión de código

**Objetivo:** mejorar la calidad sin frenar la entrega.

## Antes de pedir revisión

- [ ] La rama está actualizada con la principal.
- [ ] Los tests pasan en local.
- [ ] El PR tiene descripción: qué cambia y por qué.
- [ ] La documentación afectada está actualizada en el mismo PR.
- [ ] No hay credenciales ni datos personales en el diff.

## Durante la revisión

| Aspecto       | Qué se mira                                             |
| :------------ | :------------------------------------------------------ |
| Correctitud   | El cambio hace lo que dice y cubre los casos borde.     |
| Legibilidad   | Nombres claros, funciones cortas, sin duplicación.      |
| Pruebas       | Hay tests para la lógica nueva o modificada.            |
| Seguridad     | Entradas validadas, permisos verificados, sin secretos. |
| Documentación | README, ADR o API actualizados si corresponde.          |

## Reglas

- Un PR no se mergea sin al menos una aprobación.
- Los comentarios se responden antes de mergear; no se resuelven sin discusión.
- Un PR grande se divide: menos de 400 líneas es una buena referencia.

## Documentos relacionados

- [[KB-PRO-01-gestion-de-cambios|KB-PRO-01 — Gestión de cambios]]
- [[../07-activos-ia/KB-IA-01-prompt-revision-de-pr|KB-IA-01 — Prompt de revisión de PR]]
