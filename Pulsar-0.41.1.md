## Arreglos

- _Agentes_ · Tras **reiniciar Pulsar**, lo que un ayudante reportó mientras tanto ya despierta a su orquestador al momento, en vez de esperar a tu siguiente mensaje.
- _Agentes_ · Con un agente en una carpeta con **enlace simbólico** (como `/tmp`), su consumo, su contexto y su último texto vuelven a aparecer.
- _Agentes_ · Sin avisos falsos de **«sigue con procesos en segundo plano: nc»** al acabar un turno: la conexión de los hooks de Pulsar ya no cuenta como proceso del agente.
- _Agentes_ · Una misma pregunta de un ayudante ya **no le llega dos veces** a su orquestador cuando este le escribe mientras espera.

---

## Fixes

- _Agents_ · After **restarting Pulsar**, what a helper reported in the meantime now wakes its orchestrator right away, instead of waiting for your next message.
- _Agents_ · With an agent in a folder behind a **symbolic link** (like `/tmp`), its usage, context and last text show up again.
- _Agents_ · No more false **“still has background processes: nc”** when a turn ends: the connection of Pulsar's hooks no longer counts as one of the agent's processes.
- _Agents_ · The same question from a helper **no longer reaches its orchestrator twice** when the orchestrator writes to it while it waits.
