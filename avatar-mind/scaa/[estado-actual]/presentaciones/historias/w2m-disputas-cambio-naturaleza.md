# W2M — Disputas: cambio de naturaleza del proyecto a mitad

El cliente W2M pidió una aplicación para gestionar **disputas**, entrega prevista en junio. El proyecto pasó por **muchos estadios de madurez** que cambiaron cómo se gestionaba en cada momento. Modelo inicial: **evolutivo**, entregas incrementales por hitos para que el cliente las usara progresivamente. Giro: la usuaria del cliente **rechazó** ese modelo y casi pierden el proyecto. Reorientación: entregar todo pero como **MVP** para que viera el conjunto; después un segundo MVP, un tercero, refinándose. Cierre del giro: la usuaria finalmente aceptó y ahora se trabaja sobre la versión definitiva. **La naturaleza del proyecto cambió por completo a mitad** — eso es lo que PRINCE2 no captura.

## Filosofías que sostiene

- [Planificación resiliente](../filosofia/planificacion-resiliente.md)
- [El sustrato cognitivo importa](../filosofia/el-sustrato-cognitivo-importa.md)
- [Velocidad del cambio deshace cualquier armonía](../filosofia/velocidad-deshace-armonia.md)
- [PRINCE2 — gestión por excepción](../filosofia/ciencia-prince2-gestion-por-excepcion.md)

```avatar-lang
@id: w2m-disputas-cambio-naturaleza
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
