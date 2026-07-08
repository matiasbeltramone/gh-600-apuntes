# Dominio 6: Implement guardrails and accountability (10-15%)

Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Borrador** (3 apuntes, ~26 min de lectura). En revisión; se estabiliza en los próximos días.

> Nota: este dominio está en borrador (learning-in-public). Los apuntes son legibles pero pueden ajustarse antes de marcarse como estables.

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 29 | Niveles de autonomía: clasificación de riesgo (operativo, security, compliance) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/niveles-de-autonomia-y-clasificacion-de-riesgo) |
| 30 | Guardrails y human-in-the-loop (bloquear violaciones de policy + least-privilege) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/guardrails-y-human-in-the-loop) |
| 31 | **LAB**: branch protection + CODEOWNERS + environment gates + agent firewall | 12 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-branch-protection-codeowners-environment-gates-firewall) |

## Conceptos clave

- Niveles de autonomía y clasificación de riesgo: operativo, security y compliance. GitHub no define niveles numerados; se razona por el riesgo de cada acción.
- Guardrails que bloquean violaciones de policy antes de que se ejecuten, con least-privilege como principio transversal.
- Human-in-the-loop obligatorio para acciones irreversibles o de alto riesgo.
- El "agent firewall" de red es built-in (no un panel configurable): conviene separar la capa de red de la capa de acciones.
- Accountability: dejar rastro auditable de qué agente hizo qué y bajo qué autorización.

## Hands-on

El apunte 31 cierra el cuaderno con un LAB que monta un sistema de guardrails en capas: branch protection + CODEOWNERS + environment gates + agent firewall, y muestra cómo se combinan para acotar lo que un agente puede hacer sin supervisión.

---

[← Dominio 5](./05-multi-agent-orchestration.md) · [README](../README.md)
