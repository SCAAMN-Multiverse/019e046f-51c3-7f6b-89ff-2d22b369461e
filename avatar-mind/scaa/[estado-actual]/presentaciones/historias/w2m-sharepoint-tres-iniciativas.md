# W2M — SharePoint: tres intranets como caso de éxito doble

Decisión interna del equipo Plexus en W2M, tomada desde el primer momento: **centralizar gestión de equipo + gestión de proyecto en un punto único**. Herramienta elegida: SharePoint. Hoy hay tres intranets activas, una por iniciativa: **Portfolio** (gestión transversal), **Disputas** (proyecto concreto) y **World Unite Academy**. **Caso de éxito doble**: funciona y no funciona simultáneamente. Funciona porque despliegue a producción, diagnóstico de fallos e incorporación de herramientas nuevas operan ya sin pasar por el humano. No funciona porque, aunque el marco está perfectamente estructurado y publicado, la gente sin sustrato cognitivo se pierde — la información está pero no se usa.

## Filosofías que sostiene

- [El sustrato cognitivo importa](../filosofia/el-sustrato-cognitivo-importa.md)
- [Persistencia fuera de la cabeza](../filosofia/persistencia-fuera-de-la-cabeza.md)
- [Sistema-operado como fuente de verdad](../filosofia/sistema-operado-fuente-de-verdad.md)
- [Avatar personal derivado](../filosofia/avatar-personal-derivado.md)

```avatar-lang
@id: w2m-sharepoint-tres-iniciativas
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
