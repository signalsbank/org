---
title: "KB-GOB-02 — Ciclo de revisión"
id: KB-GOB-02
owner: APM
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - gobierno
  - revision
---

# KB-GOB-02 — Ciclo de revisión

**Objetivo:** detectar documentación desactualizada, duplicada o sin dueño antes de que se
convierta en un problema.

## Momentos de actualización

| Momento                 | Qué se actualiza                                                             |
| :---------------------- | :--------------------------------------------------------------------------- |
| Inicio de un proyecto   | Se copia la plantilla y se crean `README`, `SETUP`, `AGENTS.md` y el índice. |
| Cada PR                 | Documento afectado, API, decisión o runbook.                                 |
| Cada decisión relevante | ADR con contexto, alternativas, decisión y consecuencias.                    |
| Cada incidente          | Entrada en el registro de errores y, si es grave, post-mortem.               |
| Cada hito               | Lecciones aprendidas y actualización del índice.                             |
| Cierre del proyecto     | Se archiva, se extraen activos reutilizables y se enlazan acá.               |

## Revisión mensual

Checklist de quince minutos:

- [ ] Enlaces rotos.
- [ ] Documentos sin dueño o sin versión.
- [ ] Documentos marcados como vigentes con más de seis meses sin cambios.
- [ ] Contenido duplicado entre wiki y repositorios.
- [ ] Permisos y clasificación de sensibilidad.

El resultado se registra como comentario en el issue de revisión del mes.

## Documentos relacionados

- [[KB-GOB-01-politica-documental|KB-GOB-01 — Política documental]]
- [[../05-seguridad/KB-SEC-02-privacidad-y-datos|KB-SEC-02 — Privacidad y datos]]
