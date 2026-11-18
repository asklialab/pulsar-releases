## Lo más destacado

- **Vuelve a cualquier conversación.** La paleta de lanzar tiene una pestaña nueva, **Sesiones**: busca entre las conversaciones pasadas de Claude y Codex, mira sus últimos turnos y **reanúdala con ↩** en el espacio de su carpeta. Si su panel sigue abierto o hibernado, te lleva a él. Y **⇧⌘T reabre el último panel que cerraste**.
- **Busca en la terminal y salta entre tus mensajes.** **⌘F** convierte la cabecera del panel en un buscador con contador; ↩ y ⇧↩ van a la coincidencia siguiente y a la anterior. Al acercar el puntero al borde derecho aparece la **regla de turnos**: una marca por cada mensaje tuyo, para volver a él con un clic. Sin botones nuevos: también está en el «⋯» del panel.
- **Abre el código en tu editor.** **⌘ clic en una ruta** de la terminal abre ese archivo en tu editor, en su línea. Y **⌥⌘O** abre la carpeta del agente: está en el menú de la carpeta y la rama, arriba, y en el «⋯» de cada panel, con «Abrir con» para elegir otro. El editor por defecto se elige en **Ajustes › General**.
- **Cuánto te queda de la suscripción.** Al pie de la barra lateral, junto a Memoria, la fila **Límites** dice lo que **queda** de cada suscripción; un clic abre el detalle con el ritmo al que vas y cuándo se reinicia. Por ahora lee a Codex; de Claude se enseña «sin dato» en vez de inventar un número.

## A tener en cuenta

- _Seguridad_ · Un enlace de la terminal o del visor que **abre otra app** (cualquiera que no sea una web o un correo) ahora pide confirmación y te enseña la dirección entera antes de abrirla.

## Nuevo

- _Agentes_ · **Pulsar pregunta antes de salir** si quedan agentes trabajando (⌘Q y el botón rojo de la ventana).
- _Rendimiento_ · **La Mac no entra en reposo mientras trabajan los agentes.** Por defecto, solo conectada a la corriente; se cambia en Ajustes › Rendimiento › Reposo de la Mac (Nunca, Solo conectada a la corriente, Siempre). La pantalla puede apagarse igual.
- _Agentes_ · Para los agentes: `pulsar open <ruta>[:línea]` abre un archivo de su proyecto en tu editor, `pulsar agent sessions`, `resume` y `reopen` consultan y reanudan las sesiones de su proyecto, y `pulsar system limits` dice cuánto queda de la suscripción.

## Mejoras

- _Rendimiento_ · **Pulsar descansa cuando no lo miras.** Con la ventana oculta se detienen los relojes de la interfaz y se lee mucho menos la pantalla de los agentes; en ahorro de energía, las medidas se espacian.
- _Paneles_ · **Mientras escribes en una terminal, nada que no hagas tú te quita el teclado**: ni otro agente, ni un panel que se abre o se cierra solo, ni una orden de la CLI. Un clic tuyo o un atajo con ⌘ siguen llevándote adonde quieras.
- _Apariencia_ · **La barra de menús pasa de 12 menús a 6**: Pulsar, Archivo, Edición, Visualización, Ventana y Ayuda. Notificaciones y Dictado van dentro de Pulsar; Navegador y Zoom, en Archivo y Visualización; Panel y Workspace, en Ventana. Todos los atajos se conservan.

## Arreglos

- _Barra lateral_ · Si el archivo de tus espacios no se puede leer, Pulsar **ya no lo pisa**: guarda una copia con fecha y te avisa en la barra lateral, también si los espacios dejan de guardarse.
- _Paneles_ · Mantener pulsado **⌘W** ya no cierra varios paneles seguidos.
- _Agentes_ · `pulsar agent clean` ya no cierra paneles que no pudo inspeccionar del todo ni terminales recién abiertas.

---

## Highlights

- **Get back to any conversation.** The launch palette has a new tab, **Sessions**: search your past Claude and Codex conversations, look at their last turns and **resume one with ↩** in the space for its folder. If its pane is still open or hibernated, it takes you there. And **⇧⌘T reopens the last pane you closed**.
- **Search the terminal and jump between your messages.** **⌘F** turns the pane header into a search field with a counter; ↩ and ⇧↩ go to the next and previous match. Move the pointer to the right edge and the **turn ruler** appears: one mark per message of yours, to get back to it with a click. No new buttons: it's also in the pane's “⋯” menu.
- **Open the code in your editor.** **⌘-click a path** in the terminal to open that file in your editor, at its line. And **⌥⌘O** opens the agent's folder: it's in the folder-and-branch menu at the top and in each pane's “⋯”, with “Open with” to pick another one. Choose the default editor in **Settings › General**.
- **How much of your plan is left.** At the bottom of the sidebar, next to Memory, the **Limits** row tells you what's **left** of each plan; one click opens the detail with your pace and when it resets. For now it reads Codex; for Claude it shows “no data” rather than making up a number.

## Good to know

- _Security_ · A link in the terminal or the viewer that **opens another app** (anything that isn't a web page or an email) now asks for confirmation and shows you the full address before opening it.

## New

- _Agents_ · **Pulsar asks before quitting** if agents are still working (⌘Q and the window's red button).
- _Performance_ · **Your Mac doesn't go to sleep while agents are working.** By default, only when plugged in; change it in Settings › Performance › Mac sleep (Never, Only when plugged in, Always). The display can still turn off.
- _Agents_ · For agents: `pulsar open <path>[:line]` opens a file from their project in your editor, `pulsar agent sessions`, `resume` and `reopen` list and resume their project's sessions, and `pulsar system limits` tells how much of the plan is left.

## Improvements

- _Performance_ · **Pulsar rests when you're not looking.** With the window hidden the interface clocks stop and agents' screens are read far less often; in Low Power Mode, measurements are spaced out.
- _Panes_ · **While you're typing in a terminal, nothing but you takes the keyboard away**: not another agent, not a pane that opens or closes by itself, not a CLI command. Your click or a ⌘ shortcut still takes you wherever you want.
- _Appearance_ · **The menu bar goes from 12 menus to 6**: Pulsar, File, Edit, View, Window and Help. Notifications and Dictation live inside Pulsar; Browser and Zoom, in File and View; Pane and Workspace, in Window. Every shortcut stays the same.

## Fixes

- _Sidebar_ · If your spaces file can't be read, Pulsar **no longer overwrites it**: it keeps a dated copy and tells you in the sidebar, also if spaces stop being saved.
- _Panes_ · Holding **⌘W** no longer closes several panes in a row.
- _Agents_ · `pulsar agent clean` no longer closes panes it couldn't fully inspect or terminals that were just opened.
