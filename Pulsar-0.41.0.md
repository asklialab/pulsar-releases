## Lo más destacado

- **Sabes cuándo un agente te necesita.** **«Te espera» solo cuando de verdad te pide algo**: los avisos de Claude que no son preguntas ya no lo marcan, y si se queda marcado sin nada en pantalla se corrige solo. Si un agente pregunta en texto, se le pide hacerlo con el selector; y si el modo automático le deniega algo, te avisa.
- **Orquestadores sin vigilar.** Lo que hacen sus ayudantes (reportó, pregunta, se paró) **le llega al orquestador por el buzón**: lo despierta solo cuando hay algo y, si está trabajando, le llega con su siguiente paso. Sin vigilantes que caducan ni «Esperando» de más, y gastando menos.

## Nuevo

- _Avisos y sonidos_ · Cuando el **modo automático deniega** algo a un agente (por ejemplo, publicar), te avisa en la campana con qué y por qué.
- _Agentes_ · Las novedades de los ayudantes **llegan solas al orquestador por el buzón**: ya no hace falta `watch` ni `Monitor`, que caducaban y despertaban sin nada. `watch` queda para quien quiera esperar a propósito (hasta 1 h, y avisa si recorta).

## Mejoras

- _Agentes_ · Si un agente acaba su turno con una **pregunta escrita en texto**, se le pide hacerla con el selector (un ayudante, en su reporte). Si insiste, su panel queda en «te espera» con la pregunta y, si es un ayudante, su orquestador se entera.
- _Agentes_ · `pulsar agent who` encuentra un agente por su id, y los errores con el id de otro orquestador dicen de quién es.

## Arreglos

- _Agentes_ · Un agente ya no se queda en **«te espera»** por avisos de Claude que no piden nada (inactividad, inicio de sesión, avisos de plugins…). Si aun así se queda marcado sin ninguna pregunta en pantalla, Pulsar lo corrige solo y sus mensajes ya no se quedan retenidos.
- _Agentes_ · Esperar a sus ayudantes, `sleep` o `caffeinate` ya no dejan a un agente en **«Esperando»**: cuando acaba de verdad, te avisa.
- _Agentes_ · Sin avisos falsos de **«se paró sin reportar»**: tras un aviso con `pulsar agent send --fyi` no hay nada que hacer, y una parada tras un encargo trae su último texto para ver si solo contestó.
- _Agentes_ · El **relevo por contexto** ya no se pierde: no le llegan mensajes en el turno del traspaso, esperar a los ayudantes o un despertador de Claude no lo bloquean, se vigila desde el primer turno y la pausa tras un relevo ya no apaga el tope.
- _Paneles_ · Los controles de la cabecera de cada agente ya no se quedan a media barra: van siempre junto a su estado, a la derecha.
- _Paneles_ · Las etiquetas flotantes (como la de un mensaje «en cola») ya no se cortan en el panel pegado al borde derecho: salen hacia donde caben.

---

## Highlights

- **You know when an agent needs you.** **“Waiting for you” only when it really asks you something**: Claude notices that aren't questions no longer set it, and if it gets stuck with nothing on screen it clears itself. If an agent asks in plain text, it's asked to use the picker; and if auto mode denies it something, you're told.
- **Orchestrators without polling.** What their helpers do (reported, asks, stopped) **reaches the orchestrator through its mailbox**: it's woken only when there's something and, if it's working, it arrives with its next step. No watchers that expire or extra “Waiting”, and it spends less.

## New

- _Alerts & sounds_ · When **auto mode denies** an agent something (for example, publishing), the bell tells you what and why.
- _Agents_ · Helper news **reaches the orchestrator by itself through its mailbox**: `watch` and `Monitor`, which expired and woke it for nothing, are no longer needed. `watch` stays for anyone who wants to wait on purpose (up to 1 h, and it says if it trims).

## Improvements

- _Agents_ · If an agent ends its turn with a **question written as plain text**, it's asked to use the picker (a helper, in its report). If it insists, its pane shows “waiting for you” with the question and, if it's a helper, its orchestrator is told.
- _Agents_ · `pulsar agent who` finds an agent by its id, and errors with another orchestrator's id say whose it is.

## Fixes

- _Agents_ · An agent no longer gets stuck on **“waiting for you”** because of Claude notices that ask for nothing (idle, sign-in, plugin notices…). If it still ends up marked with no question on screen, Pulsar clears it by itself and its messages are no longer held back.
- _Agents_ · Waiting for its helpers, `sleep` or `caffeinate` no longer leave an agent on **“Waiting”**: when it really finishes, you're told.
- _Agents_ · No more false **“stopped without reporting”**: after a notice sent with `pulsar agent send --fyi` there's nothing to do, and a stop after a new request includes its last text so you can see whether it just replied.
- _Agents_ · **Context handoff** is no longer lost: no messages arrive in the handoff turn, waiting for helpers or a Claude wake-up don't block it, it's watched from the first turn and the pause after a handoff no longer turns off the ceiling.
- _Panes_ · The controls in each agent's header no longer drift to the middle of the bar: they always sit next to its status, on the right.
- _Panes_ · Floating labels (like a “queued” message's) are no longer cut off in the pane against the right edge: they open toward where they fit.
