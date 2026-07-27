# Model Context Protocol (`skills/mcp/`)

Welcome to the **Model Context Protocol (MCP)** category index. This category documents specifications, servers, tools, resources, and client integration patterns for the Model Context Protocol.

---

## Category Overview

MCP is an open standard that connects AI applications to external tools, databases, and developer environments. This category documents production MCP server implementations, protocol transports (stdio, SSE), and tool schemas.

For detailed domain boundaries and inclusion rules, see [docs/taxonomy.md](file:///docs/taxonomy.md#4-mcp-model-context-protocol).

---

## Target Audience

- MCP Server Developers building custom tool integrations for Claude Code, Cursor, or custom hosts.
- DevOps engineers exposing database or repository tools to AI agents over standard transport layers.
- Security auditors verifying MCP tool schema authorization boundaries.

---

## Recommended Learning Order

1. **MCP Protocol Architecture**: Host-Client-Server relationships and transport choices.
2. **Tool & Resource Schemas**: Defining JSON-RPC methods, input schemas, and resource URIs.
3. **Production Server Deployments**: Stdio vs. SSE deployment and sandbox isolation.

---

## Related Categories

- [skills/developer-tools/](file:///skills/developer-tools/README.md): CLI utilities and developer helper tools.
- [skills/ai-ides/](file:///skills/ai-ides/README.md): Integrating MCP servers into Cursor, Claude Code, and Windsurf.

---

## Contained Skills Index

*No skills are populated in this skeleton repository yet. Contributions welcome!*

To add a new skill to this category:
1. Review [CONTRIBUTING.md](file:///CONTRIBUTING.md).
2. Copy `templates/README.template.md` to `skills/mcp/<skill-slug>/README.md`.
3. Validate `metadata.json` against `schemas/metadata.schema.json`.

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
