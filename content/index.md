---
title: Wiki organizacional
aliases:
  - "Inicio"
  - "Índice central"
---

# Wiki organizacional

Base de conocimiento transversal de la organización: estándares, procesos, activos
reutilizables, plantillas, seguridad, onboarding y activos de IA.

> **Alcance.** La wiki central no reemplaza la documentación de cada proyecto: la conecta. Lo
> específico de un proyecto vive en su repositorio, dentro de `docs/`.

## Áreas

| Área                                           | Prefijo  | Contenido                                  |
| :--------------------------------------------- | :------- | :----------------------------------------- |
| [[00-gobierno/index\|00 — Gobierno]]           | `KB-GOB` | Dueños, ciclo de revisión, índices         |
| [[01-estandares/index\|01 — Estándares]]       | `KB-EST` | Estilo, arquitectura, seguridad            |
| [[02-procesos/index\|02 — Procesos]]           | `KB-PRO` | SCM, cambios, calidad, adquisiciones       |
| [[03-reutilizables/index\|03 — Reutilizables]] | `KB-REU` | Componentes, scripts, plantillas de código |
| [[04-plantillas/index\|04 — Plantillas]]       | `TPL`    | ADR, RFC, post-mortem, README, SETUP       |
| [[05-seguridad/index\|05 — Seguridad]]         | `KB-SEC` | Secretos, accesos, privacidad              |
| [[06-onboarding/index\|06 — Onboarding]]       | `KB-ONB` | Guía de ingreso, glosario, FAQ             |
| [[07-activos-ia/index\|07 — Activos de IA]]    | `KB-IA`  | Prompts, agentes, skills                   |

## Cómo se busca la información

1. Buscar por identificador (`ADR-001`, `ERR-042`) o por etiqueta (`#seguridad`, `#postgresql`).
2. Usar el índice del proyecto y el índice central de la wiki.
3. Consultar el [[06-onboarding/KB-ONB-02-glosario|glosario]] si el término es nuevo.
4. Si no se encuentra, registrar la pregunta en el FAQ o abrir un issue de documentación.

## Reglas

- **Clasificación:** si sirve para más de un proyecto, va a la wiki central; si es específico, va
  al repositorio del proyecto.
- **Privacidad:** no se almacenan datos personales reales ni credenciales. Los datos de ejemplo son
  sintéticos o anonimizados.
- **Vigencia:** cada documento tiene dueño, versión y estado. Ver
  [[00-gobierno/KB-GOB-02-ciclo-de-revision|KB-GOB-02 — Ciclo de revisión]].

## Identificadores

| Tipo              | Formato         | Ejemplo      |
| :---------------- | :-------------- | :----------- |
| Documento de wiki | `KB-<área>-<n>` | `KB-SEC-03`  |
| Decisión          | `ADR-<n>`       | `ADR-001`    |
| Error             | `ERR-<n>`       | `ERR-042`    |
| Lección           | `LESSON-<n>`    | `LESSON-007` |
| Runbook           | `RUN-<n>`       | `RUN-002`    |
| Plantilla         | `TPL-<n>`       | `TPL-ADR`    |
