# Dominio 2: Implement tool use and environment interaction (20-25%)

El dominio con mayor peso del examen. Cómo el cuaderno cubre este dominio del [study guide oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/gh-600).

Estado: **Completo** (9 apuntes, ~67 min de lectura).

> Nota editorial: el study guide oficial pone "execution context" en el dominio 3. En este cuaderno está acá (apunte 11) porque operativamente va pegado a tools y entorno.

## Apuntes

| # | Título | Duración | Link |
|---|---|---|---|
| 7 | Tools: selección, configuración y permisos (least privilege en serio) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/tools-seleccion-configuracion-permisos) |
| 8 | MCP servers: qué son, cómo se agregan, y el GitHub remote MCP | 12 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/mcp-servers-introduccion-y-github-remote) |
| 9 | Default MCP servers (GitHub MCP, Playwright MCP) | 6 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/default-mcp-servers-github-y-playwright) |
| 10 | MCP registries y allow-lists (gobierno de tools externos) | 6 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/mcp-registries-y-allow-lists) |
| 11 | Execution context y scoping (repo, branch, CI workflows, env) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/execution-context-y-scoping) |
| 12 | Acciones autónomas: branches, PRs, agent firewall y restricciones | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/acciones-autonomas-branches-prs-firewall) |
| 13 | Error handling, retries, rollbacks y escalation paths | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/error-handling-retries-rollbacks-escalation) |
| 14 | Custom agents con el Copilot SDK (.agent.md, tools, allow-lists) | 7 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/custom-agents-con-copilot-sdk) |
| 15 | **LAB**: MCP server custom + asignación a agente + tools en acción | 12 min | [Leer](https://matiasbeltramone.com/apuntes/github-agentic-ai/lab-mcp-server-custom-asignado-a-agente) |

## Conceptos clave

- Tools como capa de capacidad: el agente no es lo que sabe, es lo que puede tocar
- MCP como el "USB-C de los agentes": tools, resources, prompts; transports stdio vs streamable HTTP
- Autenticación: OAuth interactivo para IDEs vs tokens pre-autorizados para cloud agents
- **La trampa de naming**: `servers` (mcp.json IDE) vs `mcpServers` (JSON CLI/repo) vs `mcp-servers` (YAML frontmatter de `.agent.md`)
- Registries y allow-lists para gobernar qué MCP servers pueden enchufarse a los agentes de una organización
- Execution context: la VM ephemeral del cloud agent y las cinco capas del scope (repo, branch, filesystem, red, secrets)
- Agent firewall vs runner firewall (la confusión más común del dominio)
- Custom agents en el repo con `.agent.md`, allow-lists por agente, MCP servers scopeados

## Hands-on

El apunte 15 cierra el dominio con un LAB: armado paso a paso de un MCP server propio en TypeScript con SQLite, conexión al agente vía `mcp.json`, prueba en vivo de que el scoping funciona, y un fallo forzado para ver el comentario de escalation en acción.

---

[← Dominio 1](./01-architecture-y-sdlc.md) · [README](../README.md) · [Siguiente: Dominio 3 →](./03-memory-state-execution.md)
