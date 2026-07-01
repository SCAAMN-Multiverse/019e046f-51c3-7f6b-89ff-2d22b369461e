# Versionado tri-temporal — scaa rápido, narrative medio, meta-narrative lento

El avatar versiona tres planos a velocidades distintas: **scaa** (estado actual del sistema-operado, cambia rápido), **narrative** (cómo se trabaja, cambia a velocidad media), **meta-narrative** (historia del proyecto, cambia despacio). Tres tiempos del avatar, no uno.

## Por qué importa

Resuelve la paradoja del contexto: el avatar recuerda con el humano sin enterrar al humano en historia repetida. Lo que cambia rápido se ve sin ruido; lo que cambia lento queda accesible para reconstruir contexto histórico cuando hace falta.

## Ciencia subyacente

- [Estructura dinamicodependiente](./ciencia-estructura-dinamicodependiente.md)

## Anécdotas que lo sostienen

- [Obsidian + Wikilinks — descubrimiento marzo](../historias/obsidian-wikilinks-marzo.md)

```avatar-lang
@id: versionado-tri-temporal
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
