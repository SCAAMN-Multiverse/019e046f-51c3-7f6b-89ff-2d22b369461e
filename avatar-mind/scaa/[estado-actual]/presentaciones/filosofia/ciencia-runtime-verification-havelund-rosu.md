# Ciencia — Runtime verification (Havelund & Roşu)

**Klaus Havelund** y **Grigore Roşu** formalizaron *runtime verification*: comprobación de propiedades temporales (LTL, CTL) sobre trazas de ejecución. Asume ejecutores deterministas — supuesto que se rompe con LLMs.

## Lección que el aparato extrae

El gap entre runtime verification clásica (ejecutor determinista) y la realidad LLM (ejecutor probabilístico) justifica externalizar el estado al grafo BPMN/avatar-lang. La verificación no se hace sobre la traza interna del LLM; se hace sobre los estados públicos que el avatar declara haber alcanzado. Es el puente entre la tradición formal y la práctica con modelos generativos.

## Filosofías que sostiene

- [Estados externos públicos, no internos](./estados-publicos-no-internos.md)
- [Triada de ejecución](./triada-de-ejecucion.md)
- [Soft warning no corta](./soft-warning-no-corta.md)

```avatar-lang
@id: ciencia-runtime-verification-havelund-rosu
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
