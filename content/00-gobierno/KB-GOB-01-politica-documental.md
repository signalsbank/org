---
title: "KB-GOB-01 — Política documental"
id: KB-GOB-01
owner: PMO
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - gobierno
  - documentacion
---

# KB-GOB-01 — Política documental

**Objetivo:** que toda la documentación tenga dueño, versión y estado, y que se actualice mientras
se trabaja.

## Reglas

1. **Docs-as-code.** La documentación vive en Markdown dentro del repositorio y se versiona con
   Git. Una historia o PR no está terminada si el cambio de código no actualiza su documentación.
2. **Un dueño por documento.** El dueño figura en el frontmatter y responde por su vigencia.
3. **Actualización en el mismo PR.** El cambio de documentación viaja junto con el cambio que lo
   motiva.
4. **Sin duplicación.** Si el contenido sirve a varios proyectos, se escribe una vez en la wiki y se
   enlaza desde cada proyecto.
5. **Sin datos sensibles.** No se publican credenciales ni datos personales reales.

## Estados

| Estado   | Significado                                               |
| :------- | :-------------------------------------------------------- |
| Borrador | En redacción; no debe usarse como referencia.             |
| Vigente  | Aprobado y publicado; es la referencia actual.            |
| Obsoleto | Reemplazado por otro documento; se conserva por historia. |

## Versionado

`v0.x` para borrador, `v1.0` para aprobado y `v1.x` para correcciones menores. Las versiones
anteriores se conservan en Git para auditoría.

## Documentos relacionados

- [[KB-GOB-02-ciclo-de-revision|KB-GOB-02 — Ciclo de revisión]]
- [[../04-plantillas/TPL-README|TPL-README]]
