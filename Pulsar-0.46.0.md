## A tener en cuenta

- _Agentes_ · **Antigravity CLI sustituye a Gemini CLI.** Gemini CLI ya no se actualiza: en su sitio de la barra de lanzar está su sucesor, `agy`, con su logo, sus modelos y su estado exacto. Tus espacios guardados lo abren sin hacer nada. El modo «Preguntar» no está disponible con Antigravity, porque `agy` no lo ofrece.

## Nuevo

- _Navegador_ · **El iPhone ve el navegador de cada agente mucho mejor.** Pide capturas nítidas al acercar la imagen, puede ver la página entera de un navegador que abrió el agente y, cuando te pide elegir con `pulsar browser choose`, también ve las opciones que quedan fuera de la vista. Nunca ve un navegador tuyo.
- _Agentes_ · `pulsar browser choose --note "etiqueta=nota"` añade una nota corta a cada opción; se ve bajo su nombre en la Mac y en el iPhone.
- _Compartir en vivo_ · **«En tu teléfono».** Si el agente tiene abierto su servidor de desarrollo (localhost), el iPhone puede abrirlo con Face ID, solo para ti, como un compartido en vivo. Es la página de verdad: lo que envíes en sus formularios llega a ese servidor.

## Mejoras

- _Integraciones_ · **Codex usa Pulsar sin pedir permiso cada vez.** Cada panel de Codex lleva la herramienta `pulsar`, así que abrir el visor, usar el navegador o escribir a otro agente funciona aunque Codex esté en su sandbox. Pulsar comprueba en cada llamada que viene de ese panel.
- _Seguridad_ · Cuando Pulsar lee git en una carpeta que eligió un agente (recibos de `agent report`, `pulsar lock`, envíos y reuniones), lo hace sin poder lanzar programas, escribir ni usar la red: la configuración de un repositorio ya no puede ejecutar nada fuera del sandbox del agente.
- _Ajustes_ · **Ajustes › iPhone** explica qué ve el iPhone del navegador de un agente, y cada página entera o «En tu teléfono» que pide queda en el registro.

---

## Good to know

- _Agents_ · **Antigravity CLI replaces Gemini CLI.** Gemini CLI is no longer updated: its successor, `agy`, takes its place in the launch bar, with its own logo, models and exact status. Your saved spaces open it with nothing to do. “Ask” mode isn't available with Antigravity, because `agy` doesn't offer it.

## New

- _Browser_ · **The iPhone sees each agent's browser much better.** It asks for sharp captures when you zoom in, can see the whole page of a browser the agent opened and, when it asks you to choose with `pulsar browser choose`, it also sees the options that are out of view. It never sees a browser of yours.
- _Agents_ · `pulsar browser choose --note "label=note"` adds a short note to each option; it shows under its name on the Mac and on the iPhone.
- _Share live_ · **“On your phone”.** If the agent has its development server open (localhost), the iPhone can open it with Face ID, just for you, as a live share. It's the real page: whatever you submit in its forms reaches that server.

## Improvements

- _Integrations_ · **Codex uses Pulsar without asking every time.** Each Codex pane carries the `pulsar` tool, so opening the viewer, using the browser or writing to another agent works even inside Codex's sandbox. Pulsar checks on every call that it comes from that pane.
- _Security_ · When Pulsar reads git in a folder an agent chose (`agent report` receipts, `pulsar lock`, sends and meetings), it does so without being able to launch programs, write or use the network: a repository's settings can no longer run anything outside the agent's sandbox.
- _Settings_ · **Settings › iPhone** explains what the iPhone sees of an agent's browser, and every whole page or “On your phone” it asks for is kept in the log.
