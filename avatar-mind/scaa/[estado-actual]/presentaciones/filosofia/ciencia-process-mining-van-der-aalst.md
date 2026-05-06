# Ciencia — Process mining (van der Aalst)

**Wil van der Aalst** desarrolló *process mining*: extraer modelos de proceso reales a partir de logs de ejecución, y comparar lo ejecutado contra el modelo BPMN ideal post-hoc. Conformance checking BPM extiende esta lógica a verificación si las instancias respetan el modelo.

## Lección que el aparato extrae

Evolution-Art (paradigma del aparato) extiende esto a **verificación runtime con consenso humano-avatar**: no se compara solo post-hoc contra un modelo fijo; el modelo se renegocia durante la ejecución cuando el avatar y el humano detectan desviaciones legítimas. avatar-lang es la gramática que hace ejecutables esos modelos BPMN.

## Filosofías que sostiene

- [avatar-lang sirve para cualquier proceso](./avatar-lang-cualquier-proceso.md)
- [Estados externos públicos, no internos](./estados-publicos-no-internos.md)
- [Triada de ejecución](./triada-de-ejecucion.md)
