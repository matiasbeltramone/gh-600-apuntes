# Dominio 5: Orchestrate multi-agent coordination (15-20%)

Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Completo** (5 apuntes, ~40 min de lectura).

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 24 | Patrones de orquestación multi-agente (researcher + editor, parallel, conflict detection) | 8 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/patrones-de-orquestacion-multi-agente) |
| 25 | Observabilidad multi-agente: artifacts auditables y handoffs | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/observabilidad-multi-agente-artifacts-handoffs) |
| 26 | Failures multi-agente: stalled, degraded, rollback y human-in-the-loop | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/failures-y-recovery-multi-agente) |
| 27 | Lifecycle de agentes en workflows multi-agente | 6 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lifecycle-de-agentes-en-workflows-multi-agente) |
| 28 | **LAB**: dos sub-agentes con Copilot SDK (researcher + editor) | 12 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-dos-subagentes-con-copilot-sdk) |

## Conceptos clave

- Patrones de orquestación: researcher + editor (lectura vs escritura), ejecución en paralelo, y conflict detection.
- El patrón que funciona es dejar las escrituras single-threaded: un researcher read-only que propone y un único editor dueño de tocar el código.
- Multi-agente no sale gratis: Anthropic reporta ~15x tokens en su sistema de research, y coding es el contraejemplo donde un solo agente bien llevado suele ganar (Anthropic y Cognition coinciden).
- Observabilidad: reconstruir el árbol de ejecución desde los eventos `subagent.*` y los toolCallId, con artifacts auditables y handoffs trazables.
- Failures: identificar ejecuciones stalled, degraded o parciales; recovery vía rollback o human-in-the-loop. El fallo suele manifestarse lejos de donde nace.
- Lifecycle: los agentes son configuración versionada en git (`.github/agents/*.md`), no una API. Add, update y retire se hacen por PR con review como código.

## Hands-on

El apunte 28 cierra con un LAB: se definen dos subagentes con el Copilot SDK (researcher read-only + editor con escritura) y se les da una tarea sin elegir agente, para observar al runtime delegar por inferencia y reconstruir el árbol con los eventos `subagent.*`. Incluye un anexo con la reproducción del flujo usando Claude Code disparado desde un issue de GitHub, verificando que la delegación es real (no narrada) y cómo se comporta ante un handoff vacío.

---

[← Dominio 4](./04-evaluation-y-tuning.md) · [README](../README.md) · [Dominio 6 →](./06-guardrails-y-accountability.md)
