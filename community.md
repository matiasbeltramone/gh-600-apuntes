# Community resources & sources of truth

Una curaduría honesta de qué hay disponible para el GH-600 más allá de este cuaderno. **Marcamos lo que sabemos que es AI-generated** para que no pierdas tiempo.

## Sources of truth (docs oficiales)

| Recurso | Para qué sirve |
|---|---|
| [Study guide GH-600](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600) | Fuente primaria. Define los 6 dominios y sub-skills. |
| [Página oficial de la cert](https://learn.microsoft.com/en-us/credentials/certifications/agentic-ai-developer/) | Logística, beta status, precio. |
| [Developing Agentic Systems Part 1 of 2 (Microsoft Learn)](https://learn.microsoft.com/en-us/training/paths/gh-developing-agentic-systems-1) | 3 módulos que cubren D1 y parte de D2. La "Part 2 of 2" prometida sigue sin existir a jun-2026. |
| [GitHub Docs: Copilot agents](https://docs.github.com/en/copilot/concepts/agents) | Conceptos centrales del Copilot coding agent. |
| [GitHub Docs: Copilot Memory](https://docs.github.com/en/copilot/concepts/agents/copilot-memory) | Memory feature (preview a jun-2026), regla de 28 días, scope. |
| [Risks and mitigations for Copilot cloud agent](https://docs.github.com/en/copilot/concepts/agents/cloud-agent-risk-mitigation) | Clave para D6 (guardrails). |

## First-hand exam experience

A jun-2026 la única experiencia first-hand documentada del examen beta es la de **Matías Daniel Adés** (consultor de Cybersecurity & GRC), publicada en LinkedIn el 30 de mayo de 2026. Lo que confirma:

- **~65 preguntas en 120 min**, no 60 como se asumía
- **2 case studies largos al inicio** (uno de 7 preguntas, otro de 12), el primero le consumió ~1 hora
- Tipos de pregunta: multiple choice clásico, checkboxes multi-respuesta, **drag-and-drop** para completar código, **ordering cronológico** descartando pasos que no aplican
- El examen pide **interpretar artefactos reales**: YAML, JSON, logs de CLI y sesión, agent files, MCP config, hooks, fragmentos de GitHub Actions
- "No es certificación de fundamentos": apunta a perfiles con experiencia real
- Tips logísticos: rendir en centro Pearson presencial (no online), reservar a la mañana, en preguntas largas marcar y seguir

Esta data es la que mejor calibra cómo escribir y leer cualquier material de estudio del GH-600.

## Otros materiales (assessment honesto)

| Recurso | Tipo | Calidad | Nota |
|---|---|---|---|
| [jtur671/gh-600-study-guide](https://github.com/jtur671/gh-600-study-guide) | Repo + serie de 7 videos en dev.to | **AI-slop** | Cuenta dev.to creada el mismo día que publicó (22-may-2026), username con sufijo random, videos de 2-5 min tipo HeyGen, 1 solo commit en el repo, flashcards sin un solo YAML real, mock exam con preguntas conceptuales sin case studies (no simula el formato real del examen). Evitar. |
| [Gist de naim149](https://gist.github.com/naim149/a8aa41c7468685b7d984822c38863aae) | Gist único `.md` | **AI con curaduría light** | Mejor que jtur671: incluye snippets YAML/JSON, sección "Domain Traps" y "Self-Check" por dominio, citations a docs oficiales. Pero sigue sin autoría humana verificable (cuenta sin track record relevante, gist creado en 1 día con 2 revisiones). Útil como referencia cruzada, no como estudio principal. |
| Practice tests en Udemy / SkillCertPro | Practice tests pagos | No verificado | Hay simulacros pagos en Udemy y dumps en SkillCertPro. No verificamos calidad. **No existe practice test oficial Microsoft/GitHub.** |

## Material en español (estado al 2026-06-19)

Aparte de este cuaderno, los pocos materiales en español que encontramos son notas periodísticas (qué es la cert, cómo apuntarse) o agregadores de links a docs oficiales. **No hay otro material didáctico exhaustivo en español.**

Si encontrás material serio en español que falte acá, abrí un issue o PR.

---

[← README](./README.md)
