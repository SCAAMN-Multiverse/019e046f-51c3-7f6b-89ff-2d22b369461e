# Sistema-operado como fuente de verdad última

El sistema-operado (el repo, el producto, la presentación, lo que sea que el avatar opera) es la fuente de verdad. El `avatar-mind` es **espejo derivado**: puede ir desfasado y debe reconciliarse, no fabricarse.

## Por qué importa

Disciplina la disciplina cognitiva del avatar: ante cualquier pregunta sobre estado real, mirar primero la fuente; ante cualquier ciclo de trabajo nuevo, contrastar avatar-mind con sistema-operado y reconciliar antes de planificar.

## Ciencia subyacente

- [Estructura dinamicodependiente](./ciencia-estructura-dinamicodependiente.md)

## Anécdotas que lo sostienen

- [W2M — SharePoint tres iniciativas](../historias/w2m-sharepoint-tres-iniciativas.md)

```avatar-lang
@id: sistema-operado-fuente-de-verdad
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
