# Inditex — empaquetado de productos: ChatGPT en reunión

En Inditex había que decidir cómo empaquetar productos (qué tamaño de caja y cómo ordenar dentro). Las reglas de empaquetado cambian con el tiempo, así que el equipo quería un algoritmo que aceptara reglas de negocio metidas por el usuario sin recodificar. **Durante la reunión en directo**, el líder técnico preguntó a ChatGPT qué business rules de empaquetado se usaban en el sector; ChatGPT devolvió 3-4 candidatas en segundos. En paralelo un compañero consultó la **IA interna de Inditex** (sobre la documentación de arquitectura propia) para verificar cuál estaba realmente desplegada. Una de las que sugirió ChatGPT era exactamente la que estaba en uso. Decisión técnica tomada en la reunión, no diferida a "mañana".

## Filosofías que sostiene

- [El sustrato cognitivo importa](../filosofia/el-sustrato-cognitivo-importa.md)
- [Persistencia fuera de la cabeza](../filosofia/persistencia-fuera-de-la-cabeza.md)

```avatar-lang
@id: inditex-empaquetado
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
