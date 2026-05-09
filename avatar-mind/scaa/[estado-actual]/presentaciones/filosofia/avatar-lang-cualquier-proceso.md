# avatar-lang sirve para cualquier proceso con principio y fin

avatar-lang no es el lenguaje de las cinco fases del ciclo. Es la gramática de **cualquier proceso del avatar con estados, acciones, transiciones y dependencias entre módulos**. Las cinco fases son una instancia, no la definición.

## Por qué importa

Permite expresar en la misma gramática: el ciclo de vida, las 13 comprobaciones de coherencia de RELEASE, el proceso `create-avatar`, las reglas de naming/versionado/docs-io. Resultado: composabilidad, versionado independiente y trazabilidad uniforme. La generalidad es criterio de calidad del DSL.

## Ciencia subyacente

- [Process mining — van der Aalst](./ciencia-process-mining-van-der-aalst.md)

## Anécdotas que lo sostienen

- [Weft — DSL paralelo el 15 de abril](../historias/weft-15-abril-paralelo.md)
- [Obsidian + Wikilinks — descubrimiento marzo](../historias/obsidian-wikilinks-marzo.md)

```avatar-lang
@id: avatar-lang-cualquier-proceso
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
