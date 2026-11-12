---
title: "TPL-ADR — Plantilla de decisión de arquitectura"
id: TPL-ADR
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - plantillas
  - adr
---

# TPL-ADR — Plantilla de decisión de arquitectura

> Copiar este bloque al repositorio del proyecto, en `docs/02-arquitectura/adr/`, y numerar de forma
> correlativa (`ADR-001`, `ADR-002`, …).

## Encabezado

| Campo  | Valor                              |
| :----- | :--------------------------------- |
| ID     | `ADR-000`                          |
| Título | Decisión en una frase              |
| Fecha  | `dd/mm/aaaa`                       |
| Estado | Propuesto / Aceptado / Reemplazado |
| Dueño  | Rol o persona                      |

## Contexto

Qué situación obliga a decidir. Restricciones técnicas, de plazo o de costo.

## Alternativas evaluadas

| Alternativa | Ventajas | Desventajas |
| :---------- | :------- | :---------- |
| A           | …        | …           |
| B           | …        | …           |

## Decisión

Qué se elige y por qué. Una o dos frases.

## Consecuencias

- Qué se gana.
- Qué se pierde o queda pendiente.
- Qué documentos o componentes hay que actualizar.

## Ejemplo breve

`ADR-001 — Base de datos relacional para el módulo de usuarios`: se elige PostgreSQL por integridad
transaccional y soporte de tipos JSON. Consecuencia: el equipo debe mantener migraciones versionadas.

## Documentos relacionados

- [[../01-estandares/KB-EST-02-estandar-de-arquitectura|KB-EST-02 — Estándar de arquitectura]]
