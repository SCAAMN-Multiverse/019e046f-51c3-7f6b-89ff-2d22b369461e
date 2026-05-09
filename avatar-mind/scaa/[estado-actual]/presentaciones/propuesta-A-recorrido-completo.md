Vale, pues te voy a escribir ahora mismo sin un orden concreto. Te voy a decir que es lo que me gusta de unas propuestas y otras, y primero tú y yo vamos a condensarlo, ¿vale? para llegar a una estructura y luego se la pasamos al arquitecto para que lo genere.

A ver, de la propuesta, hay, o sea, lo que no me gusta en general de ninguna de las tres propuestas es que me gustaría que fuera un poco más condensado. O sea, me gustaría que se quedara con la filosofía y con la ciencia que hay detrás, no tanto con las historias. Las historias me gustaría que las utilizara solamente, cosa que me las dejara ahí puestas, por si tengo que hacer en un momento determinado una referencia. Yo las historias ya las conozco, pero lo que necesito en el esquema es conocer exactamente qué es lo que tengo que hablar en cada uno de ellos. # Propuesta A — Recorrido completo

**Sirve mejor a:** audiencia técnica que necesita entender el viaje completo (Juan + comité técnico, equipo Plexus, perfiles ingeniero senior). **Énfasis:** narrativa lineal pasado → presente → propuesta → caso real, sin saltos.

## Slides

1. **De dónde venimos — 4 fases del uso profesional de IA** (5 min). ChatGPT 2023 → Copilot → Agentes → Claude Code como operador. Anécdotas Inditex (fase 1) y W2M batch (fase 2).
2. **No impacta igual a todos: la IA es herramienta cultural** (4 min). Tesis perfiles. Junior 150h Java vs senior dilatado: misma IA, distinto multiplicador.
3. **Lo verdaderamente difícil es la gestión** (4 min). Síntomas, disfunciones, dilema confianza/autonomía. Tres niveles: proceso ingeniería / proyecto / portfolio empresa. Caso BBVA — Nivel 3 sin rodaje IA.
4. **Estado de partida W2M/Plexus** (4 min). Stack humano (Teams/Discord/Jira/Redmine) + técnico cliente (Azure DevOps/Tecton/Backstage) + intranet propia SharePoint.
5. **El dilema estructural — la intranet funciona y no funciona** (5 min). Caso éxito doble. PRINCE2 + caso Disputas. Sustrato cognitivo: la herramienta no salva al sustrato.
6. **Estado actual de los agentes** (4 min). Capacidad bruta, requisitos (Git/worktrees), Claude bien usado. Mismo dilema cognitivo en silicio.
7. **Cronología técnica: cómo nació SCAAMN** (6 min). 24 hitos condensados — Akdong → Obsidian → ciclo EXPLORE/PLAN/DO/CHECK/RELEASE → estratificación scaa/narrative/meta-narrative.
8. **Cómo los avatares mejoran la gestión hoy** (8 min). De semanas a horas en IDEAR. Triada executor/planner/checker. Tres capacidades: certificación, I+D+i nocturna, tren-del-release.
9. **Cifras y comparativas** (4 min). ROI 2,1 M €/año conservador, 3,5× realista. 690–1.150 reemplazos/año en Plexus. vs Copilot/Cursor/Indra/GFT.
10. **Aparato SCAAMN — capas** (5 min). Herramientas, ciencia (FIPA-BDI, Maturana-Varela, Shu-Ha-Ri), filosofía, procesos.
11. **Cierre** (3 min). Por qué no se queda desfasado: autoconsciente y evolutivo.

**Pros:** completo; cada decisión justificada; audiencia técnica termina con modelo mental sólido. **Contras:** ~52 min, largo; pierde a audiencia ejecutiva en slides 1–4; el "punch" tarda en llegar (slide 8).

**Recomendable si:** audiencia técnica con tiempo, primera exposición al sistema, o decisión a 3+ meses vista.
**No recomendable si:** comité ejecutivo, slot ≤30 min, o audiencia que ya conoce el problema y quiere la respuesta.

```avatar-lang
@id: propuesta-a-recorrido-completo
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
