## Lo más destacado

- **Historial de tus agentes en Recursos.** Pulsar guarda en tu Mac, sin subir nada, cuánto gasta cada agente y cómo van las compilaciones. En **Recursos › Historial** verás el gasto por día y por papel, cuánto esperan y fallan los turnos de `pulsar lock`, y qué ayudantes crecen demasiado de contexto o se paran sin reportar. Los agentes lo consultan con `pulsar metrics`.
- **Los orquestadores ya no pierden de vista a sus ayudantes.** Cada reporte o pregunta de un ayudante le llega a su orquestador en el momento, también si ocurre entre dos vigilancias o tras reiniciar Pulsar. Las preguntas de trabajo de un ayudante las responde su orquestador: a ti solo te llega lo que él no puede decidir. Un ayudante que recibe un mensaje nuevo o que se está relevando ya no aparece como «parado sin reportar».

## Mejoras

- _Agentes_ · Al cerrar un sub-orquestador, sus ayudantes pasan al agente que lo lanzó en vez de quedarse huérfanos, y «Limpiar» no cierra tareas con un reporte sin leer (salvo con `--force`).
- _Seguridad_ · Cuando un orquestador responde una pregunta de su ayudante, la respuesta dice que fue él y no tú, y nunca responde por un ayudante que va sin permisos.
- _Seguridad_ · Tras reiniciar, un mensaje entre workspaces que habías confirmado y aún no se había entregado te pide confirmarlo otra vez.
- _Agentes_ · Los recibos de comprobaciones ya no salen «parciales» por hacer un commit mientras corren, y dicen qué archivos cambiaron.

## Arreglos

- _Agentes_ · Un mensaje a un agente con texto sin enviar en su caja ya no se queda pegado ni se reenvía en bucle: va por el buzón y **tu borrador nunca se envía ni se pierde**.
- _Agentes_ · El relevo por contexto ya no se cancela si llega un mensaje justo después del traspaso (lo recibe el agente nuevo) y se reintenta solo si algo lo frena al acabar el turno.
- _Agentes_ · Los reportes de los ayudantes y los mensajes pendientes sobreviven a un reinicio de Pulsar.
- _Agentes_ · Codex en su sandbox explica que no puede hablar con Pulsar en vez de decir que Pulsar está cerrado, y `pulsar lock` avisa cuando corre sin turno.

---

## Highlights

- **Your agents' history in Resources.** Pulsar keeps on your Mac, without uploading anything, how much each agent spends and how builds are going. In **Resources › History** you'll see spend per day and per role, how long `pulsar lock` turns wait and how often they fail, and which helpers grow too much context or stop without reporting. Agents can query it with `pulsar metrics`.
- **Orchestrators no longer lose track of their helpers.** Every report or question from a helper reaches its orchestrator right away, even between two watches or after restarting Pulsar. A helper's work questions are answered by its orchestrator: only what it can't decide reaches you. A helper that gets a new message or is handing over no longer shows up as «stopped without reporting».

## Improvements

- _Agents_ · Closing a sub-orchestrator hands its helpers to the agent that launched it instead of orphaning them, and «Clean up» no longer closes tasks with an unread report (unless `--force`).
- _Security_ · When an orchestrator answers its helper's question, the answer says it came from the orchestrator and not you, and it never answers for a helper running without permissions.
- _Security_ · After a restart, a cross-workspace message you had confirmed but that wasn't delivered yet asks you to confirm it again.
- _Agents_ · Check receipts no longer come out «partial» because of a commit made while they run, and they say which files changed.

## Fixes

- _Agents_ · A message to an agent with unsent text in its box no longer gets stuck or resent in a loop: it goes through the mailbox and **your draft is never sent or lost**.
- _Agents_ · Context handover is no longer cancelled when a message arrives right after the handoff (the new agent gets it), and it retries on its own if something holds it up at the end of the turn.
- _Agents_ · Helper reports and pending messages survive a Pulsar restart.
- _Agents_ · Codex in its sandbox explains it can't talk to Pulsar instead of saying Pulsar is closed, and `pulsar lock` warns when it runs without a turn.
