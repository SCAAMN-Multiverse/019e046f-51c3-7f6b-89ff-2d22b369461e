# Quenda Medic — validación con agentes simulando pacientes y operadores

Aplicación del **tren-del-release v7.1** al proyecto Quenda Medic: **27 millones de visitas/paciente al año**, **67 hospitales** atendidos. Cada despliegue se valida con **agentes simulando pacientes, operadores e integraciones externas** dentro del tren-del-release: 8 agentes Claude Code coordinados (Project Manager, Tech Lead, Frontend, Backend, Data Engineer, QA, Security, DevOps) en 5 fases canónicas (Discovery → Architecture → Implementation → Quality → Delivery). El dashboard captura todos los eventos vía hooks nativos de Claude Code, los reemite por WebSocket en tiempo real, y los pinta — auditable, observable, AI Act-ready por construcción. *(Cifras procedentes del estudio de mercado de `departamento-ia` para Juan.)*

## Filosofías que sostiene

- [Triada de ejecución](../filosofia/triada-de-ejecucion.md)
- [Multi-avatar / multi-rol](../filosofia/multi-avatar-multi-rol.md)
- [Estados públicos no internos](../filosofia/estados-publicos-no-internos.md)
- [Soft warning no corta](../filosofia/soft-warning-no-corta.md)
