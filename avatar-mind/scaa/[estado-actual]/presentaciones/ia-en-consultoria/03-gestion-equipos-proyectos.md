# 3. Lo verdaderamente difícil de la consultoría: gestión de equipos y proyectos

Resumen: **[TENTATIVO — el humano duda si dejarlo o quitarlo, decisión pendiente]** Tesis sobre el oficio en sí (independiente de IA, pero recontextualiza el papel que la IA puede jugar): en consultoría lo verdaderamente difícil no es lo técnico — es la gestión de equipos y proyectos. Ahí se consume gran parte del trabajo. Cualquier discusión sobre productividad, IA o herramientas que ignore esta capa está dejando fuera el factor que más peso tiene en el resultado real. Por eso se introduce antes de los retos (4) y la propuesta de aplicación (5).

## 3.1. Síntomas habituales

Resumen: Manifestaciones cotidianas de la dificultad. **Alto número de reuniones constantes** para saber qué pasa en cada momento. **Carga ceremonial Scrum**: dailies, retrospectivas, plannings, refinements — aplicarlo bien tiene coste real. **Caso Inditex**: Scrum bien marcado, ceremonia completa, y aun así la dinámica real del equipo manda sobre la filosofía Scrum. Por mucha herramienta y estructura que tengas, si el equipo es disfuncional la metodología no salva nada.

## 3.2. Disfunciones típicas que rompen la auto-gestión

Resumen: Patrones que vacían la promesa Scrum del "equipo que se gestiona solo". **Líder técnico** que acaba cargando con todo. **Developer senior** que va a su manera y no sigue las directrices del equipo. **Juniors** sin claridad sobre por dónde va el asunto. **Reparto desequilibrado**: una persona carga con todo y luego delega a dos o tres. **Inversión de roles**: el Product Owner delega en el líder técnico, o el técnico se pone por encima del PO. **Developers excesivamente dependientes** del líder técnico — cuello de botella inmediato.

## 3.3. Las dos condiciones para que un equipo funcione

Resumen: **Confianza** (la gente tiene que confiar unos en otros) y **autonomía** (la gente tiene que ir cogiendo autonomía progresivamente). Con esas dos cosas se construye **unidad de equipo**: cada miembro puede trabajar en distintas cosas en paralelo, sin la jerarquía bloqueante del "hasta que X no haga Y, yo no puedo hacer Z".

## 3.4. Lo que NO es un equipo sano

Resumen: Un **waterfall encubierto** — análisis funcional → diseño técnico → construcción → pruebas, con una persona fija en cada fase. Eso no es Scrum aunque tenga ceremonias. Los equipos sanos funcionan precisamente cuando esa secuencia rígida se rompe: varias personas trabajan en distintas tareas dentro del equipo sin que cada tarea tenga preasignada una persona concreta.

## 3.5. Roles necesarios (sin que ninguno sea cuello de botella)

Resumen: **Product Owner** (mantiene la relación con el cliente); **Líder Técnico** (marca las directrices técnicas); **Developers** (construyen). Los roles existen, pero la salud del equipo se mide en si pueden colaborar en paralelo o si todo el flujo depende secuencialmente del que está justo "encima".

## 3.6. Dos visiones sobre cómo se gestiona un proyecto de ingeniería

Resumen: **[TENTATIVO — hereda del Punto 3]** Raíz estructural de buena parte de la fricción descrita en 3.1/3.2: en gestión de proyectos de ingeniería conviven dos visiones radicalmente distintas según el perfil formativo de quien gestiona. **Conecta con el Punto 2** (mismo IA, distinto efecto según sustrato): cada visión usa la IA como palanca diferente.

**Visión A — quien NO ha estudiado ingeniería**: gestiona como ha visto gestionar en los grandes clientes por los que ha pasado. No tiene conocimiento teórico del *por qué*, tiene conocimiento por exposición. Consecuencia: el cliente concreto en el que aprendió tiene mucho **peso emocional** y se convierte en su modelo mental de "cómo se hacen los proyectos"; cuesta salir de ahí, y cuando se le intenta explicar el fundamento tiende a volver a lo conocido.

**Visión B — quien SÍ ha estudiado ingeniería del software**: conoce los modelos formales y el *por qué* de cada uno. Reducidos a dos familias: **Waterfall** (fases secuenciales rígidas) y **modelos evolutivos** (iterativos, ágiles, incrementales). Conoce además la **cadena completa** del oficio: (1) toma de requisitos con el cliente; (2) análisis funcional — a nivel negocio (cómo funciona realmente el cliente) y a nivel técnico (cómo se pasa ese negocio a sistema); (3) construcción; (4) pruebas — TDD como práctica de partida, distintos niveles (unitarias, integración, sistema, aceptación) y paso por distintos entornos (dev, pre, pro).

**Por qué importa**: la fricción Visión A vs Visión B es uno de los obstáculos reales de la gestión en consultoría — y enlaza con el Punto 2: una persona con Visión A usará la IA para **reproducir más rápido** lo que ya hacía; una persona con Visión B la usará para **acelerar y validar pasos concretos** del modelo formal. No es la misma palanca. Conecta también con 3.4 (waterfall encubierto): la Visión A explica por qué surge sin que nadie lo declare como tal.

## 3.7. Dos niveles distintos de "gestión": proceso de ingeniería vs gestión de proyecto

Resumen: **[TENTATIVO — hereda del Punto 3]** Continuación natural de 3.6: aunque hayas estudiado modelos de gestión (waterfall, evolutivos), eso es solo el **nivel del proceso de ingeniería** — cómo pasar de una idea del cliente a producción dentro de un sprint o ciclo de entrega. Por encima hay otro nivel que conviene no mezclar: la **gestión de proyecto**, orientada a OKRs empresariales.

**Nivel 1 — proceso de ingeniería** (lo que cubre 3.6): el modelo que sigues *dentro* de un sprint o ciclo. Waterfall típico está orientado aquí; los modelos evolutivos aparecen como alternativa en este mismo nivel.

**Nivel 2 — gestión de proyecto** (un nivel por encima): aquí no se habla de código ni de sprints, sino de **objetivos empresariales**. Consiste en (1) identificar un **OKR empresarial** que se quiere resolver; (2) establecer un **proyecto** con una serie de **hitos** que llevan a resolver ese OKR; (3) cada hito produce a su vez **múltiples versiones** del producto/sistema. Es la capa que da sentido al trabajo de ingeniería que hay debajo: sin ella los sprints no tienen dirección empresarial; con ella, cada sprint contribuye a un hito que contribuye a un OKR.

**Por qué importa para la presentación**: muchas veces se mezclan los dos niveles al discutir "cómo se gestiona la consultoría". La IA tiene impacto distinto en cada uno: en el **nivel de proceso de ingeniería** acelera construcción, pruebas e integración (lo visto en fases 2–4 del Punto 1); en el **nivel de gestión de proyecto** su rol está mucho menos asentado (sintetizar estados, anticipar riesgos, conectar OKRs con hitos…), pero el ciclo *OKR → hitos → versiones* sigue siendo decisión humana. Distinguir los dos niveles evita prometer impactos del nivel equivocado.

## 3.8. Nivel 3: estrategia empresarial, portfolio y trenes de release

Resumen: **[TENTATIVO — hereda del Punto 3]** Tercer escalón sobre 3.6 (proceso de ingeniería) y 3.7 (gestión de proyecto). En empresas grandes este nivel domina la realidad operativa: la **estrategia empresarial multi-departamento**. Es el plano que más fricción produce y el que tiene **menos rodaje con IA**.

**Caso conocido por el humano — BBVA (y por extensión Banco Santander)**: en compañías muy grandes (BBVA en primera persona) la estrategia empresarial abarca **muchos departamentos** trabajando sobre un **portfolio común** que se divide a su vez en **muchos proyectos**.

**Implicación operativa — trenes de release**: como muchos proyectos deben coordinarse entre sí para que la estrategia avance, hace falta interconectar equipos y departamentos. De ahí nacen los **"trenes de release"**: cadenas coordinadas de releases desde la idea inicial hasta la puesta en producción, sincronizando equipos que de otra forma no podrían entregar a la vez.

**Por qué importa para la presentación**: gestionar esto **a nivel de compañía** es muy complicado y queda fuera del alcance práctico de los Niveles 1 y 2. La IA tiene rodaje muy desigual en los tres planos: **Nivel 1** — acelera código, pruebas e integración (fases 2–4 del Punto 1), territorio bien explorado; **Nivel 2** — empieza a aportar valor en síntesis, anticipación de riesgos, conexión OKR↔hito, territorio en exploración; **Nivel 3** — todavía marginal, porque la coordinación estratégica multi-departamento sigue siendo trabajo humano (negociaciones políticas, compromisos cross-departamentales, límites de información confidencial entre divisiones). Distinguir los tres niveles permite no prometer impactos de IA en planos donde la IA aún no llega.

### 3.8.1. Por qué el Nivel 3 es especialmente difícil: el marco común se rompe en quien lo gestiona

Resumen: **[TENTATIVO — hereda del Punto 3]** Profundización del "por qué" abierto en 3.8. **Tesis**: aunque la empresa establezca un **marco común de trabajo** que en teoría coordina los departamentos del portfolio, en la práctica el marco solo funciona si quien lo gestiona **lo entiende y lo defiende** — y ahí es donde se rompe.

**Dos perfiles típicos que rompen el marco común**: (1) **Programadores escalados a gestión sin formación en ingeniería** — saben programar pero no entienden el *por qué* del marco; lo aplican de forma mecánica o lo ignoran cuando choca con su intuición. Conecta directamente con la **Visión A de 3.6** (gestionan como vieron gestionar donde estuvieron, sin teoría detrás). (2) **Managers que solo saben de gestión** — conocen las herramientas de proceso (planificación, reporting, gestión de equipo) pero no entienden lo que hay por debajo técnicamente; no pueden juzgar si un *trade-off* técnico es razonable ni traducir compromisos técnicos en hitos creíbles para el portfolio.

**Consecuencia**: en ambos casos el marco común **queda fuera de las políticas reales** con las que cada manager gestiona su parcela. Cada uno opera con su propia lógica → la coordinación cross-departamento se rompe, los release trains pierden la sincronía que los justifica, el portfolio empieza a divergir de la estrategia empresarial que pretende ejecutar.

**Conexión con el resto**: refuerza **Visión A vs Visión B (3.6)** — lo que allí era problema formativo a nivel equipo, escala a problema estructural a nivel empresa; refuerza el **Punto 2 (perfiles)** — si la IA cae sobre sustratos profesionales distintos, en gestión ese efecto se multiplica porque el "sustrato profesional del manager" decide si el marco se sostiene; y explica por qué la promesa "la IA va a resolver la coordinación estratégica" es prematura: lo que falla en el Nivel 3 no es procesamiento de información — es el **sustrato cognitivo de quien gestiona**.

---

> **Cierre del Punto 3 — el problema está atacado**: los problemas de gestión enumerados en 3.1–3.8.1 no se quedan en diagnóstico. Hay casi **dos años de trabajo continuado** del equipo del humano en World2Meet dedicados específicamente a resolverlos, cuyo resultado es el aparato SCAAMN del Punto 6. Ver **6.1 (Génesis: dos años de trabajo en W2M)** para el contexto histórico y la tesis derivada (W2M es escenario perfecto porque su complejidad está concentrada en flujo de información, no en cadena física).
