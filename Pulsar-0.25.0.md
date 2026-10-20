## Lo más destacado

- **Preguntas y estados de Codex más fiables.** Pulsar distingue mejor **cuándo Codex termina, trabaja o necesita una respuesta**. Las preguntas con varias partes mantienen cada respuesta en su lugar, y los agentes que coordinan tareas pueden responder preguntas de sus ayudantes sin concederles permisos de ejecución.
- **Imágenes y documentos con menos carga.** El visor comparte la vigilancia de archivos y limita las lecturas y decodificaciones simultáneas. **Cambiar de documento o cerrar un panel cancela su trabajo pendiente** sin interrumpir otros visores que usan el mismo archivo.

## Nuevo

- _Agentes_ · La firma de los agentes permite consultar **modelos y consumo observados por tarea**, junto con la elección registrada al lanzarla.

## Mejoras

- _Agentes_ · Las tareas pueden declarar su dificultad y riesgo para elegir modelo y esfuerzo según el modo de trabajo del proyecto. Los recibos distinguen las comprobaciones declaradas de la evidencia disponible.
- _Rendimiento_ · La coordinación de compilaciones tiene en cuenta la carga sostenida de CPU de los agentes. Las instrucciones del proyecto se cargan por área para evitar contexto innecesario.

## Arreglos

- _Agentes_ · Los hilos internos de Codex y las notificaciones duplicadas ya no se confunden con la finalización de la tarea visible. Una notificación genérica tampoco se interpreta por sí sola como una petición de permiso.
- _Agentes_ · Las respuestas vuelven a comprobar la pregunta, la sesión y el candado antes de escribir. Se evita mezclar mensajes simultáneos y se avisa si quedó un borrador sin enviar.
- _Agentes_ · Si Codex tarda en registrar una respuesta, Pulsar muestra que está esperando confirmación y evita enviarla dos veces. Las partes todavía pendientes conservan su propia pregunta.
- _Agentes_ · Las esperas y la vigilancia de tareas se cancelan cuando se desconecta quien las pidió. Los cambios de pregunta se anuncian aunque el agente conserve el mismo estado.
- _Agentes_ · Las tareas hibernadas dejan de ocupar cupo activo. Al despertar se comprueba de nuevo la capacidad y se conserva la identidad de la tarea.
- _Apariencia_ · Se corrigen el tamaño óptico de la tipografía, las sombras en capturas de vistas y la reutilización de vistas nativas al cambiar de sesión.

---

## Highlights

- **More reliable Codex questions and status.** Pulsar more reliably identifies **when Codex finishes, works or needs an answer**. Multi-part questions keep each answer in the right place, and coordinating agents can answer their helpers' questions without granting execution permissions.
- **Lighter images and documents.** The viewer shares file monitoring and limits simultaneous reads and image decoding. **Switching documents or closing a pane cancels its pending work** without interrupting other viewers using the same file.

## New

- _Agents_ · Agent signatures let you inspect **observed models and usage per task**, alongside the choice recorded at launch.

## Improvements

- _Agents_ · Tasks can declare difficulty and risk to select a model and effort according to the project's work mode. Receipts distinguish reported checks from available evidence.
- _Performance_ · Build coordination accounts for sustained agent CPU load. Project instructions are loaded by area to avoid unnecessary context.

## Fixes

- _Agents_ · Internal Codex threads and duplicate notifications are no longer confused with completion of the visible task. A generic notification is no longer treated as a permission request on its own.
- _Agents_ · Answers recheck the question, session and lock before writing. Simultaneous messages no longer interleave, and Pulsar warns when an unsent draft remains.
- _Agents_ · When Codex takes time to record an answer, Pulsar shows that confirmation is pending and prevents duplicate delivery. Unanswered parts retain their own question.
- _Agents_ · Task waits and watches are cancelled when their caller disconnects. Question changes are announced even when the agent keeps the same status.
- _Agents_ · Hibernated tasks no longer occupy active capacity. Waking a task rechecks capacity and preserves its identity.
- _Appearance_ · Fixes optical font sizing, shadows in view snapshots and native view reuse when switching sessions.
