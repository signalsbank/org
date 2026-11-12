---
title: "KB-EST-02 — Estándar de arquitectura"
id: KB-EST-02
owner: Líder técnico
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - estandares
  - arquitectura
---

# KB-EST-02 — Estándar de arquitectura

**Objetivo:** que las decisiones técnicas se tomen con los mismos criterios en todos los proyectos.

## Principios

1. **API primero.** El contrato se documenta con OpenAPI antes de implementar.
2. **Separación por capas.** Interfaz, lógica de negocio y persistencia no se mezclan.
3. **Configuración por entorno.** Nada de valores fijos: variables de entorno y secretos fuera del
   repositorio.
4. **Trazabilidad.** Toda decisión relevante se registra en un [[../04-plantillas/TPL-ADR|ADR]].
5. **Simplicidad.** Se elige la solución más simple que cumpla los requisitos; la complejidad se
   justifica.

## Documentación mínima de un proyecto

```text
docs/
├── 00-indice.md
├── 01-requisitos/
├── 02-arquitectura/
│   ├── c4/
│   ├── base-de-datos/
│   └── adr/
├── 03-despliegue/
├── 04-calidad/
└── 05-operacion/
```

## Revisión

Un cambio de arquitectura requiere ADR y revisión del líder técnico antes de mergear.

## Documentos relacionados

- [[KB-EST-01-guia-de-estilo|KB-EST-01 — Guía de estilo]]
- [[../02-procesos/KB-PRO-02-revision-de-codigo|KB-PRO-02 — Revisión de código]]
