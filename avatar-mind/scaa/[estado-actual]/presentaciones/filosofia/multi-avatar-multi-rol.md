# Multi-avatar / multi-rol — el multiverso especializado

No un avatar omnisciente, sino **muchos avatares especializados por rol** (front, back, diseño técnico, diseño funcional, QA, manager, etc.) que se coordinan vía contratos públicos (`capability registry`). Cada avatar tiene su `avatar-mind` y opera su sistema-operado; el multiverso es la red.

## Por qué importa

Replica la división de roles humana en consultoría sin perder coherencia: cada avatar profundiza en su dominio, los managers (multiverse-manager [019dedce-5e50-7559-8b65-b99c3705caec], manager) coordinan. Es la respuesta a "cómo escala el aparato más allá de un solo proyecto".

## Anécdotas que lo sostienen

- [Cambio de nombre agente → avatar](../historias/cambio-nombre-agente-a-avatar.md)

```avatar-lang
@id: multi-avatar-multi-rol
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
