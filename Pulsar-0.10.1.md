## Lo más destacado

- **Las preguntas de Codex, también en el iPhone.** Cuando Codex te pregunta con opciones mientras sigue trabajando, la pregunta llega al iPhone con sus botones: en la **isla**, en el aviso y en la vista del agente. Puedes elegir una opción o escribir o dictar otra respuesta. Antes de pulsar nada en su terminal, Pulsar comprueba que se ve esa pregunta con esas opciones; si algo no cuadra, no envía nada.

## Mejoras

- _Agentes_ · `pulsar agent` solo actúa en nombre de un panel si quien lo ejecuta es de verdad un proceso de ese panel: nadie más puede dejar un reporte falso en nombre de una tarea.

## Arreglos

- _Agentes_ · Al cerrar un agente con una pregunta pendiente, la pregunta desaparece también de la **isla del iPhone**, en vez de quedarse hasta abrir la app.
- _Agentes_ · Tras responder desde la isla, el agente vuelve a «trabajando» al momento y la isla se pone al día en un segundo, sin pasar por «Alguien te espera».
- _Agentes_ · Un Codex lanzado con `pulsar agent spawn --agent codex` ya puede usar `pulsar agent report`, `pulsar browser` y `pulsar share` aunque tu `~/.codex/config.toml` le limite el entorno (`shell_environment_policy`).

---

## Highlights

- **Codex’s questions, on your iPhone too.** When Codex asks you a question with options while it keeps working, the question reaches your iPhone with its buttons: in the **island**, in the notification and in the agent view. You can pick an option or type or dictate another answer. Before pressing anything in its terminal, Pulsar checks that this question and these options are on screen; if something doesn’t match, it sends nothing.

## Improvements

- _Agents_ · `pulsar agent` only acts on behalf of a pane if whoever runs it really is a process of that pane: nobody else can leave a fake report on behalf of a task.

## Fixes

- _Agents_ · Closing an agent with a pending question also removes it from the **iPhone island**, instead of leaving it there until you open the app.
- _Agents_ · After you answer from the island, the agent goes back to “working” right away and the island catches up within a second, without showing “Someone is waiting for you”.
- _Agents_ · A Codex launched with `pulsar agent spawn --agent codex` can now use `pulsar agent report`, `pulsar browser` and `pulsar share` even if your `~/.codex/config.toml` limits its environment (`shell_environment_policy`).
