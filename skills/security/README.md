# Security (`skills/security/`)

Welcome to the **Security** category index. This category documents prompt injection defenses, tool permission boundaries, sandboxing utilities, secret scanning guardrails, and security policies for AI coding assistants.

---

## What is Security?

Security in AI coding workflows addresses risks unique to LLM integrations. This includes protecting local developer environments against malicious prompt injection in untrusted repositories, enforcing strict file access boundaries for MCP tools, and preventing secret exposure in prompt payloads.

---

## Why Security Matters

- **Protects Local Developer Workspaces**: Prevents malicious repositories or web content from executing unauthorized terminal commands.
- **Prevents Secret Exposure**: Scans prompts and context payloads to block API keys or credentials from leaking to LLM APIs.
- **Enforces Principle of Least Privilege**: Enforces read-only sandboxing for automated tool calls.

---

## When to Use Security

- When using AI assistants to analyze third-party or untrusted open-source code repositories.
- When configuring MCP servers that execute system tools or access databases.
- When deploying enterprise AI coding guidelines across development teams.

---

## Recommended Learning Order

1. **Tool Permission Boundaries**: Configuring read-only vs. read-write MCP permissions.
2. **Prompt Injection Defense**: Guardrail patterns for untrusted input ingestion.
3. **Secret Scanning Guardrails**: Pre-prompt sanitization for credentials and API keys.

---

## Related Categories

- 🔌 [skills/mcp/](file:///skills/mcp/README.md): Model Context Protocol server permission controls.
- ✍️ [skills/prompt-engineering/](file:///skills/prompt-engineering/README.md): System prompt guardrails.
- 🔭 [skills/observability/](file:///skills/observability/README.md): Security audit logging and tracing.

---

## Documented Tools

Below are the open-source security tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **PromptGuard** | Prompt injection defense and input sanitization library | ✅ Active | *[View Guide](file:///skills/security/README.md)* |
| **ToolSandbox** | Execution sandbox and permission gate for MCP tool calls | ✅ Active | *[View Guide](file:///skills/security/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
