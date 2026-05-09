# Comunidad de Madrid — diseño CFTO para interventores de carreteras

Diseño de la aplicación para **interventores de concesiones de carreteras** de la Comunidad de Madrid. Sistema de **control de facturación mes a mes** contra el trabajo realizado por la empresa concesionaria. Diseño desde cero hablando directamente con el funcionario del Ministerio de Transporte; construcción delegada al equipo de Cantabria. Caso de "diseño funcional + gestión cross-equipo" que el humano cubrió por encima de su rol nominal de mantenimiento.

## Filosofías que sostiene

- [Fricción estructura-cliente](../filosofia/friccion-estructura-cliente.md)
- [Realidad ingenieril — el aparato invisible](../filosofia/realidad-ingenieril-aparato-invisible.md)

```avatar-lang
@id: comunidad-madrid-cfto
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
