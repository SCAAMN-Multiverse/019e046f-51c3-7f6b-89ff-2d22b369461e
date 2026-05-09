# W2M — Cherry-pick rescatado por compañero competente

Un compañero hizo una batería de tests en una rama. No se quería traer entera a la principal, pero un merge directo era imposible (incompatibilidades). Solución: **cherry-pick del commit concreto** que tenía las novedades, ignorando el resto, **reescribiendo la historia de Git por debajo**. Esto no lo sabe hacer cualquiera. Un agente que ejecutase "merge esto" sin entender el problema lo rompería seguro. Caso canónico de por qué la pareja **agente + humano-no-especialista** es el peor escenario: la velocidad del agente convierte en irreversibles errores que un humano lento habría detectado a tiempo.

## Filosofías que sostiene

- [El sustrato cognitivo importa](../filosofia/el-sustrato-cognitivo-importa.md)
- [Del agente al avatar](../filosofia/del-agente-al-avatar.md)
- [Soft warning no corta](../filosofia/soft-warning-no-corta.md)
- [Analogía cloud antes de Istio](../filosofia/analogia-cloud-pre-istio.md)

```avatar-lang
@id: w2m-cherry-pick-rescatado
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
