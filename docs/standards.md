# Documentation & Writing Standards Guide

This guide establishes the mandatory formatting, writing, architectural, and structural standards for all documentation in **Awesome-Claude_Skills**.

Consistency is paramount. Every skill README, category guide, and template must adhere to these specifications.

---

## 1. Core Documentation Rules

1. **Single Source of Truth**: All human documentation for a skill belongs in its single `README.md`. Creating split files (e.g. `installation.md`, `architecture.md`, `benchmarks.md`) is forbidden.
2. **Master README → Automated PDF**: `Guide.pdf` (or `<SkillName>-Guide.pdf`) is compiled automatically from `README.md`. Never edit PDFs manually.
3. **Machine vs. Human Separation**: `metadata.json` exists for automation, search, and AI agents. `README.md` exists for human developers. Do not duplicate narrative prose between them.
4. **Glossary Utilization**: Do not redefine core terms (RAG, MCP, Context Window, Prompt Cache). Link directly to entries in [docs/glossary.md](file:///docs/glossary.md).
5. **Factual Integrity**: Never invent benchmark numbers or unverified claims. If official benchmarks exist, cite them; otherwise explicitly state that no official benchmark exists under Performance Notes.

---

## 2. Heading Hierarchy & Structure

All skill README files must follow the exact 28-section hierarchy defined in [templates/README.template.md](file:///templates/README.template.md):

```markdown
# <Skill Name>

[Quick Facts Table]

## Overview
## Problem Statement
## Why this Skill Exists
## When Should You Use It
## When Should You NOT Use It
## Key Features
## Architecture Overview
## Workflow Overview
## Installation
## Configuration
## Supported Platforms
## Supported AI Models
## Supported IDEs
## Usage
### Basic Example
### Advanced Example
## Real-World Use Cases
## Performance Notes
## Comparison Table
## Advantages
## Limitations
## Best Practices
## Common Mistakes
## Troubleshooting
## Security Considerations
## Related Skills
## Official References
## FAQ
## License & Contributors
```

- **Rules**:
  - Top title must be a single `#` heading.
  - Primary sections must use `##`.
  - Subsections must use `###`. Do not skip heading levels (e.g., `#` to `###`).

---

## 3. Quick Facts Table Standard

Every skill `README.md` must begin with a standardized Quick Facts table immediately below the main `# <Skill Name>` heading:

| Property | Value |
| :--- | :--- |
| **Category** | `[Category Name](file:///skills/<category>/README.md)` |
| **Difficulty** | Beginner \| Intermediate \| Advanced |
| **Skill Type** | Memory System \| MCP Server \| Prompt Pattern \| Tooling \| Protocol |
| **Works With** | Claude Code, Cursor, Windsurf, Custom Agents |
| **Installation** | `pip install ...` \| `npm install ...` \| Docker \| N/A |
| **Maintenance Status** | Active \| Maintained \| Experimental |
| **Official Resource** | Yes ([Link](url)) \| Community |
| **License** | MIT \| Apache 2.0 \| CC BY 4.0 |
| **Last Updated** | YYYY-MM-DD |
| **Supported Models** | Claude 3.5 Sonnet, GPT-4o, Gemini 1.5 Pro |
| **Supported IDEs** | Cursor, Claude Code, VS Code |
| **Estimated Learning Time** | XX minutes |
| **Core Purpose** | Single-sentence explanation of what this skill achieves. |

---

## 4. Markdown Style & Formatting

- **Code Blocks**: Specify syntax language for all code blocks (`bash`, `json`, `yaml`, `python`, `typescript`, `mermaid`).
- **Callouts**: Use standard GitHub-style alerts sparingly for emphasis:
  > [!NOTE]
  > Useful background context or implementation detail.

  > [!IMPORTANT]
  > Critical step or requirement.

  > [!WARNING]
  > Potential issue, security risk, or breaking change.
- **Tone**: Formal, clear, professional, objective. Avoid marketing hype, excessive exclamation marks, or gratuitous emojis.
- **File Links**: Use relative file links with standard GitHub Markdown syntax.

---

## 5. Mermaid Workflow Diagram Standards

- **Source File**: `workflow.mmd`
- **Rendered Output**: `workflow.svg`
- **Layout**: Top-Down (`TD`)
- **Flow Pattern**: Must clearly depict:
  `Input Layer -> Processing Engine -> Core Components -> Output Handler -> Final Result`
- **Example Template**:
  ```mermaid
  graph TD
      A[Input Request] --> B[Processing Engine]
      B --> C[Core Components]
      C --> D[Output Handler]
      D --> E[Final Result]
  ```

---

## 6. Metadata JSON Standards

- Must validate clean against `schemas/metadata.schema.json`.
- Must contain all mandatory fields: `name`, `slug`, `description`, `category`, `tags`, `difficulty`, `license`, `official`, `official_repository`, `supported_models`, `supported_platforms`, `supported_ides`, `version`, `status`, `maintainer`, `last_updated`.

---

## 7. Link & Navigation Validation

- All README files must end with the navigation footer:
  `← [Previous Skill](file://...) | [Category Home](file://...) | [Next Skill](file://...)`
- All relative file links must point to existing files in the repository.
- External URLs must point to official documentation or source repositories.
