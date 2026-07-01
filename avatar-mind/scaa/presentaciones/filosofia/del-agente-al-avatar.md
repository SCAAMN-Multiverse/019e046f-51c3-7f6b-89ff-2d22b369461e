# Del agente al avatar — siempre hay un humano dentro del traje

Un agente IA no es inteligente por sí mismo: es un ejecutor rápido sin sustrato. El **avatar** es el sistema completo *humano + IA + estructura externa*. La distinción no es retórica — cambia qué se puede delegar, qué se debe verificar, y dónde vive la responsabilidad. Analogías: Sully en *Avatar* (humano dentro del cuerpo na'vi), Tony Stark dentro del traje Iron Man.

## Por qué importa

Define el contrato real de uso: la velocidad del agente solo da ventaja si el humano que lo pilota sabe lo que pide y cómo verificarlo. Sin esa pareja, el agente convierte en irreversibles errores que un humano lento habría detectado.

## Ciencia subyacente

- [FIPA-BDI y el estado opaco](./ciencia-fipa-bdi-y-estado-opaco.md)

## Anécdotas que lo sostienen

- [Cambio de nombre agente → avatar](../historias/cambio-nombre-agente-a-avatar.md)
- [W2M — Cherry-pick rescatado por compañero competente](../historias/w2m-cherry-pick-rescatado.md)

```avatar-lang
@id: del-agente-al-avatar
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
