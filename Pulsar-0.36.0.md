## Lo más destacado

- **Agentes que arrancan más ligeros.** Los agentes Claude que abre Pulsar empiezan **sin cargar los conectores de claude.ai ni Artifact**, que ocupaban casi la mitad de cada petición: pasan de unos 64k a unos 37k tokens. Si el agente necesita Gmail, Vercel u otro conector, **lo enciende él solo** y el panel se reanuda en unos segundos con la conversación intacta, sin volver a iniciar sesión. Se apaga en **Ajustes › Agentes › Arranque ligero**.
- **Relevo cuando el contexto crece.** Cuando una conversación pasa de 300k tokens (o del 70 % de la ventana del modelo), Pulsar **releva al agente por uno nuevo en el mismo panel**: el viejo escribe un traspaso con lo decidido y lo pendiente, se hiberna, y el nuevo sigue con el mismo modo de permisos o uno más estricto. Cada turno sale mucho más barato y el agente no pierde el hilo. Te pregunta una sola vez; también puedes **Relevar ahora** desde el menú del panel.
- **Mensajes entre agentes que siempre llegan.** Los mensajes entre agentes ya no se pierden ni se quedan a medias en la caja: esperan en un buzón hasta que el destino puede recibirlos, van siempre firmados y el orquestador recibe copia de lo que se habla con sus tareas sin que le interrumpa. `pulsar agent who` marca a tu orquestador, al coordinador y a las tareas hermanas.

## Mejoras

- _Agentes_ · El traspaso del relevo enseña qué permisos no pasan al agente nuevo (los «siempre» de Bash sí siguen valiendo) y tus respuestas anteriores como historial, nunca como permiso.
- _Agentes_ · Un modo de permisos fijado en un panel, también desde el iPhone, ya no supera lo que digan los Ajustes de la Mac.

## Arreglos

- _Agentes_ · Tras reiniciar Pulsar, un mensaje a un agente de un workspace que aún no abriste ya no falla: su terminal arranca en segundo plano y el mensaje le llega en cuanto puede recibirlo.

---

## Highlights

- **Agents that start lighter.** Claude agents opened by Pulsar start **without loading the claude.ai connectors or Artifact**, which took almost half of every request: from about 64k down to about 37k tokens. If the agent needs Gmail, Vercel or another connector, **it turns them on by itself** and the pane resumes in a few seconds with the conversation intact, without signing in again. Turn it off in **Settings › Agents › Light startup**.
- **Handoff when the context grows.** When a conversation passes 300k tokens (or 70% of the model's window), Pulsar **hands the agent off to a fresh one in the same pane**: the old one writes a handoff with what was decided and what's pending, goes to sleep, and the new one continues with the same permission mode or a stricter one. Each turn gets much cheaper and the agent keeps the thread. It asks you only once; you can also **Hand off now** from the pane menu.
- **Messages between agents that always arrive.** Messages between agents no longer get lost or stuck half-typed in the input box: they wait in a mailbox until the recipient can take them, they are always signed, and the orchestrator gets a copy of what is said to its tasks without being interrupted. `pulsar agent who` marks your orchestrator, the coordinator and sibling tasks.

## Improvements

- _Agents_ · The handoff shows which permissions don't carry over to the new agent (Bash “always” rules still apply) and your earlier answers as history, never as permission.
- _Agents_ · A permission mode set on a pane, including from the iPhone, no longer goes beyond what the Mac's Settings allow.

## Fixes

- _Agents_ · After restarting Pulsar, a message to an agent in a workspace you haven't opened yet no longer fails: its terminal starts in the background and the message reaches it as soon as it can take it.
