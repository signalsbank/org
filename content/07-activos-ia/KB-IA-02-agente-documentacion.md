---
title: "KB-IA-02 — Agente de documentación"
id: KB-IA-02
owner: APM
version: 1.0
date: 2026-11-12
status: vigente
tags:
  - ia
  - agente
  - documentacion
---

# KB-IA-02 — Agente de documentación

**Qué hace:** responde preguntas sobre la wiki citando los documentos fuente y detecta enlaces
rotos o documentos sin dueño.

## Configuración

| Campo    | Valor                                                        |
| :------- | :----------------------------------------------------------- |
| Fuente   | Contenido de esta wiki y repositorios con permiso de lectura |
| Ámbito   | Interno                                                      |
| Permisos | Lectura; sin escritura ni merge                              |
| Dueño    | APM                                                          |
| Revisión | Mensual, junto con la revisión de la wiki                    |

## Comportamiento esperado

- Cita siempre el documento y el identificador (`KB-...`, `ADR-...`).
- Si no encuentra la respuesta, lo dice y sugiere abrir un issue de documentación.
- No responde con información fuera de las fuentes autorizadas.
- No muestra contenido de nivel confidencial a quien no tiene permiso.

## Límites

- No modifica documentos.
- No aprueba cambios.
- No reemplaza la revisión humana.

## Documentos relacionados

- [[KB-IA-01-prompt-revision-de-pr|KB-IA-01 — Prompt de revisión de PR]]
- [[../00-gobierno/KB-GOB-02-ciclo-de-revision|KB-GOB-02 — Ciclo de revisión]]
