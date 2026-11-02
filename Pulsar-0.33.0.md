## Lo más destacado

- **Tus agentes saben quién lleva qué.** Un agente ya no pregunta a todas las sesiones: con **`pulsar agent who`** ve los agentes abiertos en todos tus espacios, con su carpeta, rama, título y estado, y escribe solo al que corresponde. Entre agentes del **mismo proyecto** el mensaje llega directo; a **otro espacio**, también si tú se lo pediste en ese turno. Si no, Pulsar lo retiene en una **tarjeta al pie del agente que escribe** con el texto exacto, y solo sale cuando pulsas «Enviar».

## A tener en cuenta

- _Resumen_ · **El Resumen se retira**: la vista general (⌘0), la Persiana, el correo de Gmail y Mail, el calendario, los recordatorios y `pulsar vista` ya no están. Pulsar deja de pedir los permisos de Calendario y Recordatorios.

## Nuevo

- _Agentes_ · **`pulsar agent who [texto]`** lista todos los agentes abiertos y su relación con quien pregunta (tú, tu tarea, mismo proyecto u otro espacio), y para Claude Code la dirección exacta de su sesión. Nunca enseña lo que hace otro agente: ni su pantalla, ni sus preguntas, ni sus informes.
- _Agentes_ · **`pulsar agent send`** llega también a agentes que no lanzaste, con una cabecera de Pulsar que dice quién escribe y cómo responderle. Siempre te pide el OK si quien escribe no es un agente, si el destino trabaja sin permisos, si el mensaje es largo o si se pasa de los topes; si descartas, ese agente tarda cada vez más en poder volver a pedirlo.

## Mejoras

- _Agentes_ · El papel «Calidad» se separa en **Diseño** (maquetas y llevarlas a la app) y **Pruebas** (pruebas con navegador o visor y revisión crítica), cada uno con su modelo y esfuerzo. Pruebas baja un escalón de serie, porque son largas y de muchos turnos. `--role quality` sigue valiendo y equivale a Diseño.
- _Integraciones_ · La skill de Pulsar para Codex, Claude y ChatGPT aclara que, **dentro de un panel de Pulsar**, los agentes se manejan con `pulsar agent …` y no con las herramientas `pulsar_*`, que allí no aparecen.

## Arreglos

- _Integraciones_ · Si un agente de Codex no pasa `PULSAR_PANE_ID` a sus órdenes (con `shell_environment_policy.inherit = "core"`), `pulsar agent`, `browser` y `board` ahora le dicen **cuál es su panel** y cómo repetir la orden, en vez de un error a secas. Sigue sin hacerse nada sin esa variable.

---

## Highlights

- **Your agents know who's on what.** An agent no longer asks every session: with **`pulsar agent who`** it sees the agents open across all your spaces, with their folder, branch, title and status, and writes only to the right one. Between agents of the **same project** the message goes straight through; to **another space**, too, if you asked it to in that turn. Otherwise Pulsar holds it in a **card at the foot of the agent that's writing** with the exact text, and it only goes out when you click “Send”.

## Good to know

- _Brief_ · **Brief is retired**: the overview (⌘0), the Shade, Gmail and Mail email, calendar, reminders and `pulsar vista` are gone. Pulsar no longer asks for Calendar and Reminders permissions.

## New

- _Agents_ · **`pulsar agent who [text]`** lists every open agent and how it relates to whoever asks (you, your task, same project or another space), and for Claude Code the exact address of its session. It never shows what another agent is doing: not its screen, questions or reports.
- _Agents_ · **`pulsar agent send`** also reaches agents you didn't launch, with a Pulsar header saying who's writing and how to reply. It always asks for your OK if the sender isn't an agent, if the target runs without permissions, if the message is long or if it goes over the limits; if you dismiss it, that agent waits longer each time before it can ask again.

## Improvements

- _Agents_ · The “Quality” role splits into **Design** (mockups and bringing them into the app) and **Testing** (browser or viewer tests and critical review), each with its own model and effort. Testing goes one step down by default, since tests are long and take many turns. `--role quality` still works and means Design.
- _Integrations_ · The Pulsar skill for Codex, Claude and ChatGPT makes clear that **inside a Pulsar pane** agents are handled with `pulsar agent …` and not with the `pulsar_*` tools, which don't show up there.

## Fixes

- _Integrations_ · If a Codex agent doesn't pass `PULSAR_PANE_ID` to its commands (with `shell_environment_policy.inherit = "core"`), `pulsar agent`, `browser` and `board` now tell it **which pane is its own** and how to repeat the command, instead of a bare error. Nothing runs without that variable, as before.
