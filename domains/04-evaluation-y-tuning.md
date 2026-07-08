# Dominio 4: Perform evaluation, error analysis, and tuning (15-20%)

Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Completo** (4 apuntes, ~33 min de lectura).

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 20 | Success criteria y evaluation signals (cuali, cuanti y automated scanning) | 8 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/success-criteria-y-evaluation-signals) |
| 21 | Análisis de fallos: logs, plans, traces, outputs, artifacts | 8 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/analisis-de-fallos-logs-plans-traces) |
| 22 | Tuning del agente: instrucciones, workflows, memoria y tools | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/tuning-instructions-workflows-memoria-tools) |
| 23 | **LAB**: provocar un fallo, leer session logs, ajustar instructions | 10 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-provocar-fallo-leer-logs-ajustar-instructions) |

## Conceptos clave

- Signals de evaluación: cualitativas, cuantitativas y automated scanning (tests, lint, CodeQL, dependency review), y por qué ninguna sabe qué declaraste como scope.
- Un PR puede pasar todos los checks automáticos y aun así estar mal: las signals no reemplazan el criterio de review.
- Análisis de fallos a partir de logs, plans, traces, outputs y artifacts: dónde mirar según el síntoma.
- Las cuatro palancas de tuning: custom instructions, workflows, memoria y tools. El feedback es configuración persistida, no conversación en un comentario de PR.
- Por qué "no vuelvas a hacer X" en un comentario no tunea al agente si no se persiste en una de las cuatro palancas.

## Hands-on

El apunte 23 cierra el dominio con un LAB: se arma una trampa de contexto donde el agente elige una solución que rompe en producción, se leen los session logs para entender la decisión, y el fix termina siendo un cambio en la configuración (por ejemplo `copilot-instructions.md`), no una discusión con el agente.

---

[← Dominio 3](./03-memory-state-execution.md) · [README](../README.md) · [Dominio 5 →](./05-multi-agent-orchestration.md)
