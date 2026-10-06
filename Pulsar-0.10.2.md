## Lo más destacado

- **Arrastra archivos e imágenes a tus agentes.** Suelta sobre la terminal de un agente archivos de Finder, fotos de Fotos o imágenes de Safari, PDF o cualquier documento: le llegan sus rutas, y **Claude Code** y **Codex** convierten cada imagen en `[Image #1]`. Al arrastrar, el panel te dice a quién se lo pasas, y al soltar confirma cuántos archivos llegaron.

## Nuevo

- _Navegador_ · `pulsar browser animations list|pause|play|seek <ms>` y `perf [--duration s] [--scroll]`; `screenshot --hide-fixed` / `--hide <css>` y `wait --scroll-idle`; `emulate --reduced-motion` también en el navegador integrado.

## Mejoras

- _Navegador_ · `pulsar browser open` con `127.0.0.1` o `[::1]`: si el servidor solo escucha en la otra familia (Vite o Astro en `::1`), abre `localhost` y lo avisa. Y avisa una vez si el viewport `desktop` mide menos de 1024 px (para escritorio real, `viewport 1440x900`).
- _Navegador_ · Localizadores `name*=`, `^=`, `$=` y `/regex/i`; si nada coincide, el navegador sugiere nombres parecidos con su `@N`.
- _Navegador_ · Con `--backend chrome`, una ventana por agente; `focus` y `screenshot` esperan a que la página se vea, y las capturas y el pie de `run` dicen qué navegador se usó.

## Arreglos

- _Agentes_ · Pegar con ⌘V varios archivos copiados en Finder: **Codex** recibe cada imagen como imagen (antes, con más de una, las dejaba como rutas de texto).
- _Agentes_ · Pegar una imagen grande con ⌘V ya no frena Pulsar: la imagen se guarda en segundo plano, y la terminal se vuelve a pintar mientras el agente la procesa.

---

## Highlights

- **Drag files and images onto your agents.** Drop files from Finder, photos from Photos or images from Safari, PDFs or any document onto an agent’s terminal: it gets their paths, and **Claude Code** and **Codex** turn each image into `[Image #1]`. While you drag, the pane shows who you’re passing it to, and when you drop it confirms how many files arrived.

## New

- _Browser_ · `pulsar browser animations list|pause|play|seek <ms>` and `perf [--duration s] [--scroll]`; `screenshot --hide-fixed` / `--hide <css>` and `wait --scroll-idle`; `emulate --reduced-motion` in the built-in browser too.

## Improvements

- _Browser_ · `pulsar browser open` with `127.0.0.1` or `[::1]`: if the server only listens on the other family (Vite or Astro on `::1`), it opens `localhost` and says so. It also warns once if the `desktop` viewport is narrower than 1024 px (for a real desktop, `viewport 1440x900`).
- _Browser_ · `name*=`, `^=`, `$=` and `/regex/i` locators; if nothing matches, the browser suggests similar names with their `@N`.
- _Browser_ · With `--backend chrome`, one window per agent; `focus` and `screenshot` wait until the page is visible, and screenshots and the `run` footer say which browser was used.

## Fixes

- _Agents_ · Pasting several files copied in Finder with ⌘V: **Codex** gets each image as an image (with more than one, it used to leave them as text paths).
- _Agents_ · Pasting a large image with ⌘V no longer slows Pulsar down: the image is saved in the background, and the terminal repaints while the agent processes it.
