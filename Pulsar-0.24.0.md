## Lo más destacado

- **Las compilaciones de prueba ya no llenan el disco.** Los agentes compilan mucho, y cada compilación deja una carpeta de varios GB. Ahora Pulsar las encuentra y las **borra solas cuando llevan unos días sin usarse** (3 de serie, en **Ajustes › Rendimiento › «Borrar las de prueba sin usar»**). En **«Limpiar»** ves lo que ocupan y puedes liberarlas a mano. Nunca toca lo que está compilando: vuelven a generarse solas al compilar.

## Mejoras

- _Agentes_ · Las tareas dejan un **recibo** al terminar: qué comprobaron, en qué commit y la app que compilaron. Quien las lanzó ya no repite esas pruebas ni revisiones, y quien prueba usa esa app sin volver a compilar.
- _Agentes_ · **`pulsar build-dir`** da a los agentes una carpeta de compilación estable para cada proyecto: dejan de compilar desde cero en cada sesión.

## Arreglos

- _Agentes_ · Si una copia de prueba de Pulsar pisaba su conexión, **los agentes perdían la CLI** (`pulsar agent`, `pulsar browser`…) hasta reiniciar. Ahora Pulsar la recupera sola en segundos.
- _Rendimiento_ · La columna de CPU del desplegable de recursos ya no se parte en dos líneas con el zoom de la interfaz.

---

## Highlights

- **Test builds no longer fill your disk.** Agents build a lot, and every build leaves a folder of several GB. Pulsar now finds them and **deletes them on its own once they go unused for a few days** (3 by default, in **Settings › Performance › “Delete unused test builds”**). In **“Clean up”** you can see how much space they take and free them by hand. It never touches anything that is building: they come back on their own the next time you build.

## Improvements

- _Agents_ · Tasks leave a **receipt** when they finish: what they checked, at which commit and the app they built. Whoever launched them no longer repeats those tests or reviews, and whoever tests uses that app without building it again.
- _Agents_ · **`pulsar build-dir`** gives agents a stable build folder for each project: they stop building from scratch in every session.

## Fixes

- _Agents_ · If a test copy of Pulsar took over its connection, **agents lost the CLI** (`pulsar agent`, `pulsar browser`…) until you restarted. Pulsar now recovers it on its own within seconds.
- _Performance_ · The CPU column in the resources popover no longer wraps onto two lines with interface zoom.
