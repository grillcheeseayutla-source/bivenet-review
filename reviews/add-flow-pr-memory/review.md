# Paquete de revisión Bivenet

## ID de tarea

add-flow-pr-memory

## Rama base

origin/main

## Rama revisada

origin/tarea/add-flow-pr-memory

## Archivos modificados

- CLAUDE.md
- docs/ARQUITECTURA_MASTER.md
- docs/CHECKLIST_AUDITORIA.md
- docs/FLUJO_SUPERVISOR_OBRERO.md
- docs/POLITICA_DEPLOY.md
- package.json
- scripts/flow.js
- scripts/flow.mjs

## Diff stat

```
CLAUDE.md                       |  39 ++++
 docs/ARQUITECTURA_MASTER.md     |  19 ++
 docs/CHECKLIST_AUDITORIA.md     |  13 ++
 docs/FLUJO_SUPERVISOR_OBRERO.md |  16 ++
 docs/POLITICA_DEPLOY.md         |  27 +++
 package.json                    |  10 +-
 scripts/flow.js                 | 214 -------------------
 scripts/flow.mjs                | 463 ++++++++++++++++++++++++++++++++++++++++
 8 files changed, 583 insertions(+), 218 deletions(-)
```

## Impacto detectado

- Next.js: SÍ
- provision-agent-v2: NO
- wsp-agent-v2: NO

## Resultado esperado si se aprueba release

- Merge a main.
- Push a origin/main.
- Next.js se despliega manualmente en Vercel si aplica.
- Solo se reinician backends afectados.
- No usar PM2.

## Reglas de revisión

Este paquete público es solo para revisión del Arquitecto.

No autoriza release por sí solo.

El Arquitecto debe revisar `review.md`, `files.txt` y `diff.patch`.

## Veredicto requerido

Responder exactamente una de estas opciones:

APROBADO PARA RELEASE

o

NO APROBADO, con correcciones necesarias.
