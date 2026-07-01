# Avatar autoconsciente que opera sobre sí mismo

Un avatar conoce su propia estructura (su `avatar-mind`) y puede modificarla dentro de su propio ciclo de vida. No es un programa que ejecuta tareas; es un sistema que se actualiza a sí mismo a medida que aprende.

## Por qué importa

Es la única respuesta arquitectónica posible al hecho de que la velocidad del sector caduca cualquier sistema estable en ~6 meses. Un manual envejece; un avatar autoconsciente se reescribe.

## Ciencia subyacente

- [Autopoiesis — Maturana & Varela](./ciencia-autopoiesis-maturana-varela.md)
- [Estructura dinamicodependiente](./ciencia-estructura-dinamicodependiente.md)

## Anécdotas que lo sostienen

- [Cambio de nombre agente → avatar](../historias/cambio-nombre-agente-a-avatar.md)
- [Obsidian + Wikilinks — descubrimiento marzo](../historias/obsidian-wikilinks-marzo.md)

```avatar-lang
@id: avatar-autoconsciente
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
