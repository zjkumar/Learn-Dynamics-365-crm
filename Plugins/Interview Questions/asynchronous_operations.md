# Async Service

- It handles the execution of async plugins and workflows.
- The async operations are registered with async service when event triggers.
- Async service uses managed FIFO queue to process these operations whenever resources are available.
- So there is no guarantee, which operation would get executed first.

**Benefits :**
- It takes of the load and improve system performance.
