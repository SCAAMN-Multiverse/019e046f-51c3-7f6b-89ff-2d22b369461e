# Triada de ejecución — executor + planner + checker

Tres roles separados con responsabilidades diferenciadas: el **planner** descompone el objetivo en pasos; el **executor** los ejecuta; el **checker** verifica el resultado contra el plan. Reportan en JSON. **Dos políticas de desviación**: si el destino sigue siendo el mismo → continuar; si el destino ha cambiado → cortar y pedir feedback humano. Es PRINCE2 gestión por excepción aplicado a IA.

## Por qué importa

Convierte al agente del "arquero con flecha al viento" en un "misil inteligente" — no porque el agente decida más, sino porque la arquitectura de roles externos cierra el bucle de control sin requerir supervisión continua del humano.

## Ciencia subyacente

- [PRINCE2 — gestión por excepción](./ciencia-prince2-gestion-por-excepcion.md)
- [Runtime verification — Havelund & Roşu](./ciencia-runtime-verification-havelund-rosu.md)

## Anécdotas que lo sostienen

- [Akdong — migración 10 días enero](../historias/akdong-migracion-10-dias.md)
