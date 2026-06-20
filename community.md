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
| [Peterc3-dev/gh600-exam-prep](https://github.com/Peterc3-dev/gh600-exam-prep) | 3 archivos HTML monolíticos | **AI-slop high-volume** | Cuenta creada en ene-2026 con 78 repos públicos en 5 meses sobre temas no relacionados (Rust AI red team, AMD NPU, ratatui TUIs, Chrome extensions, etc.). Patrón de generación masiva con LLM. Sin build, sin data files, todo inline. Evitar. |
| [CarlasHub/gh600-agentic-ai-study-site](https://github.com/CarlasHub/gh600-agentic-ai-study-site) | SPA Vite + JSON masivo (101 lessons, 505 quizzes, 40 labs) | **AI-bulk-templated** | Carla Goncalves es developer real (cuenta 2017, foco histórico en A11Y / WCAG, no en agentic AI). El sitio impresiona por volumen pero el contenido está scaffoldeado con LLM: 101 lessons usan solo 6 plantillas de `agentRequestTemplate`, los 505 quizzes comparten una sola `correctExplanation` literal, y aparecen oraciones con gramática rota tipo *"The agent must pull requests as evidence objects for this repository task"*. Mucho volumen, cero depth técnico verificable, cero ejemplos YAML/JSON con valores concretos. 1 star, hash-routed SPA (no rankea bien en Google). |
| [Gist de naim149](https://gist.github.com/naim149/a8aa41c7468685b7d984822c38863aae) | Gist único `.md` | **AI con curaduría light** | El mejor del lote AI-generado: incluye snippets YAML/JSON con valores plausibles, sección "Domain Traps" y "Self-Check" por dominio, citations a docs oficiales. Pero sigue sin autoría humana verificable (cuenta sin track record relevante, gist creado en 1 día con 2 revisiones). Útil como referencia cruzada, no como estudio principal. 25 stars. |
| [zpwpe/gh600-study](https://github.com/zpwpe/gh600-study) | App Vite + React (94 preguntas, mock 50/120min) | **AI-assisted con atribución honesta** | El más transparente del lote: el README cita explícitamente sus fuentes (naim149, jtur671, PromptLab YT, Reddit) y declara los 4 LLMs usados (GPT-Pro, Claude, Grok, Gemini). Commit messages con `Co-Authored-By: Claude Sonnet 4.6`. Estructura solapa con el cuaderno (mismas referencias). No es estudio original pero la honestidad de atribución la diferencia del resto. |
| [CertyPro (8 repos GH-600)](https://github.com/CertyPro) | Hub + 7 labs TypeScript ejecutables | **AI-assisted con producción técnica** | Org creada el 10-jun-2026 (fábrica multi-cert: GH-200, GH-500, GH-600, GH-900). Commits firmados por entidad genérica "Coded Vision Design", sin instructor identificado, 0 stars/forks. **Pero los labs son TypeScript ejecutable de verdad**: MCP server con `@modelcontextprotocol/sdk` (4 tools + zod schemas + allowlist + rate-limiter + 7 tests), labs de memory/state, evaluation, multi-agent orchestration, guardrails, todo determinístico (sin LLM calls, corre offline en CI). El recurso más útil del lote AI a jun-2026: sirve como **sandbox técnico para practicar MCP / guardrails / evals**, no como curso pedagógico. Apto para "agarrá el lab, corré los tests, ignorá la prosa de los READMEs". |
| Practice tests en Udemy / SkillCertPro | Practice tests pagos | No verificado | Hay simulacros pagos en Udemy y dumps en SkillCertPro. No verificamos calidad. **No existe practice test oficial Microsoft/GitHub.** |

## Material en español (estado al 2026-06-19)

Aparte de este cuaderno, los pocos materiales en español que encontramos son notas periodísticas (qué es la cert, cómo apuntarse) o agregadores de links a docs oficiales. **No hay otro material didáctico exhaustivo en español.**

Si encontrás material serio en español que falte acá, abrí un issue o PR.

---

[← README](./README.md)
