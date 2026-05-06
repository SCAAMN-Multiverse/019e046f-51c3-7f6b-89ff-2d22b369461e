# Analogía cloud antes de Istio — dónde estamos hoy con la IA

Estamos con la IA exactamente en la misma fase en la que estaba el cloud antes de Istio.

**Lo que pasó con el cloud y los sistemas distribuidos.** Al principio, alquilar cloud parecía mucho más barato que tener servidores on-premise. Pero había mucho trabajo invisible: antes de **Istio** los equipos de desarrollo tenían que **programarse las herramientas de plataforma a mano** — tomaban prestado material de Netflix (Hystrix, Eureka, Zuul…) y lo ensamblaban ellos. Los equipos de desarrollo se quedaron con la responsabilidad de la plataforma además del producto. El aparente abaratamiento se compensaba con explosión del coste de desarrollo. Hoy, gracias a Istio y similares, ese problema está resuelto: API Gateway, service mesh, observabilidad — todo eso lo asume una capa de plataforma reutilizable; el equipo de plataforma se encarga de la plataforma; el de desarrollo se encarga del producto.

**El traslado a IA.** Promesa pública: *"con IA hago todo solo y barato"* (igual que *"alquilar cloud es más barato que servidores propios"*). Realidad: requiere mucho trabajo invisible de plataforma que cada equipo está reinventando — context engineering, gestión de prompts, coherencia inter-agente, observabilidad. Y quien hace la chapuza son, otra vez, los equipos de desarrollo asumiendo responsabilidad de la "plataforma de IA".

## La pregunta abierta

**¿Cuál será el "Istio de la IA"?** ¿Qué capa va a aparecer que estandarice esta plataforma de soporte para que los equipos de desarrollo dejen de reinventarla? El equipo del humano sostiene una respuesta parcial: **SCAAMN aspira a ser parte de esa capa** — no el "Istio" entero, pero sí un patrón formalizado (avatar como unidad, capability registry, manager, ciclo evolutivo, avatar-lang) que cualquier equipo puede adoptar como infraestructura reutilizable.

## Filosofías que enlaza

- [Realidad ingenieril — el aparato invisible](./realidad-ingenieril-aparato-invisible.md)
- [Las dos líneas — evolución vs degeneración](./dos-lineas-evolucion-vs-degeneracion.md)
- [Elevar en vez de parchear](./elevar-en-vez-de-parchear.md)

## Anécdotas que lo sostienen

- [Sorolla — arquitectura, migración Java 6→8 + microservicios](../historias/sorolla-arquitectura.md)
- [SEPE — migración Struts → Spring + Spring Webflow](../historias/sepe-migracion-struts-spring.md)
- [Telefónica — procesos SOA, Enterprise Architect](../historias/telefonica-procesos-soa.md)
- [Inditex — outage de fin de semana, sistemas distribuidos](../historias/inditex-outage-fin-de-semana.md)
