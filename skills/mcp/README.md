# Model Context Protocol (MCP) (`skills/mcp/`)

Welcome to the **Model Context Protocol (MCP)** category index. This category documents open-source MCP servers, standardized tool specifications, resource providers, and prompt servers connecting AI coding assistants safely to local and remote resources.

---

## What is MCP?

The Model Context Protocol (MCP) is an open specification that enables AI models to securely interact with local filesystems, git repositories, databases, web APIs, and specialized developer utilities through standardized tool, resource, and prompt interfaces.

---

## Why MCP Matters

- **Eliminates Custom Tool Wrappers**: Replaces ad-hoc integration scripts with a single universal protocol standard supported across Claude Code, Cursor, Windsurf, Roo Code, and CLI tools.
- **Enforces Security & Sandboxing**: Provides clear tool permission controls and execution boundaries.
- **Standardizes Developer Workflows**: Enables instant plug-and-play integration for local files, version control, and external services.

---

## When to Use MCP

- When giving AI coding assistants access to local file editing, git operations, or terminal output.
- When connecting AI agents to external APIs (GitHub, web fetching, database queries).
- When implementing multi-step reasoning protocols (like Sequential Thinking).

---

## Recommended Learning Order

1. **MCP Core Concepts**: Tools, Resources, Prompts, and Transports (stdio, SSE).
2. **Local System MCP Servers**: Filesystem MCP, Git MCP.
3. **API & Remote MCP Servers**: GitHub MCP, Fetch MCP.
4. **Reasoning MCP Servers**: Sequential Thinking MCP.

---

## Related Categories

- 🔍 [skills/codebase-intelligence/](file:///skills/codebase-intelligence/README.md): Codebase indexing and repository packing.
- 🔄 [skills/agent-workflows/](file:///skills/agent-workflows/README.md): Sequential thinking and reasoning protocols.
- 🛡️ [skills/security/](file:///skills/security/README.md): Tool permissions and sandboxing security.

---

## Documented Tools

Below are the open-source MCP servers documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **Filesystem MCP** | Secure local file reading, writing, and directory traversal | ✅ Active | *[View Guide](file:///skills/mcp/README.md)* |
| **Git MCP** | Git history, diffs, log inspection, and branch management | ✅ Active | *[View Guide](file:///skills/mcp/README.md)* |
| **Fetch MCP** | Web page fetching and markdown conversion server | ✅ Active | *[View Guide](file:///skills/mcp/README.md)* |
| **GitHub MCP** | GitHub API integration for PRs, issues, and code search | ✅ Active | *[View Guide](file:///skills/mcp/README.md)* |
| **Sequential Thinking MCP** | Dynamic multi-step reasoning server for complex problem solving | ✅ Active | *[View Guide](file:///skills/mcp/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
