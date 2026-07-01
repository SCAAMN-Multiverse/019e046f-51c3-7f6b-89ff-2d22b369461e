# El ejército de una persona — la fantasía viral de la IA

Versión actual de un patrón viejo: en su día los chavales abrían un canal de YouTube diciendo *"hago esto y gano un montón donde otros no la están ganando"*. Hoy la versión es *"monto N agentes y tengo una empresa entera por mí mismo"*. Es la fantasía que llena los reels de Instagram y los hilos virales sobre IA.

## Por qué importa

Es **real solo para tareas que caben dentro de la ventana de contexto del LLM**: una landing page, un script puntual, una web simple. Funciona como demo, no como producción enterprise. Confundir esa franja con la consultoría real es el error de framing más común que el equipo se va a encontrar en clientes y compañeros.

## Filosofías que enlaza

- [Realidad ingenieril — el aparato invisible](./realidad-ingenieril-aparato-invisible.md) (la contraparte)
- [Las dos líneas — evolución vs degeneración](./dos-lineas-evolucion-vs-degeneracion.md)
- [Del agente al avatar](./del-agente-al-avatar.md)

```avatar-lang
@id: ejercito-de-una-persona-ruido-viral
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
