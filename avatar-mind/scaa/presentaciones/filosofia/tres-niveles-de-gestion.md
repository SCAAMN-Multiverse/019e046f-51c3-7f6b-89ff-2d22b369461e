# Tres niveles de gestión — proceso, proyecto, portfolio

Distinguir tres planos que se mezclan habitualmente: **Nivel 1** proceso de ingeniería (waterfall vs evolutivos, dentro de un sprint); **Nivel 2** gestión de proyecto (OKR → hitos → versiones); **Nivel 3** estrategia empresarial (portfolio multi-departamento, trenes de release). Cada nivel tiene fricciones distintas y rodaje IA distinto.

## Por qué importa

Evita prometer impactos de IA en planos donde no llega. La IA acelera bien el Nivel 1 (código, pruebas, integración); aporta valor incipiente en Nivel 2 (síntesis, anticipación de riesgos); es marginal en Nivel 3 (negociación política, compromisos cross-departamentales).

## Ciencia subyacente

- [PRINCE2 — gestión por excepción](./ciencia-prince2-gestion-por-excepcion.md)

## Anécdotas que lo sostienen

- [BBVA — portfolio y trenes de release](../historias/bbva-portfolio-trenes-release.md)
- [Comunidad de Madrid — CMMI](../historias/comunidad-madrid-cmmi.md)
- [Inditex — outage de fin de semana](../historias/inditex-outage-fin-de-semana.md)

```avatar-lang
@id: tres-niveles-de-gestion
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
