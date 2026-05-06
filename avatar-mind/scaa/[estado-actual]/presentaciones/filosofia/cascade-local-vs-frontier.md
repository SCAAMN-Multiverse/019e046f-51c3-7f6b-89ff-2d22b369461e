# Cascade local-vs-frontier — modelo local barato por defecto

Routing de modelo: por defecto, las sub-tareas baratas (resumir, clasificar, extraer entidades) se delegan a un modelo local (Ollama vía MCP `local-llm`); solo se escala a un modelo frontier cuando la sub-tarea lo exige (juicio, diseño, edición de código). El cascade es regla, no excepción.

## Por qué importa

Reduce coste y latencia sin comprometer calidad donde importa. Y, más profundamente, obliga al aparato a clasificar sus propias sub-tareas — qué es ejecución mecánica y qué es razonamiento — lo cual disciplina la arquitectura misma.

## Anécdotas que lo sostienen

- [Akdong — migración 10 días enero](../historias/akdong-migracion-10-dias.md)
