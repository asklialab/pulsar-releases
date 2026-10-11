## Lo más destacado

- **Muchos agentes a la vez, sin que la Mac se trabe.** Cuando falta CPU, **el agente que miras y Pulsar van primero**: los que no ves ceden hasta que vuelvas a mirarlos, y con la Mac libre nadie va más lento. Cada herramienta de Claude cuesta **4 procesos en vez de 17**, y ningún aviso de estado se pierde aunque trabajen muchos agentes a la vez. Al cerrar un agente **se cierra lo que lanzó** (servidores, watchers); lo que se desligó para vivir por su cuenta aparece en **Limpiar** con su puerto, para que decidas tú.
- **Navegadores de agentes más rápidos y ligeros.** Las capturas pesan **unas 10 veces menos** (con `--scale`, `--format jpeg` y `--clip` si hacen falta) y se borran solas al día. Los clics de un agente van **el doble de rápido**, las ventanas emergentes también se duermen, y un navegador dormido ya no se despierta solo por pasar el ratón o abrir un menú. Los navegadores de agentes que no ves quedan **en silencio**.
- **Los agentes se turnan las compilaciones.** Con `pulsar lock build -- <orden>` las compilaciones y los tests pesados **esperan su turno** (2 a la vez en una Mac de 16 GB) en vez de saturarla todas juntas; los agentes ya saben usarlo. Si la Mac va cargada o caliente, **el medidor de memoria se tiñe de ámbar** y quien lanza tareas recibe un aviso. Las tareas delegadas arrancan con una guía **más corta**.

## Mejoras

- _Agentes_ · Abrir un espacio con muchos agentes **los escalona** antes de cargar el shell, así arrancan antes y sin picos.
- _Navegador_ · `text`, `html` y `eval` recortan dentro de la página (el valor entero sigue con `--json`), la consola se agrupa y la red solo guarda cuerpos cuando se piden.

## Arreglos

- _Agentes_ · Con muchos agentes a la vez, Pulsar ya no rechaza conexiones de `pulsar` ni de los avisos de los agentes.

---

## Highlights

- **Many agents at once without the Mac stalling.** When CPU runs short, **the agent you’re looking at and Pulsar go first**: the ones you can’t see yield until you look at them again, and with the Mac idle nobody slows down. Each Claude tool call costs **4 processes instead of 17**, and no status update gets lost even with many agents working at once. Closing an agent **closes what it launched** (servers, watchers); whatever detached to live on its own shows up in **Clean up** with its port, so you decide.
- **Faster, lighter agent browsers.** Screenshots are **about 10 times smaller** (with `--scale`, `--format jpeg` and `--clip` when needed) and clean themselves up after a day. An agent’s clicks are **twice as fast**, pop-up windows go to sleep too, and a sleeping browser no longer wakes up just because you hover it or open a menu. Agent browsers you can’t see stay **muted**.
- **Agents take turns on builds.** With `pulsar lock build -- <command>`, builds and heavy test runs **wait their turn** (2 at a time on a 16 GB Mac) instead of all swamping it together; agents already know how to use it. When the Mac is busy or hot, **the memory meter turns amber** and whoever launches tasks gets a heads-up. Delegated tasks start with a **shorter** guide.

## Improvements

- _Agents_ · Opening a space with many agents **staggers them** before loading the shell, so they start sooner and without spikes.
- _Browser_ · `text`, `html` and `eval` trim inside the page (the full value is still there with `--json`), the console is batched and the network only keeps bodies when asked.

## Fixes

- _Agents_ · With many agents at once, Pulsar no longer refuses connections from `pulsar` or from agent notifications.
