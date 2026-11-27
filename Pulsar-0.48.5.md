## Mejoras

- _Rendimiento_ · La hoja **«Limpiar»** enseña las compilaciones al momento en vez de esperar a buscar en todos los worktrees, y la búsqueda es varias veces más rápida. Al borrar, lo elegido desaparece enseguida, Ajustes y el medidor dicen «Borrando…» y al acabar un aviso cuenta lo liberado y lo que se quedó en uso.
- _Visor_ · Al **elegir entre vídeos**, el vídeo se queda casi todo el panel: la lista de opciones mide lo que ocupan sus filas, y «Comparar a la vez» reparte las celdas para que se vean lo más grandes posible.

## Arreglos

- _Rendimiento_ · La **limpieza de compilaciones** encuentra también los `.build` que deja el índice de Swift (SourceKit-LSP), que antes se quedaban para siempre; ya no ofrece carpetas que nunca se pueden borrar porque llevan un worktree dentro, y quita las carpetas vacías que quedaban en las cachés.
- _Agentes_ · `pulsar lock` deja de esperar en cuanto se cierra la terminal que pidió el turno, y el nombre de otro panel ya no puede enviar códigos de control a tu terminal.

---

## Improvements

- _Performance_ · The **Clean up** sheet shows builds right away instead of waiting to search every worktree, and the search is several times faster. When deleting, what you chose disappears at once, Settings and the meter say “Deleting…”, and a notice at the end tells you what was freed and what stayed in use.
- _Viewer_ · When **choosing between videos**, the video gets most of the pane: the list of options takes only the room its rows need, and “Compare side by side” lays out the cells so they’re as large as possible.

## Fixes

- _Performance_ · **Build cleanup** now also finds the `.build` folders left by Swift’s index (SourceKit-LSP), which used to stay forever; it no longer offers folders that can never be deleted because they contain a worktree, and it removes the empty folders left behind in the caches.
- _Agents_ · `pulsar lock` stops waiting as soon as the terminal that asked for a turn closes, and another pane’s name can no longer send control codes to your terminal.
