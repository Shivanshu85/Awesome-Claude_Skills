# Security Policy & Vulnerability Disclosure

**Awesome-Claude_Skills** takes the security and safety of AI systems, prompt engineering patterns, Model Context Protocol (MCP) integrations, and developer environments seriously.

---

## Supported Versions

Since this repository is a documentation library, security updates apply to the current `main` branch documentation and canonical schemas.

| Component / Asset | Supported Version | Status |
| :--- | :--- | :--- |
| `schemas/metadata.schema.json` | v1.x (Draft 07) | Supported |
| `templates/` | v1.x | Supported |
| `skills/` Documentation | Main Branch | Supported |

---

## Reporting Security Vulnerabilities

If you discover a security vulnerability, security flaw in documented MCP server patterns, prompt injection vulnerability in recommended prompt templates, or secret exposure within documentation examples, **do not open a public GitHub issue**.

### Reporting Process

1. Email security disclosure reports to the maintainers at `security@awesome-claude-skills.org` (or submit a private security advisory on GitHub).
2. Include the following details:
   - Affected skill path (e.g., `skills/mcp/github/`)
   - Description of the security risk or vulnerability
   - Potential impact (e.g., prompt injection, code execution, unauthorized data access)
   - Suggested remediation or safer documentation pattern

### Response Timeline

- **Initial Acknowledgment**: Within 48 hours of receipt.
- **Assessment & Triage**: Within 5 business days.
- **Remediation Release**: Depending on severity, within 14 business days.

---

## AI-Specific Security Guidelines

When contributing skills to this repository, adhere to the following safety rules:

1. **No Credentials or API Keys**: Never include hardcoded API keys, bearer tokens, or real connection credentials in examples. Use environment variable placeholders (e.g., `${GITHUB_TOKEN}`).
2. **Prompt Injection Mitigations**: Skills documenting prompt engineering or system prompts must explicitly address prompt injection risks and document input validation/sanitization boundaries.
3. **MCP Tool Authorization**: Skills documenting Model Context Protocol (MCP) servers must highlight authorization requirements, read vs. write boundaries, and sandbox considerations.
4. **Code Execution Safety**: Documentation involving dynamic code evaluation or agentic shell tools must specify isolation requirements (containers, virtual machines, sandboxes).
