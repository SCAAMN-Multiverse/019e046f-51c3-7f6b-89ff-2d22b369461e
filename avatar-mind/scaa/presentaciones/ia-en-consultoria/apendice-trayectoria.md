# Apéndice — Trayectoria profesional del humano

Resumen: Material de respaldo, no contenido principal de slides. Citado desde **2.2** (senior dilatado vs junior 150h Java) y desde **5.4** (legitimidad del diseño de la intranet — visión transversal acumulada). Justifica que el equipo ha cubierto la función de arquitectura más allá del oficio nominal, y que el humano tenía claro qué meter y qué no meter en SharePoint.

## Resumen ordenado de la trayectoria

- **Telefónica** (3 años, analista funcional) — departamento problema cliente + departamento calidad y SLAs. Modelado de procesos de negocio con **Enterprise Architect**, paso a diseño técnico, arquitectura **SOA distribuida**.
- **SEPE** — migración **Struts → Spring + Spring Webflow** (gestión mediante procesos). Aportó la experiencia previa de modelado funcional de Telefónica.
- **Comunidad de Madrid (interventores de concesiones)** — diseño de la aplicación para interventores de concesiones de carreteras. Sistema de control de facturación mes a mes contra el trabajo realizado por la empresa concesionaria. Diseño desde cero hablando con el funcionario del Ministerio de Transporte; construcción delegada al equipo de Cantabria.
- **Comunidad de Madrid (capa servicio CMMI/SLAs)** — la C. de Madrid trabaja bajo **CMMI**: modelo de calidad que sustituye el mantenimiento ITIL flexible por **SLAs rígidos** (ej.: aplicación crítica → resolución en 3 horas; si no llegas, penalización económica directa sobre la facturación del mes). Además de diseñar CFTO, gestionó mantenimiento de **15 aplicaciones simultáneamente**. Caso vivido: ante dos críticas simultáneas avisaba a los funcionarios; respuesta literal del cliente: *"Ese no es nuestro problema, son dos críticas y para eso os hemos contratado"*. **Aprendizaje no obvio**: la estructura de gestión de la consultora puede no encajar con la del cliente — en C. de Madrid: directora → funcionarios → cada funcionario es un dominio con sus aplicaciones, fechas y prioridades; si la consultora reparte ingenieros sin alinear con esos dominios, dos críticas pueden caer sobre la misma persona.
- **Intervención General del Estado / Sorolla** — 50 ingenieros dando mantenimiento y mejora a Sorolla (gestión económica de portfolios estatales). En 6 meses los propios compañeros eligieron al humano para pasarlo al departamento de arquitectura. Estando allí desbloqueó la migración **Java 6 → Java 8** y acompañó el paso a **microservicios**.
- **Inditex** (líder técnico) — outage de fin de semana de jueves a lunes: **1 millón de pedidos sin procesar** por la aplicación de empaquetado. El lunes hubo que escalar de **2 nodos a 14 nodos durante 3 horas** para procesar todo el backlog. Además: arquitectura **Hexagonal**, **Kafka**, sistemas distribuidos, mucho conocimiento DevOps/Kubernetes en proyectos grandes.

## Tesis derivada

Gracias a esta visión transversal, cuando arrancó SharePoint el humano tenía muy claro **qué meter y qué no meter** en la intranet en cada momento. Por eso hoy la **gestión del proyecto está alineada con la gestión del equipo** (no son dos planos separados, comparten estructura) y ese modo de trabajar está **pactado con el usuario** (cliente acepta cómo se opera). Conecta directamente con la tesis 2.2 (senior dilatado vs junior 150h Java).

```avatar-lang
@id: apendice-trayectoria
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
