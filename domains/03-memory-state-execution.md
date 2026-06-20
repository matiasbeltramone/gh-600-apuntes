# Dominio 3: Manage memory, state, and execution (10-15%)

Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Completo** (4 apuntes, ~32 min de lectura).

> Nota editorial: el study guide pone "execution" en este dominio, pero en el cuaderno los temas de execution se cubrieron en el dominio 2 (apuntes 11-13) porque operativamente van pegados a tools y entorno. Este dominio se enfoca en memory y state.

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 16 | Estrategias de memoria: short-term, long-term y external (Copilot Memory) | 8 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/estrategias-de-memoria-short-long-external) |
| 17 | Persistencia de estado y context drift | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/persistencia-de-estado-y-context-drift) |
| 18 | Continuidad de memoria entre tools y environments | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/continuidad-de-memoria-entre-tools-environments) |
| 19 | **LAB**: habilitar Copilot Memory, crear repo facts y ver expiración | 10 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-copilot-memory-y-repo-facts) |

## Conceptos clave

- Las tres clases de memoria que el study guide distingue (short-term, long-term, external)
- Cómo Copilot Memory implementa repo facts vs user preferences, con qué scope cada uno
- Reglas de expiración (28 días) y pruning
- Cómo capturar estado como durable artifacts para retomar trabajo sin divergir de decisiones previas
- Detectar context drift durante ejecuciones extendidas
- Smart zone / dumb zone (Matt Pocock) y su conexión con context rot
- Compartir state entre tools (cloud agent, code review, CLI) sin contexto conflictivo ni stale

## Hands-on

El apunte 19 cierra el dominio con un LAB: habilitación de Copilot Memory en un repo, captura de repo facts, validación de citations, edición manual de facts, y razonamiento sobre qué pasa cuando una fuente cambia antes que Memory la recapture.

---

[← Dominio 2](./02-tools-y-mcp.md) · [README](../README.md)
