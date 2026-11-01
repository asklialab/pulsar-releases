## Nuevo

- _Navegador_ · **Reloj virtual** para probar animaciones: `pulsar browser animations clock pause | advance <ms> | play | status` congela el tiempo de la página (rAF, temporizadores, `Date`, CSS y SMIL) y lo avanza cuadro a cuadro, así una captura justo después enseña ese instante exacto.
- _Navegador_ · `pulsar browser perf -- <acción>` mide mientras corre una acción (p. ej. un clic) y `--from-mark`/`--to-mark` recorta a los cuadros entre dos `performance.mark`. `perf`, `wait` y `expect` aguantan una navegación a mitad.

## Mejoras

- _Navegador_ · La **barra del navegador de un agente** en su tarjeta queda más limpia: un solo botón de **ampliar** (el de la cabecera), la **×** para cerrar su navegador dentro del 🌐 del conmutador y **«Abrir en el visor»** en las herramientas de la cabecera. La fila del navegador queda para la página: la **consola** sale solo con errores o abierta (si no, en «⋯» y con ⌥⌘C), **Compartir** es un icono que se enciende en vivo y las pestañas de las **ventanas emergentes** llevan el título de su página.
- _Agentes_ · «No puedo ahora» en una ventana emergente ya **no interrumpe al agente** ni le gasta un turno: la cierra y el agente se entera en su siguiente orden del navegador. Si esperaba en ella, su orden ya no la da por hecha, y una pregunta `pulsar browser ask` en una página que se cierra deja de esperar al momento.
- _Navegador_ · `pulsar browser wait --time 5` (o `2s`, `500ms`) hace una pausa fija y `viewport reset` vuelve al escritorio. Los avisos (un tamaño simulado que sigue fijado, un navegador libre adoptado) salen aparte, sin mezclarse con lo que un guion lee.

## Arreglos

- _Navegador_ · Cuando el navegador de un agente abre una **ventana emergente**, «Ver su navegador» la enseña y el aviso **desaparece** (antes se quedaba por más que lo pulsaras).
- _Navegador_ · Con un **tamaño de pantalla simulado** (p. ej. 1440×900) en un panel más pequeño, `svh` y `lvh` miden ese tamaño y no el del panel: las páginas a pantalla completa se ven como en un navegador de verdad.

---

## New

- _Browser_ · A **virtual clock** for testing animations: `pulsar browser animations clock pause | advance <ms> | play | status` freezes the page's time (rAF, timers, `Date`, CSS and SMIL) and moves it forward frame by frame, so a screenshot right after shows that exact instant.
- _Browser_ · `pulsar browser perf -- <action>` measures while an action runs (e.g. a click) and `--from-mark`/`--to-mark` trims to the frames between two `performance.mark`s. `perf`, `wait` and `expect` survive a navigation halfway through.

## Improvements

- _Browser_ · An **agent's browser bar** on its card is cleaner: a single **maximize** button (the header's), the **×** to close its browser inside the face switcher's 🌐 and **“Open in the viewer”** among the header tools. The browser row is just for the page: the **console** shows only with errors or when open (otherwise in “⋯” and with ⌥⌘C), **Share** is an icon that lights up when live, and **pop-up window** tabs carry their page's title.
- _Agents_ · “Can’t right now” on a pop-up window **no longer interrupts the agent** or costs it a turn: it closes it and the agent finds out on its next browser command. If it was waiting on it, its command no longer reports it as done, and a `pulsar browser ask` question on a page that closes stops waiting right away.
- _Browser_ · `pulsar browser wait --time 5` (or `2s`, `500ms`) pauses for a fixed time and `viewport reset` goes back to desktop. Notices (a simulated size still set, a free browser adopted) come out separately, without mixing with what a script reads.

## Fixes

- _Browser_ · When an agent's browser opens a **pop-up window**, “See its browser” shows it and the notice **goes away** (before, it stayed no matter how many times you clicked it).
- _Browser_ · With a **simulated screen size** (e.g. 1440×900) in a smaller pane, `svh` and `lvh` measure that size and not the pane's: full-screen pages look as they would in a real browser.
