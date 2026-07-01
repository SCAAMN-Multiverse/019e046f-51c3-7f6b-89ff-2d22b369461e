# Planificación resiliente — el plan asume que cambiará

Un plan no es un compromiso; es un punto de partida. Si la naturaleza del proyecto cambia a mitad, el plan se replantea — no se rompe. La capacidad de re-planificar es parte de la planificación misma.

## Por qué importa

Es la lección que PRINCE2 no captura: en la práctica no entras en mantenimiento puntual, estás en transformación continua. El caso Disputas (modelo evolutivo rechazado por la usuaria, reorientado a MVPs sucesivos) es ejemplo canónico.

## Ciencia subyacente

- [PRINCE2 — gestión por excepción](./ciencia-prince2-gestion-por-excepcion.md)
- [Antifragilidad — Taleb](./ciencia-antifragilidad-taleb.md)

## Anécdotas que lo sostienen

- [W2M — Disputas: cambio de naturaleza del proyecto](../historias/w2m-disputas-cambio-naturaleza.md)

```avatar-lang
@id: planificacion-resiliente
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
