---
title: "KB-PRO-01 — Gestión de cambios"
id: KB-PRO-01
owner: PM
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - procesos
  - cambios
---

# KB-PRO-01 — Gestión de cambios

**Objetivo:** que todo cambio de alcance, plazo o costo quede registrado, aprobado y trazable.

## Cuándo se abre un RFC

- Cambia el alcance, el plazo o el costo acordado.
- Se modifica un requisito aprobado.
- Se incorpora una tecnología o dependencia nueva que afecta la arquitectura.

Los cambios menores de redacción no requieren RFC: se corrigen en el PR.

## Flujo

| Paso | Responsable     | Resultado                                     |
| :--- | :-------------- | :-------------------------------------------- |
| 1    | Solicitante     | RFC con motivo, impacto y alternativas        |
| 2    | PM              | Análisis de impacto en alcance, plazo y costo |
| 3    | Revisor técnico | Evaluación de factibilidad                    |
| 4    | CCB             | Aprobado, rechazado o diferido                |
| 5    | Autor           | Actualiza documentos y registra el cambio     |

## Reglas

- Un RFC aprobado no se modifica: si cambia la decisión, se abre otro.
- El registro de cambios es la referencia única de estado.
- Todo RFC aprobado actualiza la línea base y los documentos afectados.

## Documentos relacionados

- [[KB-PRO-02-revision-de-codigo|KB-PRO-02 — Revisión de código]]
- [[../04-plantillas/index|04 — Plantillas]]
