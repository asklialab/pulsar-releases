## Nuevo

- _Agentes_ · `pulsar metrics messages` muestra cómo se entregan los mensajes entre agentes: por qué vía, cuánto tardan y por qué no llegan. Pulsar guarda cada decisión del buzón para poder diagnosticar.

## Mejoras

- _Agentes_ · Cada mensaje dice quién lo envía y qué relación tiene con quien lo recibe: su orquestador, una de sus tareas, otro agente del espacio u otro espacio. Lo que pide el orquestador llega como encargo, y lo demás, como información. `--fyi` también vale entre agentes del mismo espacio.
- _Agentes_ · Cuando una tarea pregunta algo, su orquestador recibe la pregunta con sus opciones, sin tener que ir a buscarla.
- _Agentes_ · Menos ruido para los agentes: ya no se les despierta para decirles que no hace falta nada, las novedades no repiten líneas y las salidas llevan menos pistas.
- _Agentes_ · En el **modo automático de Claude**, Pulsar le explica al clasificador que los mensajes entre tus agentes son parte de su trabajo. Si aun así bloquea un `send`, un `report` o un `answer`, el orquestador recibe un aviso.

## Arreglos

- _Agentes_ · Los **mensajes a Codex** llegan a la conversación que ves. Antes, un hilo interno de Codex podía quedarse con el mensaje y el agente no lo leía nunca.
- _Agentes_ · Si un mensaje entre agentes no se puede entregar o caduca, quien lo envió recibe un aviso con el motivo, y si conviene volver a enviarlo.
- _Agentes_ · Al detener a **Claude con Esc**, el panel deja de salir como «trabajando» a los pocos segundos. Los mensajes esperan un minuto o hasta lo siguiente que escribas, para no interrumpirte.
- _Agentes_ · Los procesos que usa Pulsar para entregar mensajes ya no cuentan como procesos del agente: el relevo no se queda esperando por «nc» y desaparecen los avisos de «terminó sin reportar y sigue con procesos».
- _Agentes_ · Un mensaje del orquestador despierta a un agente hibernado aunque tenga avisos pendientes. Antes se rechazaba con «inténtalo más tarde».

---

## New

- _Agents_ · `pulsar metrics messages` shows how messages between agents are delivered: which path they took, how long they took, and why they didn’t arrive. Pulsar keeps each mailbox decision so problems can be diagnosed.

## Improvements

- _Agents_ · Each message says who sent it and how they relate to the recipient: its orchestrator, one of its tasks, another agent in the workspace or another workspace. What the orchestrator asks arrives as an assignment, and the rest as information. `--fyi` also works between agents in the same workspace.
- _Agents_ · When a task asks something, its orchestrator gets the question with its options, without having to go look for it.
- _Agents_ · Less noise for agents: they’re no longer woken up just to be told nothing is needed, updates don’t repeat lines, and command output carries fewer hints.
- _Agents_ · In **Claude’s auto mode**, Pulsar explains to the classifier that messages between your agents are part of their work. If it still blocks a `send`, `report` or `answer`, the orchestrator gets a notice.

## Fixes

- _Agents_ · **Messages to Codex** reach the conversation you see. Before, an internal Codex thread could take the message and the agent never read it.
- _Agents_ · If a message between agents can’t be delivered or expires, the sender gets a notice with the reason and whether to send it again.
- _Agents_ · When you stop **Claude with Esc**, the pane stops showing as “working” after a few seconds. Messages wait a minute or until you type something, so they don’t interrupt you.
- _Agents_ · The processes Pulsar uses to deliver messages no longer count as the agent’s own: handoffs no longer wait on “nc”, and the “finished without reporting and still has processes” notices are gone.
- _Agents_ · A message from the orchestrator wakes a hibernated agent even if it has pending notices. Before, it was rejected with “try again later”.
