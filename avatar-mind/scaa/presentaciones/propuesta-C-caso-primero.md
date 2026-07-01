# Propuesta C — Caso primero

**Sirve mejor a:** audiencia escéptica que ha visto demasiados *AI pitches* y exige ver el sistema funcionando antes de aceptar la teoría (perfiles arquitectura cliente, técnicos veteranos, comité auditor). **Énfasis:** demo / caso real al principio; el "por qué" se desbobina hacia atrás.

## Slides

1. **Esto está funcionando hoy** (5 min). Demo o captura del aparato SCAAMN operando en W2M (proyecto Disputas). Dashboard tren-del-release [019de212-0508-78b4-af1b-55fc84bbde14] con 8 agentes coordinados. Caso real, no maqueta. Cifras de uso reales del último mes.
2. **Cómo se ve la operativa diaria** (4 min). Despliegue a producción autónomo desde la intranet. Diagnóstico de fallos sin pasar por el líder técnico. Tres iniciativas vivas: Portfolio, Disputas, World Unite Academy.
3. **¿Y la IA dónde está?** (5 min). Triada executor/planner/checker. avatar-lang como lenguaje formal con compilador de 4 pases (Parse/Link/Validate/Index) y 16 reglas. Política rectora: *"si la condición merece atención, debe ser hard-fail; si no merece bloquear, no merece notificarse"*.
4. **Por qué hizo falta inventar avatar-lang** (4 min). El estado interno de un agente LLM es opaco — mismo problema que FIPA-BDI años 2000 con agentes BDI. Solución Evolution-Art: estados externos públicos en grafo BPMN, verificación runtime con consenso humano-avatar.
5. **El dilema que dio origen al sistema** (5 min). Caso SharePoint en W2M: funciona y no funciona. Tres gaps acumulativos (conocimiento, asimilación, auto-responsabilización). El sustrato cognitivo no se compra, se construye — y caduca en 6 meses por velocidad del sector.
6. **Cronología — cómo llegamos aquí** (5 min). 24 hitos condensados: enero 2025 experimento Akdong → revelación del contexto repetido → cambio de nombre agente→avatar → cuatro preguntas fundacionales → ciclo evolutivo canónico → estratificación tri-temporal.
7. **Por qué importa para Plexus** (4 min). Rotación 15–25% = 690–1.150 reemplazos/año. Onboarding 2 sem en lugar de 6–8. Tres capacidades: certificación, I+D+i nocturna, tren-del-release. ROI 2,1 M €/año conservador, 3,5× realista.
8. **Cierre — qué se necesita para arrancar** (3 min). Piloto 30 días. Indicador medible al día 30: tiempo a primer commit productivo reducido en ~1 semana.

**Pros:** demuestra antes de explicar; desarma escepticismo de entrada; el "por qué" emerge como respuesta a preguntas reales del propio sistema. **Contras:** depende fuerte de la calidad de la demo (si falla, naufraga); ROI llega tarde (slide 7); audiencia ejecutiva pura puede impacientarse.

**Recomendable si:** demo sólida disponible; audiencia técnica veterana o auditora; slot 30–40 min.
**No recomendable si:** no hay demo en condiciones, slot <30 min, o decisor económico puro.

```avatar-lang
@id: propuesta-c-caso-primero
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
