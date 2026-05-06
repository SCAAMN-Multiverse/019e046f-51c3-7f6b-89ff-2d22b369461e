# Ciencia — FIPA-BDI y el problema del estado opaco (años 2000)

**FIPA-ACL / KQML / BDI** (Belief-Desire-Intention) fue el intento serio de los años 90-2000 de formalizar agentes inteligentes con estados mentales internos verificables. Fracasó precisamente ahí: los estados internos del agente no son inspeccionables fiablemente. El mismo problema reaparece hoy con los LLMs.

## Lección que el aparato extrae

Lo que fracasó como verificación interna se reformula como verificación externa: **avatar-lang** declara estados públicos en grafo BPMN; el checker valida sobre los estados declarados, no sobre creencias del modelo. La opacidad del LLM se convierte en restricción arquitectónica, no en obstáculo.

## Filosofías que sostiene

- [Estados externos públicos, no internos](./estados-publicos-no-internos.md)
- [Del agente al avatar](./del-agente-al-avatar.md)
- [Triada de ejecución](./triada-de-ejecucion.md)
