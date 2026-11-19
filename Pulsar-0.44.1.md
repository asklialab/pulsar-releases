## Mejoras

- _Barra lateral_ · La fila **Límites** ya lee a **Claude** sin configurar nada: Pulsar se lo pregunta a la propia CLI de Claude y enseña la semana del plan, la del modelo con ventana propia, las cinco horas si el plan las tiene y el tipo de plan. La fila del pie muestra la ventana que menos margen deja.
- _Agentes_ · Las preguntas de una tarea llegan a su orquestador con la **descripción de cada opción** y una sola línea por espera. El despertar del buzón ya no llama «mensaje de otro agente» a un aviso de Pulsar.

## Arreglos

- _Agentes_ · Un agente de Claude cuyo turno acaba por un **error del proveedor** ya no se queda «trabajando» durante horas: el panel termina con el error, suena y avisa a su orquestador.
- _Agentes_ · Un mensaje a una tarea **hibernada tras su relevo** la despierta, en vez de quedarse en su buzón hasta caducar.
- _Agentes_ · Tras reiniciar Pulsar, un orquestador no vuelve a recibir los reportes que ya había leído, y uno intermedio no se da por parado mientras su tarea sigue sin medir.
- _Navegador_ · Para los agentes: `pulsar browser upload` funciona con campos de archivo **ocultos** (los que la página abre desde un botón propio).
- _Rendimiento_ · `pulsar lock` ya no deja un informe de cierre a nombre de la CLI cuando la orden muere por una señal: lo dice y sale con `128 + señal`. `pulsar system status` muestra el **intercambio** y avisa si es alto.
- _Barra lateral_ · El botón de **plegar la barra lateral** vuelve a responder al clic.

---

## Improvements

- _Sidebar_ · The **Limits** row now reads **Claude** with nothing to set up: Pulsar asks Claude's own CLI and shows the plan's week, the week of the model with its own window, the five hours if the plan has them, and the plan type. The footer row shows the window with the least room left.
- _Agents_ · A task's questions reach its orchestrator with **each option's description** and a single line per wait. The mailbox wake-up no longer calls a notice from Pulsar a “message from another agent”.

## Fixes

- _Agents_ · A Claude agent whose turn ends on a **provider error** no longer stays “working” for hours: the pane finishes with the error, plays its sound and tells its orchestrator.
- _Agents_ · A message to a task **hibernated after its handoff** wakes it up, instead of sitting in its mailbox until it expires.
- _Agents_ · After restarting Pulsar, an orchestrator no longer gets reports it had already read again, and an intermediate one isn't taken as stopped while its task is still unmeasured.
- _Browser_ · For agents: `pulsar browser upload` works with **hidden** file inputs (the ones a page opens from its own button).
- _Performance_ · `pulsar lock` no longer leaves a crash report under the CLI's name when the command dies from a signal: it says so and exits with `128 + signal`. `pulsar system status` shows **swap** and warns when it's high.
- _Sidebar_ · The **collapse sidebar** button responds to clicks again.
