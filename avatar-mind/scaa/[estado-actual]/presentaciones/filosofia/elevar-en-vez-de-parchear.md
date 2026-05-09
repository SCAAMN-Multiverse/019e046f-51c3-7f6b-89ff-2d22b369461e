# Elevar en vez de parchear

Ante un problema recurrente, no parchear local: subir el nivel de abstracción donde el problema se disuelve. Si la misma fricción aparece tres veces, el problema está un nivel por encima.

## Por qué importa

Es la disciplina que llevó del SharePoint manual al avatar-lang formal: se podía parchear cada incidente de "información perdida" con más documentación, pero la solución real era subir a un DSL que el compilador valida. Mismo patrón en cada salto evolutivo del aparato.

## Anécdotas que lo sostienen

- [Obsidian + Wikilinks — descubrimiento marzo](../historias/obsidian-wikilinks-marzo.md)
- [Akdong — migración 10 días enero](../historias/akdong-migracion-10-dias.md)

```avatar-lang
@id: elevar-en-vez-de-parchear
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
