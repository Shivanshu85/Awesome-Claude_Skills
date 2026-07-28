# {{TOOL_NAME}}

<p align="center">
  <strong>{{SHORT_TAGLINE}}</strong>
</p>

---

## Quick Facts

| Property | Value |
| :--- | :--- |
| **Category** | [{{CATEGORY_NAME}}](file:///skills/{{CATEGORY_SLUG}}/README.md) |
| **Primary Benefit** | {{PRIMARY_BENEFIT}} |
| **Difficulty** | {{DIFFICULTY}} |
| **Works With** | {{WORKS_WITH}} |
| **License** | {{LICENSE}} |
| **Official Repository** | [{{OFFICIAL_REPO_NAME}}]({{OFFICIAL_REPO_URL}}) |
| **Maintenance Status** | {{MAINTENANCE_STATUS}} |
| **Last Updated** | {{LAST_UPDATED}} |
| **Estimated Learning Time** | {{LEARNING_TIME}} |
| **Setup Complexity** | {{SETUP_COMPLEXITY}} |
| **Token Saving Potential** | {{TOKEN_SAVING_RATING}} |
| **Context Improvement** | {{CONTEXT_IMPROVEMENT_RATING}} |
| **Memory Support** | {{MEMORY_SUPPORT_RATING}} |

---

## Overview

[Provide a clear, high-level explanation of the tool, what problem it solves, and its significance in AI coding workflows. Link to core terms in [docs/glossary.md](file:///docs/glossary.md) such as [RAG](file:///docs/glossary.md#rag), [MCP](file:///docs/glossary.md#mcp), or [Context Window](file:///docs/glossary.md#context-window).]

---

## Problem Solved

[Describe the technical bottleneck, developer friction, excessive token cost, or AI limitation that exists when this tool is NOT used.]

---

## Why Use It

[Explain the design intent, technical architecture advantages, and specific benefits that make this tool effective for AI coding assistants.]

---

## When To Use

- [Scenario 1: e.g. When processing large repositories that exceed context limits]
- [Scenario 2: e.g. When integrating external APIs with Claude Code or Cursor]
- [Scenario 3: e.g. When operating under strict monthly LLM API budgets]

---

## When NOT To Use

- [Anti-pattern 1: e.g. Do not use for small, single-file scripts where overhead is unnecessary]
- [Anti-pattern 2: e.g. Do not use if proprietary data policy forbids external indexing]

---

## Architecture Overview

[Provide a deep-dive explanation of component interaction. Describe how the tool processes inputs, handles AST parsing or token pruning, and interfaces with the LLM assistant.]

---

## Workflow

Below is the step-by-step execution lifecycle for {{TOOL_NAME}}:

```mermaid
graph TD
    A[Input: User Prompt / Codebase] --> B[Processing: {{TOOL_NAME}} Engine]
    B --> C[Optimization: Token Pruning / Context Assembly]
    C --> D[Output: Efficient Context / Tool Response to Assistant]
```

*(See [workflow.svg](file:///skills/{{CATEGORY_SLUG}}/{{TOOL_SLUG}}/workflow.svg) for vector export).*

---

## Installation

```bash
# Install via package manager or CLI tool
{{INSTALLATION_COMMAND}}
```

---

## Configuration

Provide environment variables or configuration file setups:

```json
{
  "setting": "value"
}
```

---

## Compatibility Table

| Environment | Supported | Notes |
| :--- | :---: | :--- |
| **Claude Code** | Yes / No | {{CLAUDE_CODE_NOTES}} |
| **Cursor** | Yes / No | {{CURSOR_NOTES}} |
| **Codex** | Yes / No | {{CODEX_NOTES}} |
| **Gemini CLI** | Yes / No | {{GEMINI_NOTES}} |
| **Continue** | Yes / No | {{CONTINUE_NOTES}} |
| **Roo Code** | Yes / No | {{ROO_CODE_NOTES}} |
| **VS Code** | Yes / No | {{VS_CODE_NOTES}} |

---

## Basic Example

```python
# Minimal working example demonstrating core functionality
def basic_example():
    pass
```

---

## Advanced Example

```python
# Production-grade example showing advanced options and integrations
def advanced_example():
    pass
```

---

## Use Cases

1. **Use Case 1**: [Description of practical engineering workflow]
2. **Use Case 2**: [Description of practical engineering workflow]

---

## Performance Notes

- **Token Impact**: [Describe qualitative token savings e.g. High / Very High]
- **Inference Speed**: [Describe latency impact]
- **Memory Footprint**: [Describe resource utilization]

---

## Comparison Table

| Feature | {{TOOL_NAME}} | Alternative Tool A | Alternative Tool B |
| :--- | :--- | :--- | :--- |
| **Token Economy** | High | Medium | Low |
| **Setup Complexity** | Low | High | Medium |
| **Open Source** | Yes | Yes | No |

---

## Advantages

- **Advantage 1**: Technical strength or efficiency gain.
- **Advantage 2**: Integration simplicity.

---

## Limitations

- **Limitation 1**: Known constraint or trade-off.
- **Limitation 2**: Dependency requirements.

---

## Best Practices

1. **Best Practice 1**: Recommended configuration or setup pattern.
2. **Best Practice 2**: Usage guideline.

---

## Common Mistakes

1. **Mistake 1**: Common misconfiguration to avoid.
2. **Mistake 2**: Misinterpretation of tool boundaries.

---

## Troubleshooting

| Issue / Error | Cause | Resolution |
| :--- | :--- | :--- |
| `Error: Connection Refused` | MCP server transport offline | Verify stdio/SSE server process is active |

---

## Security Considerations

- **Permissions**: Describe required file or network permissions.
- **Secret Protection**: Ensure API keys and credentials are never exposed.

---

## Related Tools

- 🔗 [Complementary Tool 1](file:///skills/{{CATEGORY_SLUG}}/README.md): Description of relation.
- 🔗 [Complementary Tool 2](file:///skills/{{CATEGORY_SLUG}}/README.md): Description of relation.

---

## Official Repository

- 📦 **GitHub Repository**: [{{OFFICIAL_REPO_URL}}]({{OFFICIAL_REPO_URL}})

---

## Official Documentation

- 📖 **Official Docs**: [{{OFFICIAL_DOCS_URL}}]({{OFFICIAL_DOCS_URL}})

---

## References

1. Author / Project Announcement, "[Title of Article or Paper]({{REFERENCE_URL}})", Year.

---

## FAQ

**Q: Is {{TOOL_NAME}} free and open-source?**  
A: Yes, licensed under {{LICENSE}}.

---

## License & Contributors

- **License**: {{LICENSE}}
- **Contributors**: {{CONTRIBUTORS}}

---

← [{{CATEGORY_NAME}} Index](file:///skills/{{CATEGORY_SLUG}}/README.md) | [Root README](file:///README.md) →
