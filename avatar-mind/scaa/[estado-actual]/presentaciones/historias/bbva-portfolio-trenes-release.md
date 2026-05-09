# BBVA — portfolio multi-departamento y trenes de release

En BBVA (caso vivido en primera persona; por extensión también Banco Santander) la estrategia empresarial abarca **muchos departamentos** trabajando sobre un **portfolio común** que se divide en muchos proyectos. Como muchos proyectos deben coordinarse entre sí para que la estrategia avance, hace falta interconectar equipos y departamentos: de ahí los **"trenes de release"**, cadenas coordinadas de releases desde la idea inicial hasta producción que sincronizan equipos que de otra forma no podrían entregar a la vez. Es el escenario donde la IA tiene **menos rodaje** — Nivel 3 (estrategia empresarial multi-departamento) sigue siendo trabajo humano.

## Filosofías que sostiene

- [Tres niveles de gestión](../filosofia/tres-niveles-de-gestion.md)
- [Fricción estructura-cliente](../filosofia/friccion-estructura-cliente.md)
- [El sustrato cognitivo importa](../filosofia/el-sustrato-cognitivo-importa.md)

```avatar-lang
@id: bbva-portfolio-trenes-release
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
