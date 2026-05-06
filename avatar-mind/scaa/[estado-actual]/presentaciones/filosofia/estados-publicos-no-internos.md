# Estados externos públicos, no estados mentales internos

El estado interno de un agente IA es opaco — no se puede inspeccionar fiablemente. La respuesta arquitectónica del aparato es **externalizar el estado**: hacerlo público en un grafo BPMN/avatar-lang que cualquier checker puede leer y verificar.

## Por qué importa

Es la lección directa de los años 2000 con FIPA-BDI: querían verificar creencias y deseos internos del agente y no se pudo. El aparato evita ese pozo redefiniendo el problema — no se verifica el estado mental, se verifica el estado externo declarado por el avatar.

## Ciencia subyacente

- [FIPA-BDI y el estado opaco](./ciencia-fipa-bdi-y-estado-opaco.md)
- [Process mining — van der Aalst](./ciencia-process-mining-van-der-aalst.md)
- [Runtime verification — Havelund & Roşu](./ciencia-runtime-verification-havelund-rosu.md)

## Anécdotas que lo sostienen

- [Cambio de nombre agente → avatar](../historias/cambio-nombre-agente-a-avatar.md)
- [Weft — DSL paralelo el 15 de abril](../historias/weft-15-abril-paralelo.md)
