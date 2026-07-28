# Documentation & Writing Standards Guide

This guide establishes the mandatory formatting, writing, architectural, and structural standards for all documentation in **Awesome-Claude_Skills**.

Consistency across thousands of tools is paramount. Every tool README, category index, and template must adhere strictly to these specifications.

---

## 1. Core Documentation Rules

1. **Single Source of Truth**: All human narrative documentation for a tool belongs in its single `README.md`. Creating split files (e.g. `installation.md`, `architecture.md`, `benchmarks.md`) is strictly forbidden.
2. **Master README → Automated PDF**: `Tool-Guide.pdf` is compiled automatically from `README.md`. Never edit PDF files manually.
3. **Machine vs. Human Separation**: `metadata.json` exists for automation, search engines, and AI agents. `README.md` exists for human software engineers. Do not duplicate narrative prose between them.
4. **Glossary Utilization**: Do not redefine core terms (RAG, MCP, Context Window, Prompt Cache, AST Parsing). Link directly to entries in [docs/glossary.md](file:///docs/glossary.md).
5. **Evidence-Based Content**: Never invent quantitative benchmark numbers or fake metrics. Use qualitative impact ratings (Low, Medium, High, Very High) unless official, reproducible benchmark data is cited.

---

## 2. Heading Hierarchy & Structure

Every tool `README.md` MUST follow the exact 28-section hierarchy defined in `templates/README.template.md`:

```markdown
# {{TOOL_NAME}}

## Quick Facts
## Overview
## Problem Solved
## Why Use It
## When To Use
## When NOT To Use
## Architecture Overview
## Workflow
## Installation
## Configuration
## Compatibility Table
## Basic Example
## Advanced Example
## Use Cases
## Performance Notes
## Comparison Table
## Advantages
## Limitations
## Best Practices
## Common Mistakes
## Troubleshooting
## Security Considerations
## Related Tools
## Official Repository
## Official Documentation
## References
## FAQ
## License & Contributors
```

---

## 3. Qualitative Impact Ratings

In both `Quick Facts` and `metadata.json`, use standard qualitative ratings instead of invented metrics:

- **Token Saving Potential**: `Low`, `Medium`, `High`, `Very High`, `N/A`
- **Context Improvement**: `Low`, `Medium`, `High`, `Very High`, `N/A`
- **Developer Productivity**: `Low`, `Medium`, `High`, `Very High`, `N/A`
- **Reasoning Improvement**: `Low`, `Medium`, `High`, `Very High`, `N/A`
- **Setup Complexity**: `Low`, `Medium`, `High`, `Very High`, `N/A`

> [!WARNING]
> Never invent exact percentage claims like "Reduces cost by exactly 78.4%" unless quoting official, published peer-reviewed research papers cited in the References section.

---

## 4. Compatibility Table Rules

The Compatibility Table MUST list all major AI coding environments:

```markdown
| Environment | Supported | Notes |
| :--- | :---: | :--- |
| **Claude Code** | Yes | Full native support via CLI and MCP |
| **Cursor** | Yes | Supported via `.cursorrules` and MCP |
| **Codex** | Yes | Supported via API payload injection |
| **Gemini CLI** | Yes | Supported via CLI transport |
| **Continue** | Yes | Supported via config.json extension |
| **Roo Code** | Yes | Supported via MCP tools |
| **VS Code** | Yes | Supported via extension bridge |
```

---

## 5. Mermaid Diagram Rules

- Store source Mermaid diagram in `workflow.mmd`.
- Render vector SVG export to `workflow.svg`.
- Always enclose node labels in quotes if they contain special characters: `A["Label (Details)"]`.
- Use top-down (`graph TD`) or sequence (`sequenceDiagram`) layouts.

---

## 6. Relative File Link Conventions

All internal links between Markdown documents MUST use standard Markdown syntax with relative paths:

- **Root Landing Page**: `[Root README](file:///README.md)`
- **Category Index**: `[Memory Systems](file:///skills/memory/README.md)`
- **Glossary Entry**: `[RAG](file:///docs/glossary.md#rag)`
- **Taxonomy Guide**: `[Taxonomy Guide](file:///docs/taxonomy.md)`

Do not wrap file link text in code backticks, as backticks break markdown hyperlink rendering in GitHub.
