---
hito: cumplir-regla-14
estado: DECISION_CERRADA
sigue-a: []
precede-a: []
fecha: 2026-05-08
destino: [scaa]
---

# Laguna: cumplir la regla 14 en `scaa` (md sin bloque `avatar-lang`)

Dirección abierta, decidida pero aún sin ejecutar. Nace del barrido global del compilador
`check-avatar-lang.ts` el 2026-05-08: los md de `scaa/[estado-actual]/presentaciones/` que
son unidades operativas no llevan el bloque `avatar-lang` que la **regla 14** exige (un
`@id` + al menos un `state ... terminal ...` + al menos un `action ...`). Sin ese bloque el
compilador no puede usarlos como piezas referenciables cross-avatar (`requires-from`, etc.),
y disparan warning de regla 14.

## Qué se haría

1. Por cada md afectado, leer su estado terminal natural (qué cierra el md cuando está
   completo) y derivar la FSM mínima.
2. Añadir el bloque `avatar-lang` al final del md, siguiendo
   `../../../019d8dc4-d3e0-76ca-b047-70e2b5b71674/avatar-mind/scaa/[estado-actual]/structure/data-structure/avatar-lang.md`
   § *Estructura canónica del doc*.
3. Re-correr el compilador acotado (`npm run check -- --avatar=019e046f-51c3-7f6b-89ff-2d22b369461e`)
   y comprobar que el conteo de warnings de regla 14 baja a cero.

## Naturaleza

Es mantenimiento puro: no añade ni cambia conocimiento del sistema-operado, solo formaliza
lo existente para que el motor lo trate como unidad. Por eso queda como laguna de baja
prioridad — se trabaja cuando convenga, sin urgencia. Estos warnings son materia preexistente,
no los crea ninguna migración estructural.

## Ver también

- `../../../019d8dc4-d3e0-76ca-b047-70e2b5b71674/avatar-mind/scaa/[estado-actual]/structure/data-structure/avatar-lang.md` — la regla 14 y la estructura canónica del bloque.
