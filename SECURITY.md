# Security Policy & Vulnerability Disclosure

**Awesome-Claude_Skills** takes the security and safety of AI systems, prompt engineering patterns, Model Context Protocol (MCP) integrations, tool permission boundaries, and developer environments seriously.

---

## Supported Versions

Since this repository is a documentation library for AI optimization tools and protocols, security updates apply to the current `main` branch documentation, canonical schemas, and template guides.

| Component / Asset | Supported Version | Status |
| :--- | :--- | :--- |
| `schemas/metadata.schema.json` | v1.x (Draft 07) | Supported |
| `templates/` | v1.x | Supported |
| `skills/` Documentation | Main Branch | Supported |

---

## Reporting Security Vulnerabilities

If you discover a security vulnerability in documented MCP server implementations, unsafe default configurations, prompt injection flaws in recommended templates, or secret exposures within documentation examples, **do not open a public GitHub issue**.

### Reporting Process

1. Email security disclosure reports to the maintainers at `security@awesome-claude-skills.org` (or submit a private security advisory on GitHub).
2. Include the following details:
   - Affected tool path (e.g., `skills/mcp/filesystem-mcp/`)
   - Description of the security risk or vulnerability
   - Potential impact (e.g., prompt injection, code execution, unauthorized file read/write, credential exposure)
   - Suggested remediation or safer documentation pattern

### Response Timeline

- **Initial Acknowledgment**: Within 48 hours of receipt.
- **Assessment & Triage**: Within 5 business days.
- **Remediation Release**: Depending on severity, within 14 business days.

---

## AI-Specific Security Guidelines

When documenting AI tools and MCP servers, maintainers and contributors must enforce the following security principles:

### 1. Model Context Protocol (MCP) Sandboxing
- MCP servers interacting with local filesystems or system commands must explicitly specify read-only boundaries by default.
- Root path access (`/`) or wildcard shell execution must be marked as high risk with explicit `[CAUTION]` alerts in documentation.

### 2. Secret & Credential Scanning
- Example configurations must never contain real API keys, private tokens, passwords, or sensitive environment variables.
- Always use placeholder syntax: `YOUR_API_KEY_HERE`, `YOUR_AUTH_TOKEN`.

### 3. Prompt Injection Defense
- Prompts that ingest untrusted user input or external web content must include guardrails instructing the assistant to ignore embedded system instruction overrides.

---

## Licensing of Security Advisories

All published security advisories and remediation documentation will be made available under the [CC BY 4.0](file:///LICENSES/CC-BY-4.0.txt) license.
