---
title: "KB-EST-01 — Guía de estilo"
id: KB-EST-01
owner: APM
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - estandares
  - documentacion
---

# KB-EST-01 — Guía de estilo

**Objetivo:** que cualquier integrante escriba un documento que el resto pueda leer y encontrar sin
preguntar.

## Escritura

- Español neutro, tono formal, sin marketing ni emojis decorativos.
- Frases cortas. Una idea por párrafo.
- Siglas definidas la primera vez que aparecen; el resto, al [[../06-onboarding/KB-ONB-02-glosario|glosario]].
- Sin datos personales reales ni credenciales.

## Formato

| Elemento     | Convención                                    |
| :----------- | :-------------------------------------------- |
| Fechas       | `dd/mm/aaaa`                                  |
| Moneda       | `USD` para caja, `ARS` para esfuerzo interno  |
| Títulos      | Un solo `#` por documento; secciones con `##` |
| Tablas       | Para fichas, matrices y comparaciones         |
| Enlaces      | Por identificador, no solo por título         |
| Diagramas    | Bloques `mermaid`                             |
| Advertencias | Cita en bloque (`>`)                          |

## Frontmatter mínimo

```yaml
---
title: "KB-XXX-00 — Título"
id: KB-XXX-00
owner: Rol o persona
version: 1.0
date: 2026-01-01
status: vigente
tags:
  - area
---
```

## Documentos relacionados

- [[KB-EST-02-estandar-de-arquitectura|KB-EST-02 — Estándar de arquitectura]]
- [[../04-plantillas/index|04 — Plantillas]]
