# Fricción estructura-cliente como costo invisible

La estructura de gestión interna de la consultora puede no encajar con la del cliente — y cuando no encaja, el coste es invisible pero alto: dos críticas simultáneas caen sobre la misma persona porque la consultora reparte por capacidad y el cliente espera atención por dominio. Nadie lo ve hasta que estalla.

## Por qué importa

Hay que mapear la estructura del cliente (en C. de Madrid: directora → funcionarios → cada funcionario un dominio con sus aplicaciones, fechas y prioridades) y alinear la del equipo a ella, no al revés. La fricción no se resuelve hablándolo — se resuelve estructuralmente.

## Anécdotas que lo sostienen

- [Comunidad de Madrid — CMMI](../historias/comunidad-madrid-cmmi.md)
- [BBVA — portfolio y trenes de release](../historias/bbva-portfolio-trenes-release.md)

```avatar-lang
@id: friccion-estructura-cliente
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
