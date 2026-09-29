# Pulsar · versiones publicadas

Instaladores de [Pulsar](https://github.com/asklialab/pulsar-releases/releases) para macOS, desarrollado por Asklia.

- **Descargar**: el `.dmg` de la [última versión](https://github.com/asklialab/pulsar-releases/releases/latest).
  Ábrelo y arrastra Pulsar a Aplicaciones.
- **Actualizaciones**: Pulsar las busca y descarga solo, y se instalan al salir de la app (o al pulsar «Reiniciar»).

Este repositorio solo contiene lo que se publica: el feed de actualizaciones (`appcast.xml`, servido con GitHub Pages
en `https://asklialab.github.io/pulsar-releases/appcast.xml`) y las notas de cada versión. Los `.dmg` van como archivos
de cada release. Se actualiza con `scripts/publish.sh` desde el repositorio de Pulsar; no se edita a mano (las entradas
del feed llevan la firma EdDSA de cada instalador).
