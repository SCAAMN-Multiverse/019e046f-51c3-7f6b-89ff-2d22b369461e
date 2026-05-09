# W2M — Springpack: GC de la JVM y reparto de memoria del contenedor

Aportación técnica del humano al cliente W2M para Excels masivos con Springpack. La solución completa requirió **cambiar el recolector de basura de la JVM** y **reorganizar la memoria del contenedor**: split entre servidor (Apache o Netty) y aplicación. Si das de más memoria a la app, ésta la usa, y si no está bien repartido la app puede comerse al servidor en runtime. Es ejemplo del tipo de problema "invisible" que el equipo absorbe sin que figure en el rol nominal.

## Filosofías que sostiene

- [Realidad ingenieril — el aparato invisible](../filosofia/realidad-ingenieril-aparato-invisible.md)
- [Elevar en vez de parchear](../filosofia/elevar-en-vez-de-parchear.md)

```avatar-lang
@id: w2m-springpack-jvm
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
