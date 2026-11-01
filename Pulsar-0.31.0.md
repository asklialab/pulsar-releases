## Nuevo

- _Visor_ · **Elegir entre audios y vídeos** es mucho más cómodo: `pulsar media ask` abre una **lista rápida** que se recorre con las flechas y la barra espaciadora, admite hasta **24 opciones**, **elegir varias** o **«Ninguna»**, pruebas **a ciegas** (`--ciegas`, sin nombres a la vista) y **volumen igualado** (`--igualar-volumen`, sin tocar tus archivos). **Comparar a la vez** reproduce hasta 6 sincronizados. También se contesta desde el iPhone.
- _Rendimiento_ · Una **cola de GPU** de verdad: `pulsar lock gpu -- <orden>` pone en fila renders, ffmpeg y modelos de uno en uno y espera si la memoria va justa. Al terminar, `pulsar lock` dice cuánto **duró**, cuánto **esperó** y el **pico de memoria** (también con `--json`), y `--read-only` evita esperar por carpeta a lo que solo lee.

## Mejoras

- _Agentes_ · Quien coordina ayudantes sabe por fin cuándo han **terminado de verdad**: `pulsar agent wait --report` espera al reporte, no al fin del turno, y `pulsar agent watch` sigue vigilando hasta que cada tarea reporte o se cierre y distingue si **reportó**, si **sigue trabajando en segundo plano** o si **se paró sin reportar**. Los estados salen en español.
- _Agentes_ · Cuando una tarea **pide atención**, el aviso dice qué espera (una elección del visor con su pregunta, un permiso o una pregunta) y quién la responde, y ya no se repite.
- _Agentes_ · `pulsar agent report` **nunca rechaza un reporte** por un nombre de `--checks` largo o con espacios: lo corrige y avisa. Fuera de un repo git, el recibo registra los **archivos producidos** con su tamaño, su huella SHA-256 y la duración.
- _Navegador_ · En Chrome, Dia y Arc, los `click`, `press` y `type` del agente cuentan como gesto de la persona: el **audio de una página suena** sin necesidad de `click --real`.
- _Agentes_ · La ayuda va al grano: `pulsar <grupo> help <acción>` (o `<acción> --help`) enseña solo esa acción. Y `pulsar agent spawn --file encargo.md` lanza una tarea desde un archivo (antes lanzaba el texto «encargo.md»).

## Arreglos

- _Visor_ · Abrir otro archivo en el visor ya no cancela una **elección pendiente**: se abre en otro visor y la pregunta sigue esperando.
- _Navegador_ · `pulsar browser eval` respeta `--timeout` (hasta 165 s) en el navegador integrado y en Chrome, y **nunca vuelve a ejecutar** un script que falla al ejecutarse (antes podía repetir, por ejemplo, un envío).

---

## New

- _Viewer_ · **Choosing between audio and video** is much easier: `pulsar media ask` opens a **quick list** you move through with the arrow keys and the space bar, with up to **24 options**, **picking several** or **“None”**, **blind** tests (`--ciegas`, no names in sight) and **matched loudness** (`--igualar-volumen`, without touching your files). **Compare together** plays up to 6 in sync. You can answer from the iPhone too.
- _Performance_ · A real **GPU queue**: `pulsar lock gpu -- <command>` lines up renders, ffmpeg and models one at a time and waits when memory is tight. When it finishes, `pulsar lock` reports how long it **ran**, how long it **waited** and the **peak memory** (also with `--json`), and `--read-only` keeps read-only work from waiting on a folder.

## Improvements

- _Agents_ · Whoever coordinates helpers finally knows when they're **really done**: `pulsar agent wait --report` waits for the report, not the end of the turn, and `pulsar agent watch` keeps watching until each task reports or closes, telling apart whether it **reported**, is **still working in the background** or **stopped without reporting**.
- _Agents_ · When a task **needs attention**, the notice says what it's waiting for (a viewer choice with its question, a permission or a question) and who answers it, and it no longer repeats.
- _Agents_ · `pulsar agent report` **never rejects a report** over a long `--checks` name or one with spaces: it fixes it and warns. Outside a git repo, the receipt records the **files produced** with their size, SHA-256 fingerprint and duration.
- _Browser_ · In Chrome, Dia and Arc, the agent's `click`, `press` and `type` count as a person's gesture: **a page's audio plays** without needing `click --real`.
- _Agents_ · Help gets to the point: `pulsar <group> help <action>` (or `<action> --help`) shows just that action. And `pulsar agent spawn --file brief.md` launches a task from a file (before, it launched the text “brief.md”).

## Fixes

- _Viewer_ · Opening another file in the viewer no longer cancels a **pending choice**: it opens in another viewer and the question keeps waiting.
- _Browser_ · `pulsar browser eval` honors `--timeout` (up to 165 s) in the built-in browser and in Chrome, and **never runs a script again** when it fails while running (before, it could repeat, for example, a submission).
