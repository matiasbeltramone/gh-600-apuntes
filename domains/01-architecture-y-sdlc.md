# Dominio 1: Prepare agent architecture and SDLC processes (15-20%)

Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Completo** (6 apuntes, ~50 min de lectura).

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 1 | Qué es un agente agéntico en el SDLC (y por qué GitHub es el lugar) | 11 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/que-es-un-agente-agentico-en-el-sdlc) |
| 2 | El contributor model aplicado a agentes (anti-patterns cuando se rompe) | 8 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/contributor-model-aplicado-a-agentes) |
| 3 | Definir tareas de agentes: inputs, outputs y success criteria | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/definir-tareas-de-agentes-inputs-outputs-success-criteria) |
| 4 | Separar planning, reasoning y execution (el plan como artifact revisable) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/separar-planning-reasoning-execution) |
| 5 | Observabilidad y degree of autonomy (balance control vs velocidad) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/observabilidad-y-degree-of-autonomy) |
| 6 | **LAB**: setup base con Copilot coding agent | 12 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-setup-base-copilot-coding-agent) |

## Conceptos clave que vas a aprender

- Diferencia agente vs asistente, lifecycle plan→act→evaluate
- Las cuatro propiedades del contributor model (identidad, inspección, review, reglas iguales) y los cinco anti-patterns típicos cuando alguna se afloja
- Cómo modelar inputs / outputs / success criteria para que el agente no devuelva ruido
- Por qué el plan es el artifact revisable y cómo se ven los plan modes reales (Claude Code plan mode, Copilot draft PR)
- Cuándo graduar autonomía por acción (no por agente) sin frenar la entrega

## Hands-on

El apunte 6 cierra el dominio con un LAB: setup completo de un repo con Copilot coding agent, branch protection, custom instructions, primer issue asignado, lectura de los artifacts que deja el agente y verificación de que las reglas se aplican igual al agente que a un humano.

---

[← README](../README.md) · [Siguiente: Dominio 2 →](./02-tools-y-mcp.md)
