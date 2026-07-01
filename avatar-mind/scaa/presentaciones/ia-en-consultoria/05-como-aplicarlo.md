# 5. Cómo vamos a aplicar IA en consultoría

Resumen: Punto que cierra el arco entre el problema (Punto 3) y la respuesta concreta (Punto 6). Empieza por el **estado de partida** real en tres planos — coordinación humana (5.1), stack técnico contra el cliente (5.2) e intranet propia del equipo (5.3) — sigue con el **dilema estructural** que descubre que la intranet "funciona y no funciona" (5.4), examina el **estado actual de los agentes IA** sobre los que vamos a apoyarnos (5.5), y deja en placeholder las **palancas concretas** de aplicación (5.6).

> Cross-ref de origen: el enfoque que se desarrollará aquí proviene de **casi dos años de trabajo del equipo del humano en World2Meet** atacando los problemas de gestión del Punto 3. Ver **6.1 (Génesis: dos años de trabajo en W2M)** para el contexto histórico y la tesis derivada (en W2M lo difícil es la coordinación de información, no la cadena física — escenario donde la IA puede tener más impacto).

## 5.1. Estado de partida — Stack de coordinación humana en W2M / Plexus

Resumen: Foto del stack real de coordinación que el equipo usa hoy, **antes** de hablar de qué aporta la IA. No son herramientas mágicas — son las que cualquier equipo de consultoría conoce, y sobre ellas es donde la IA tiene que aterrizar.

**Inventario actual**:

- **Teams** — reuniones con el cliente y reuniones internas del equipo. Canal corporativo por defecto.
- **Discord** — usado en paralelo a Teams porque mejora la **calidad de las reuniones internas** (audio, latencia, fluidez de conversación) frente a Teams. Nota interesante: el equipo ha tenido que recurrir a una herramienta no-corporativa para tener mejores reuniones.
- **Jira** — tickets compartidos con el cliente para que sepa en todo momento el **estado de la programación** (qué está hecho, qué está en curso, qué viene).
- **Redmine** — gestión de **horas invertidas** en cada proyecto, para cuadrar la contabilidad en **UTEs (unidades de tiempo)** entre World2Meet y Plexus. Pieza que conecta el trabajo realizado con la facturación del modelo UTE.

**Por qué importa**: este inventario define **dónde la IA tiene que entrar a aportar valor**. Si la IA va a ayudar en la coordinación (la dificultad principal en W2M, ver tesis de 6.1), tiene que dialogar con estas herramientas o sustituir parte del trabajo que se hace dentro de ellas. Cada herramienta marca un tipo de fricción distinto: reuniones (Teams/Discord), trazabilidad cliente (Jira), contabilidad (Redmine). Y muestra la realidad: hoy la coordinación de un proyecto de consultoría sigue dependiendo mayoritariamente de **herramientas humanas pre-IA**; la IA todavía no está sustituyendo este stack — todo lo más, lo asiste por los bordes.

## 5.2. Estado de partida — Stack técnico de coordinación con el cliente

Resumen: Complemento técnico al inventario humano de 5.1. La coordinación con el cliente W2M se hace contra **su** infraestructura (no la de Plexus): el equipo trabaja como invitado dentro de las herramientas que el cliente impone.

**Inventario técnico**:

- **Azure DevOps** — el cliente tiene allí su proceso de integración continua. El equipo empuja la información del proyecto a los repositorios de Azure DevOps del cliente y lanza allí las **PRs** (pull requests) para las revisiones de código entre miembros y con el cliente.
- **Tecton** — sistema de integración continua sobre **Kubernetes** del cliente, integrado con Azure DevOps. Gracias a esa integración los despliegues fluyen automáticamente a los distintos entornos: **TST** (test), **PRE** (pre-producción), **Stage** y **PRO** (producción).
- **Backstage** — sistema de documentación oficial del cliente. Decisión activa del equipo: Backstage es la **fuente de información de los proyectos**. Ventaja relevante (en teoría): permite ver la **arquitectura técnica** de los servicios — por ejemplo, mirando un servicio como "disputas", Backstage muestra qué microservicios usa internamente y con qué otros sistemas se relaciona.

**Por qué importa**: este stack técnico, igual que el humano, es donde la IA tiene que aterrizar. **Azure DevOps + Tecton** son candidatos a integración con agentes que automaticen revisiones de PR, detección de regresiones, generación de notas de release entre entornos. **Backstage** es candidato a fuente estructurada que un agente pueda leer para responder preguntas tipo "¿qué microservicios afecta este cambio?" sin que un humano tenga que ir a buscarlo. Realidad actual: estos sistemas operan **sin IA por defecto**; la IA aún no está integrada como ciudadano de primera en el ciclo Azure DevOps → Tecton → entornos → Backstage. La asisten por los bordes (sugerencias en PR, redacción de tickets, búsqueda en docs); la integración estructural sigue siendo trabajo pendiente.

## 5.3. Estado de partida — Frontera cliente/equipo e intranet propia: el problema del conocimiento

Resumen: Tercer plano del estado de partida. Trata de **qué pasa fuera de las herramientas del cliente** — el ámbito interno del equipo Plexus, donde no hay criterio impuesto por W2M y todas las decisiones son propias. Aquí vive el **problema del conocimiento atrapado** que justifica la decisión de centralizar en una intranet propia.

**Frontera cliente ↔ equipo Plexus**: el contacto con el cliente cubre solo dos vértices del trabajo: la **entrada de trabajo** y las **PRs de arquitectura**. Todo lo demás cae en ámbito interno del equipo, sin criterio establecido por el cliente sobre cómo hacerlo — decisión propia.

**Decisión interna — SharePoint como intranet del equipo**: tomada desde el primer momento, **centralizar gestión de equipo + gestión de proyecto en un punto único**. Herramienta elegida: **SharePoint** (intranet de Microsoft). Hoy hay tres intranets activas, una por iniciativa: **Portfolio** (gestión transversal), **Disputas** (proyecto concreto — el mismo "disputas" mencionado como ejemplo en Backstage en 5.2) y **World Unite Academy** (otra iniciativa).

**Por qué este cambio importa — contraste con el modelo anterior (caso Inditex)**: en proyectos como Inditex, cada miembro organizaba la información del proyecto a su manera; lo único realmente común entre todos era el **tablero del sprint**. Para todo lo demás (BD, configuraciones, herramientas, atajos, procesos): si necesitabas un enlace de la BD se lo pedías a un compañero; si no sabías cómo configurar algo se lo pedías a un compañero; si aparecía algo nuevo cada uno lo organizaba a su manera, típicamente en los **favoritos de su navegador**.

**El coste oculto — cuando alguien se va**: el conocimiento operativo del proyecto vive en dos sitios invisibles: (1) en la **cabeza** del trabajador (casos de uso que ni él mismo tiene siempre claros hasta que aparecen) y (2) en **cómo monta su entorno personal** (PC, navegador, scripts locales, accesos directos, atajos privados). Ejemplo concreto: si te dicen "sube esto a producción", te metes en contexto producción y vas recordando dónde tenías cada pieza; si te dicen "hoy hacemos testing", recuerdas otras herramientas, otros lanzadores. **¿Dónde está entonces el proceso real? ¿En la cabeza de la persona o en cómo ha montado su entorno?** Aunque la persona saliente te cediera su ordenador entero, sería como **mudarte a casa de otro**: muchas cosas no sabrías dónde están ni entenderías por qué están así. Hay que rehacer el contexto desde cero — y eso es trabajo perdido.

**Causa raíz**: el proceso natural de trabajar en **proyectos complejos con tiempos estrechos** hace que no se sigan buenas prácticas y no se documente como se debería. Cuando llega el momento de pensar "no voy a ser capaz de pasar esto a quien venga detrás", ya es tarde — el conocimiento ya está atrapado en cabezas y entornos.

**Por qué esto da sentido a la intranet centralizada**: la intranet SharePoint es la respuesta directa a este problema — un punto único, accesible para todo el equipo, donde la información del proyecto vive **fuera de la cabeza y fuera del entorno personal de cada uno**. Es la **pre-condición** para que cualquier IA aplicada después tenga algo sólido sobre lo que trabajar; sin esa base, la IA tampoco puede leer lo que no está escrito.

## 5.4. El dilema estructural — la intranet funciona y no funciona

Resumen: Cierre del arco abierto en 5.3. La intranet SharePoint, aunque bien diseñada y poblada con casi dos años de trabajo, es un **caso de éxito doble**: funciona y no funciona simultáneamente. Esa paradoja revela un **dilema estructural** que generaliza a los tres niveles de gestión del Punto 3 y prepara el terreno para entender por qué hace falta el aparato SCAAMN del Punto 6.

> Notas de respaldo: la legitimidad operativa de cómo se diseñó la intranet (qué meter y qué no meter en cada momento) descansa sobre la trayectoria transversal del humano — ver **[apéndice-trayectoria.md](./apendice-trayectoria.md)**. Y la credibilidad técnica del equipo ante el cliente, sobre aportaciones concretas como Springpack y los grafos cíclicos en BBDD W2M — ver **[apéndice-aportaciones-tecnicas.md](./apendice-aportaciones-tecnicas.md)**.

### 5.4.1. Lo que buscábamos y el caso de éxito doble

Resumen: La meta original con SharePoint era **tener todo en un mismo sitio + visión global compartida del proyecto** — por eso casi dos años invirtiendo en intranet. El resultado de esos dos años es que la intranet es un **caso de éxito doble**: funciona y no funciona al mismo tiempo. Las dos cosas son verdad simultáneamente, y eso es el aprendizaje principal de los dos años.

### 5.4.2. Lo que sí funciona — operativa diaria + ciclo de vida PRINCE2

Resumen: La parte de "funciona" tiene dos caras — la operativa diaria y el método que la sostiene.

**Operativa diaria que ya funciona sin pasar por el humano**: **despliegue a producción autónomo** (el equipo va al punto correspondiente de la intranet, ve los pasos y herramientas, y procede; antes era crítico y bloqueante, hoy es rutina documentada); **diagnóstico de fallos sin pasar por el humano** (cuando hay incidencia, el humano dice "David, échale un vistazo"; David entra en SharePoint y en herramientas internas — "Argos" [a confirmar] — y resuelve, independientemente de los enlaces personales en su navegador); **incorporación de herramientas nuevas** (cuando entran piezas — Tecton; OpenAPI con ApiFresh para que front y back trabajen contra la misma definición — se añade el enlace en la intranet; nada vive solo en la cabeza de quien lo introdujo). Resultado: el equipo opera sobre un **ciclo de vida de proyecto explícito**, no implícito.

**El truco metodológico — ciclo de vida desde PRINCE2**: idea aprendida al sacar la **certificación PRINCE2** — establecer cuál es el ciclo de vida desde que **nace** un proyecto hasta que **muere**, con sus estados intermedios. Lo que importa de verdad es un **criterio genérico de fases**: (1) **Inicio** del proyecto; (2) **Desarrollo** (con varias sub-fases internas); (3) **Cierre** del proyecto. Trabajo del jefe de proyecto: reunirse con el ejecutivo y acordar **tiempo, presupuesto, OKRs**; producir un **plan de proyecto** y confirmarlo con el ejecutivo; identificar **jefes de equipo por fase** que llevarán la gestión del equipo en cada etapa hasta el cierre. **Documento inicial del proyecto** — el documento maestro: memoria, gestión de calidad, gestión de riesgo, lecciones aprendidas, diario del proyecto. Marco general sobre el que la intranet instancia cada proyecto concreto.

### 5.4.3. PRINCE2 adolece — transformación continua + caso Disputas

Resumen: PRINCE2 funciona bien cuando se cumplen sus **premisas declaradas explícitamente**: el objeto de un proyecto es una **organización que se quiere transformar**; el proceso de transformación es **único** (no repetible); el tiempo es **limitado**. Sobre esa base, filosofías de gestión entre las que destaca la **gestión por excepción**: solo molestas al ejecutivo cuando aparece un riesgo o una oportunidad que te saca del tiempo o del presupuesto; el mismo principio fluye hacia arriba (los jefes de equipo no molestan al jefe de proyecto si no hay riesgo, oportunidad o desviación significativa). Implicación: **PRINCE2 funciona sobre confianza + autonomía** — exactamente las dos condiciones de **3.3**; PRINCE2 las institucionaliza como filosofía explícita.

**Lo que PRINCE2 no captura**: en la práctica te das cuenta de que, una vez establecido el proyecto, **no entras en mantenimiento puntual — estás en transformación continua**. La visión PRINCE2 es **necesaria pero no suficiente**: sirve para describir cada paso, pero no captura que no hay un proyecto único con principio y fin, sino una **secuencia continua de re-transformaciones** del propio sistema.

**Caso vivido — Disputas (W2M)**: el cliente pidió una aplicación para gestionar disputas; entrega prevista en junio. El proyecto pasó por **muchos estadios de madurez** que cambiaron cómo se gestionaba en cada momento. Modelo inicial: **evolutivo**, entregas incrementales por hitos para que el cliente las usara progresivamente. Giro: la usuaria del cliente **rechazó** ese modelo — casi pierden el proyecto. Reorientación: entregar todo pero como **MVP** para que viera el conjunto; después un segundo MVP, un tercero, refinándose. Cierre del giro: la usuaria finalmente aceptó → ahora se trabaja sobre la versión definitiva. **Conclusión**: la naturaleza del proyecto cambió por completo a mitad de proyecto. Eso es lo que PRINCE2 no captura.

### 5.4.4. Diversidad de visiones del equipo

Resumen: A todo lo anterior se suma que cada miembro tiene una **visión distinta** de cómo deberían hacerse las cosas — porque vienen de **sustratos profesionales muy distintos** (lo que ya enuncia el Punto 2). Reparto real del equipo actual: el humano (~20 años de carrera, perfil senior multi-rol); **Michelle** (6 años de experiencia entre Indra + Plexus, sin estudios de ingeniería informática); nuevos ingenieros y grado superior (incorporaciones recientes con nivel de implicación equivalente entre sí); entradas más recientes (chicos con cursos de tecnología de **100 horas**, a los que hay que encajar en el flujo del equipo). Conecta directamente con **2.2** (150h Java vs senior dilatado): la gestión de un mismo proyecto sobre un equipo con sustratos tan distintos es una de las razones por las que el marco PRINCE2 + intranet, aun bien diseñado, "no funciona del todo".

### 5.4.5. Por qué SharePoint falla — el sustrato cognitivo

Resumen: Aunque tengas un marco común perfectamente estructurado y publicado en SharePoint, **la gente se pierde**. Y se pierde **no porque la información no esté** — está. Se pierde porque **no tiene la visión cognitiva para descodificarla**: no tiene la visión de la **relación con el cliente**, no tiene la visión de la **gestión del proyecto**, no tiene la visión del **proceso de ingeniería** que se lleva a cabo en cada etapa. Resultado en la práctica: la intranet **no se utiliza** como debería; **no se busca la información** aunque esté disponible; **incluso la gente comprometida se pierde**. Enlaza con **2.2, 3.6 y 3.8.1**: la herramienta no salva al sustrato.

### 5.4.6. Cierre — el dilema estructural y su generalización

Resumen: Síntesis del Punto 5 antes de pasar a 5.5/5.6, y bisagra explícita al Punto 6.

**El dilema**: si **aplico estructura** → parte del equipo la entiende y la usa, **otra parte se pierde** (la que no tiene el sustrato cognitivo); si **no aplico estructura** → todo se convierte en **"vete tú a saber"** — modelo Inditex de favoritos personales, conocimiento atrapado en cabezas. **No es un problema de elegir bien la estructura — es estructural**: cualquier opción binaria deja la mitad del equipo fuera.

**Generalización a los tres niveles de gestión**: el mismo dilema aparece en gestión de equipos (**3.6 — Nivel 1**), gestión de proyectos (**3.7 — Nivel 2**) y gestión de grandes corporaciones (**3.8 — Nivel 3**). En cada escala hay quien tiene el sustrato cognitivo para descodificar el marco y quien no; en cada escala el "vete tú a saber" cuesta dinero, tiempo y proyectos.

**Capa adicional — asimilación y auto-responsabilización**: aunque encuentres personas que crees que saben hacer las cosas, en la práctica **nunca tienes garantías**: (1) de que la persona haya **asimilado en su interior** la forma de trabajar (saberla decir vs haberla incorporado); (2) de que, una vez asimilada, **se responsabilice de mantener y mejorar** su parte cuando el sistema cambie. **Tres gaps acumulativos**: conocimiento, asimilación, auto-responsabilización. Cualquiera que falle → la estructura se queda colgada. Refuerza la tesis de "**avatar autoconsciente que opera sobre sí mismo**" del Punto 6.

**Tesis síntesis — la velocidad como fondo**: por mucho que tratemos de racionalizar cómo trabajar, el mundo de la informática **va tan rápido** que, aunque idealmente encontraras gente con el nivel adecuado para hacer funcionar el mejor sistema posible, **en cuestión de seis meses estaría todo desfasado**. No basta con resolver el dilema cognitivo de hoy: la velocidad del cambio convierte cualquier solución estable en obsoleta antes de consolidarse. Aunque encajases hoy a personas, marco, herramientas y procesos en armonía perfecta, esa armonía caduca. Y entonces aparece la pregunta que abre el Punto 6: **¿cómo luchas contra esto?** La respuesta concreta del equipo es el aparato SCAAMN — un sistema diseñado precisamente para **no quedarse desfasado** porque es **autoconsciente y evolutivo**.

## 5.5. Estado actual de los agentes

Resumen: Plano paralelo al dilema cognitivo de 5.4 — qué pueden hacer hoy los agentes IA (Claude Code, en concreto), qué requisitos implícitos llevan, y cuándo realmente rinden bien. Mantiene bisagras visibles con 5.4 (el sustrato cognitivo del operador del agente es el mismo dilema, en otra capa) sin fundirse del todo: la fusión completa es lo que justifica el Punto 6.

### 5.5.1. Capacidad bruta del agente actual

Resumen: Los agentes tienen ahora la capacidad de **tirar mucho trabajo hacia adelante**. Dos accesos clave: **acceso al proyecto al completo** (abres Claude Code dentro del proyecto y automáticamente tiene acceso a todo); **acceso al ordenador** (como Claude Code está metido dentro del ordenador, puede interactuar con el ordenador entero — escribir, leer ficheros, subir a GitHub, abrir tickets en Jira, lo que necesites). Resultado: **capacidad de aceleración brutal** — vas hablando con él y él va trabajando.

### 5.5.2. El requisito implícito — buenas prácticas + especialización

Resumen: Solo aprovechas esa capacidad con **infraestructura seria**. Piezas imprescindibles: **Git** (sistema de versiones) sí o sí — si el agente trabaja y no te gusta el resultado, **marcha atrás**; sin control de versiones, cada experimento del agente es irreversible. **Git worktrees / árboles de Git** — para que **varios agentes trabajen en paralelo**, cada uno en su propia rama, integrándose cuando terminan; sin esto, paralelismo de agentes = colisiones constantes.

Pero las herramientas solo dan ventaja real si **el humano que pilota al agente sabe lo que está pidiendo**. Si no: le dices al agente "hazlo" y no tienes manera de verificar que lo hace bien; cuando falla, no sabes ni por qué ni cómo deshacerlo; puedes **romper cosas** — y nos ha pasado.

**Caso vivido reciente**: un compañero hizo una batería de tests en una rama. No se quería traer entera a la principal, pero tampoco se podía hacer un merge directo (incompatibilidades). Solución: **cherry-pick** del commit concreto que tenía las novedades, ignorando el resto, **reescribiendo la historia de Git por debajo**. Esto no lo sabe hacer cualquiera. Un agente que ejecute "merge esto" sin entender el problema lo rompe seguro. Por eso la pareja **agente + humano-no-especialista** es el peor escenario: la velocidad del agente convierte en irreversibles errores que un humano lento habría detectado a tiempo.

**Bisagra con el dilema cognitivo (5.4)**: el sustrato cognitivo no solo aplica a la persona que usa SharePoint — aplica también a la persona que opera el agente. Mismo dilema, otra capa.

### 5.5.3. Cuándo Claude funciona bien — tareas acotadas + ingeniero competente

Resumen: Claude rinde para **tareas acotadas** cuando tú, como ingeniero, sabes lo que estás haciendo. La mejora se nota especialmente en dos planos.

**Plano 1 — la fricción administrativa de plataforma desaparece**: el mundo Java arrastra mucho **trabajo administrativo no productivo** — instalar Maven, instalar el JDK, configurar Docker, levantar contenedores, preparar bases de datos, configuración fina del entorno. Hasta que algo funcionaba: *fallo, fallo, fallo* — pero **fallos de configuración, no de lógica**. Comparativa: en Microsoft/C# este problema es menor — el framework es más cerrado y opinado, te dice cómo hacer las cosas; en Java toca montar y adaptar todo el entorno cada vez. Con Claude Code: cuando le pides algo, **él mismo detecta esos fallos administrativos**, los diagnostica y te los corrige; si es algo más fino ("no encuentro Java", "no encuentro Maven"), te pregunta qué quieres que haga.

**Plano 2 — Claude como "pequeño arquitecto" + profesor**: Claude no es solo un ejecutor — es un **pequeño arquitecto** comparable a un IDE Ultimate (referencia: IntelliJ IDEA Ultimate). Diferencia respecto a un IDE tradicional: Claude tiene **mucho conocimiento accesible por su propia naturaleza** (es un LLM). Consecuencia: a veces no solo resuelve un problema que tenías — **descubre un problema que ni sabías que tenías**, te da la solución y te la **explica**. Sirve para resolver y para **aprender rápido al mismo tiempo**.

**Pero — vuelve al dilema**: todo este valor solo se realiza si tú **sabes lo que estás haciendo**. Sin sustrato técnico, ese mismo Claude se convierte en una **caja negra que escupe soluciones que no puedes verificar** — exactamente el riesgo que se describió con Git/cherry-pick. La conexión con 5.4 es directa: el dilema cognitivo de la intranet **se replica en silicio** cuando el operador del agente carece del sustrato.

## 5.6. Palancas concretas de aplicación de IA

Resumen: [PLACEHOLDER] Pendiente de rellenar. Aquí se describirán los casos de uso concretos, metodología y herramientas IA específicas que el equipo va a aplicar sobre el estado de partida (5.1 + 5.2 + 5.3), asumiendo el dilema estructural identificado en 5.4 y las capacidades/limitaciones reales de los agentes descritas en 5.5, para resolver los problemas de coordinación del Punto 3. La respuesta sintética del equipo a la fusión de los dos dilemas (cognitivo humano + dilema del operador del agente) es el aparato SCAAMN del Punto 6.

```avatar-lang
@id: doc-05-como-aplicarlo
state BORRADOR "En elaboración"
state PUBLICADO terminal "Publicado en avatar-mind"
action publicar: BORRADOR -> PUBLICADO {
  title: "publicar"
  description: "Documento registrado en avatar-mind"
  requires: BORRADOR
  produces: PUBLICADO
}
```
