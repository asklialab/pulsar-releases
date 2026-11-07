## Lo más destacado

- **Los mensajes entre agentes ya no se atascan.** Cuando un agente escribe a otro con `pulsar agent send`, el mensaje ya no se pega en su caja de texto: espera en un **buzón** de Pulsar y le llega por los hooks de **Claude Code** y **Codex**, tanto si está trabajando como si acaba su turno o está parado (un Claude parado se despierta solo). Se acabaron los mensajes a medio llegar que parecían tuyos, y tu borrador en la caja queda intacto. La confianza de los hooks de Codex solo se da a las sesiones que abre Pulsar: las de fuera no cambian.
- **«Esperando»: un agente con algo en marcha no ha terminado.** Si un agente acaba su turno con subagentes, una compilación u otros ayudantes en marcha, ya no sale «Terminado»: pasa a **Esperando** y dice a qué espera («2 subagentes», «xcodebuild +2»). El aviso de «Terminó» llega **una sola vez**, cuando de verdad acaba. En el iPhone llega con su próxima versión.
- **Voice en reunión: hilo, subtítulos y ⌥ Fn.** La ventana de la reunión se lee **por turnos**, con tus preguntas y las respuestas del agente en el mismo hilo, adjuntos y citas `[mm:ss]`. Plegada, al pasar el ratón por la línea salen **subtítulos**. **Fn** sola dicta siempre y **⌥ Fn** pregunta al agente de la reunión, que ahora ve los workspaces que elijas para esa reunión y tu pantalla. Si alguien te pregunta algo, la línea se pone ámbar y te ofrece «¿Qué respondo?». Lo de cada reunión se guarda en una carpeta fija, `Meetings`.

## Nuevo

- _Dictado_ · La línea de **Pulsar Voice** se mueve con un clic sostenido o arrastrándola: al soltar se queda a la izquierda, abajo o a la derecha de la pantalla.

## Mejoras

- _Avisos y sonidos_ · Las notificaciones enseñan el nombre completo del agente, sin cortarlo a mitad.
- _Agentes_ · Si el agente al que escribes ya salió de su CLI, Pulsar deja de intentarlo en vez de reintentar sin fin.

---

## Highlights

- **Messages between agents no longer get stuck.** When an agent writes to another with `pulsar agent send`, the message is no longer pasted into its text box: it waits in a Pulsar **mailbox** and arrives through the **Claude Code** and **Codex** hooks, whether the agent is working, finishing its turn or idle (an idle Claude wakes up on its own). No more half-delivered messages that looked like yours, and your draft in the box stays untouched. Codex hook trust is only granted to sessions Pulsar opens: the rest don't change.
- **“Waiting”: an agent with something running isn't done.** If an agent ends its turn with subagents, a build or other helpers still running, it no longer shows “Done”: it moves to **Waiting** and says what it is waiting for (“2 subagents”, “xcodebuild +2”). The “Done” alert arrives **only once**, when it really finishes. On iPhone it arrives with its next version.
- **Voice in meetings: thread, captions and ⌥ Fn.** The meeting window reads **by turns**, with your questions and the agent's answers in the same thread, attachments and `[mm:ss]` quotes. Collapsed, hovering the line shows **captions**. **Fn** alone always dictates and **⌥ Fn** asks the meeting agent, which can now see the workspaces you pick for that meeting and your screen. If someone asks you something, the line turns amber and offers “What do I answer?”. Each meeting's files are kept in a fixed `Meetings` folder.

## New

- _Dictation_ · The **Pulsar Voice** line moves with a long click or by dragging it: when you let go it stays on the left, bottom or right of the screen.

## Improvements

- _Alerts & sounds_ · Notifications show the agent's full name instead of cutting it off.
- _Agents_ · If the agent you write to has already left its CLI, Pulsar stops trying instead of retrying forever.
