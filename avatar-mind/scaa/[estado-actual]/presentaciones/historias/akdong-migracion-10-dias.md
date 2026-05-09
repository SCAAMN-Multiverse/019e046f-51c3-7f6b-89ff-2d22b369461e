# Akdong — migración entera en 10 días (enero 2025)

Enero de 2025. Primer experimento serio del equipo con un agente moderno: migración entera del proyecto Akdong en **10 días**. Es el hito que cambia la percepción del humano sobre lo que un agente puede hacer: el trabajo del operador se transforma — pasa de **picar código** a **explicarle el contexto al agente**. De aquí salen, una tras otra, la "fatiga del prompt", la paradoja del contexto, y todas las decisiones arquitectónicas que llevan al aparato SCAAMN.

## Filosofías que sostiene

- [Del agente al avatar](../filosofia/del-agente-al-avatar.md)
- [Lazy context y MDs composables](../filosofia/lazy-context-mds-composables.md)
- [Triada de ejecución](../filosofia/triada-de-ejecucion.md)
- [Cascade local-vs-frontier](../filosofia/cascade-local-vs-frontier.md)
- [Elevar en vez de parchear](../filosofia/elevar-en-vez-de-parchear.md)

```avatar-lang
@id: akdong-migracion-10-dias
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
