# 1. De dónde venimos: evolución reciente del uso profesional de IA (cuatro fases)

Resumen: Contexto narrativo de arranque. Sitúa al oyente en la trayectoria reciente del uso profesional de IA — de chatbot externo a operador del propio ordenador — para que los retos (punto 2), la propuesta de aplicación (punto 3) y el caso real SCAAMN (punto 4) se entiendan sobre fondo conocido. Cuatro fases evolutivas, cada una un salto cualitativo respecto a la anterior.

## 1.1. Fase 1 — 2023: ChatGPT como interlocutor

Resumen: Chat conversacional con un LLM general. La IA guía, sugiere, explica; el humano sigue haciendo todo el trabajo manualmente (copia y pega código, traduce respuestas a su contexto, ejecuta). El valor está en tener un "experto disponible 24/7", pero el flujo de trabajo apenas cambia.

### 1.1.1. Caso vivido: ChatGPT como fuente primaria de búsqueda en una reunión (Inditex, líder técnico)

Resumen: Anécdota en primera persona que ilustra concretamente la fase 1. Cambio de hábito de búsqueda — antes de ChatGPT el primer ciclo era Stack Overflow (problemas puntuales de código) + tutoriales web (cómo se monta X); ChatGPT sustituye ese primer ciclo y se convierte en fuente primaria, ya no se va a Google ni a Stack Overflow primero.

Caso concreto: en Inditex había que decidir cómo empaquetar productos (qué tamaño de caja y cómo ordenar dentro). Existía algoritmo, pero las **reglas de empaquetado cambian mucho con el tiempo**, así que el equipo quería que el algoritmo soportase reglas de negocio que el usuario pudiera meter directamente sin re-codificar.

Lo que pasó en la reunión: el líder técnico preguntó **en directo durante la reunión** a ChatGPT qué business rules de empaquetado se usan en el sector. ChatGPT devolvió tres o cuatro candidatas en segundos. **En paralelo**, un compañero consultó la **IA interna de Inditex** (asistente entrenado sobre la documentación de arquitectura propia) para verificar cuál de esas reglas estaba realmente desplegada en sus sistemas. Resultado: una de las que ChatGPT había sugerido era exactamente la que ya estaba en uso.

Por qué importa para la presentación: la decisión a nivel producto y técnico se tomó **dentro de la propia reunión**, sin diferir a "lo investigo y os digo mañana". Ese acortamiento del ciclo investigación-decisión es el valor real de la fase 1 aplicada a un equipo de consultoría. Y muestra una pieza clave: combinar **IA generalista** (ChatGPT) con **IA específica del cliente** (asistente sobre documentación interna) para validar lo que la generalista propone.

## 1.2. Fase 2 — GitHub Copilot: la IA dentro del proyecto

Resumen: La IA pasa a vivir dentro del IDE / del proyecto. Lee el código circundante, intuye lo que estás a punto de escribir, autocompleta funciones enteras. Cuando acierta, la aceleración es radical (tareas de una hora resueltas en cinco minutos); cuando falla, hay coste de descartar sugerencias. El cambio cualitativo: la IA "ve" tu proyecto por primera vez.

### 1.2.1. Caso vivido: ChatGPT + Copilot acelerando un producto batch en World2Meet

Resumen: Anécdota en primera persona que ilustra concretamente la fase 2 — contrapartida de la 1.1.1 (Inditex / fase 1). Etapa actual del humano en **World2Meet** (W2M, agencia turística): el modo de trabajo durante mucho tiempo ha sido el combo **ChatGPT + GitHub Copilot**. La ventaja del combo es que permite abordar productos complicados en tiempos breves: la IA dentro del IDE acelera el código, ChatGPT acelera la investigación previa.

Caso concreto: gestión de hoteles vía procesos batch. W2M maneja un volumen muy grande — **miles de proveedores de hoteles, millones de hoteles, miles de millones de habitaciones** — y el equipo necesitaba que ese volumen fuese exportable y manipulable en Excel por usuarios de negocio. Para mover ese volumen entre sistemas hubo que diseñar **procesos batch**, notoriamente complicados (orquestación, reintentos, ventanas de ejecución, dependencias entre jobs, observabilidad, idempotencia).

Resultado: con IA integrada en el flujo de trabajo (ChatGPT + Copilot), el producto se implementó **completo entre junio y agosto — dos meses** para un reto que sin IA habría sido mucho mayor en tiempo y esfuerzo.

Por qué importa para la presentación: muestra que el salto de **IA-como-buscador** (fase 1) a **IA-dentro-del-proyecto** (fase 2) no solo cambia la velocidad de búsqueda — cambia la **viabilidad de productos enteros**.

## 1.3. Fase 3 — Agentes: alcance a nivel proyecto entero

Resumen: Aparecen los agentes. Ya no solo completan en línea: aceptan tareas de alcance amplio ("revisa todo el proyecto, dime dónde están los puntos calientes"; "implementa esta feature tocando los ficheros que haga falta"). El humano deja de ir línea a línea y empieza a delegar trabajos completos.

## 1.4. Fase 4 — Claude Code: la IA actúa sobre el ordenador

Resumen: El asistente (Claude Code) ya no se limita al proyecto: tiene acceso a la CLI del sistema operativo y a servidores **MCP** (Model Context Protocol) que le permiten conectarse a sistemas externos (Gmail, Drive, calendarios, bases de datos, modelos locales, lo que sea). La IA deja de ser asistente y pasa a ser **operador**: ejecuta comandos, lee y escribe ficheros, llama APIs en el contexto real del humano. Es el salto que está cambiando cómo trabajamos hoy.
