# Pulsar Agents · versiones publicadas

**[Pulsar Agents](https://pulsar.asklia.co)** es la app de Mac para lanzar Claude Code, Codex o cualquier agente de IA
de terminal a la vez, verlos trabajar en paralelo y responderles cuando te necesitan, también desde el iPhone.
Desarrollada por [Asklia](https://www.asklia.co).

- **Web**: [pulsar.asklia.co](https://pulsar.asklia.co) · [English](https://pulsar.asklia.co/en)
- **Descargar**: el `.dmg` de la [última versión](https://github.com/asklialab/pulsar-releases/releases/latest).
  Ábrelo y arrastra Pulsar a Aplicaciones. Requiere macOS 14 o posterior y Apple silicon.
- **Actualizaciones**: Pulsar las busca y descarga solo, y se instalan al salir de la app (o al pulsar «Reiniciar»).
- **Precios**: [30 días gratis, sin tarjeta](https://pulsar.asklia.co/precios).

## English

**[Pulsar Agents](https://pulsar.asklia.co/en)** is a Mac app to launch Claude Code, Codex or any terminal AI agent at
the same time, watch them work in parallel and answer them when they need you, even from your iPhone. Download the
`.dmg` from the [latest release](https://github.com/asklialab/pulsar-releases/releases/latest) (macOS 14+, Apple
silicon). [Pricing](https://pulsar.asklia.co/en/precios): 30-day free trial, no card required.

## Este repositorio

Solo contiene lo que se publica: el feed de actualizaciones (`appcast.xml`, servido con GitHub Pages en
`https://asklialab.github.io/pulsar-releases/appcast.xml`) y las notas de cada versión. Los `.dmg` van como archivos de
cada release. Se actualiza con `scripts/publish.sh` desde el repositorio de Pulsar; no se edita a mano (las entradas del
feed llevan la firma EdDSA de cada instalador).
