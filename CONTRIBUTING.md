# Contributing to Awesome-Claude_Skills

Thank you for your interest in contributing to **Awesome-Claude_Skills**! This repository is designed to be the world's premier, canonical documentation library for open-source AI context optimization, token economy, memory systems, MCP servers, prompt engineering, and developer productivity tools.

To maintain professional quality, long-term sustainability, and technical accuracy, every contribution must adhere strictly to these guidelines.

---

## Table of Contents

- [Repository Philosophy & Rules](#repository-philosophy--rules)
- [What Can Be Contributed](#what-can-be-contributed)
- [Folder & Slug Naming Rules](#folder--slug-naming-rules)
- [The 7-File Tool Specification](#the-7-file-tool-specification)
- [28-Section README Template Rules](#28-section-readme-template-rules)
- [Metadata Schema & Validation](#metadata-schema--validation)
- [Mermaid Diagram Guidelines](#mermaid-diagram-guidelines)
- [Writing Style & Content Guidelines](#writing-style--content-guidelines)
- [Pull Request Submission Checklist](#pull-request-submission-checklist)
- [Code of Conduct](#code-of-conduct)

---

## Repository Philosophy & Rules

1. **Quality over Quantity**: We only document important, useful, trusted open-source tools.
2. **Documentation First**: This is a documentation repository. Do not commit software source code, binaries, or random scripts.
3. **Single Source of Truth**: The tool's `README.md` is the authoritative documentation source. Never create extra markdown files (e.g. `installation.md` or `benchmarks.md`).
4. **No Duplicate Documentation**: Keep prose inside `README.md`. Keep `metadata.json` compact and machine-oriented.
5. **Consistency over Creativity**: Every documented tool follows the exact same structure.
6. **Evidence-Based Content**: Never invent benchmark scores, fake numbers, or marketing hype. Use official documentation and verifiable facts.

---

## What Can Be Contributed

We welcome contributions for open-source tools, MCP servers, and protocols that directly improve:

- **Memory Systems**: Persistent agent state, knowledge graph RAG, entity memory.
- **Context Management**: Context windows, packing, injection, dynamic windowing.
- **Context Compression**: LLMLingua, prompt compression, token pruning.
- **Token Optimization**: Cost reduction, whitespace pruning, input economy.
- **Prompt Engineering**: System prompt frameworks, guardrails, structured outputs.
- **Codebase Intelligence**: AST parsing, repository packing, symbol graph search.
- **MCP Servers**: Standardized Model Context Protocol servers for files, git, databases, and APIs.
- **Developer Productivity**: Developer workflow acceleration, CLI companions, IDE bindings.
- **Agent Workflows**: Sequential thinking, planning, reflection, ReAct loops.
- **Security**: Prompt injection defense, sandboxing, permission controls.
- **Evaluation & Testing**: LLM evals, prompt regression suites, accuracy metrics.
- **Observability**: Telemetry, span tracing, token usage analytics.

### What Must NEVER Be Contributed

Do **NOT** submit:
- AI IDEs or generic agent frameworks
- Closed-source / proprietary tools without open standards
- Image generation, voice AI, or general chatbots
- Fine-tuning libraries, raw datasets, or model weights
- Unverified, subjective prompt lists without tooling

---

## Folder & Slug Naming Rules

Every tool must be located within one of the 13 canonical category directories under `skills/`:

```
skills/<category>/<tool-slug>/
```

- **Category Name**: Must match an existing category directory (e.g., `skills/memory/`, `skills/mcp/`).
- **Tool Slug**: Must use lowercase `kebab-case` matching the tool name (e.g., `filesystem-mcp`, `graphiti`, `repomix`).

---

## The 7-File Tool Specification

Every tool directory MUST contain EXACTLY these 7 files. No more, no less:

```
skills/<category>/<tool-slug>/
├── README.md              <- Canonical 28-section single source of truth
├── metadata.json          <- Machine-readable metadata matching metadata.schema.json
├── workflow.mmd           <- Source Mermaid diagram (Input -> Processing -> Output)
├── workflow.svg           <- Rendered SVG diagram derived from workflow.mmd
├── <ToolName>-Guide.pdf   <- Automatically compiled PDF derived from README.md
└── LICENSE                <- Skill-level license file
```

---

## 28-Section README Template Rules

Every tool `README.md` must be created by copying `templates/README.template.md` and completing all 28 mandatory sections:

1. **Overview**: High-level explanation of the tool and its significance.
2. **Quick Facts**: Mandatory table summarizing Category, Primary Benefit, Difficulty, Works With, License, Official Repository, Maintenance Status, Last Updated, Learning Time, Setup Complexity, Token Saving Potential, Context Improvement, Memory Support.
3. **Problem Solved**: Developer friction or technical bottleneck when this tool is NOT used.
4. **Why Use It**: Design intent and technical architectural advantages.
5. **When To Use**: Clear indicators when this tool is the right choice.
6. **When NOT To Use**: Explicit anti-patterns and scenarios where the tool should be avoided.
7. **Architecture Overview**: Deep-dive explanation of component interaction.
8. **Workflow**: Step-by-step lifecycle flow from input to output.
9. **Installation**: Exact package manager or CLI commands to install.
10. **Configuration**: Environment variables, config files, or settings.
11. **Compatibility Table**: Support status for Claude Code, Cursor, Codex, Gemini CLI, Continue, Roo Code, VS Code, and others.
12. **Basic Example**: Clean, minimal copy-paste example.
13. **Advanced Example**: Production-grade complex configuration example.
14. **Use Cases**: Real-world software engineering workflows.
15. **Performance Notes**: Token reduction impact, memory footprint, and speed notes.
16. **Comparison Table**: Feature comparison against alternative tools.
17. **Advantages**: List of key technical strengths.
18. **Limitations**: Known constraints or trade-offs.
19. **Best Practices**: Recommended engineering patterns.
20. **Common Mistakes**: Misconfigurations to avoid.
21. **Troubleshooting**: Diagnostic steps for common failure modes.
22. **Security Considerations**: Sandboxing, permissions, data privacy, and secret handling.
23. **Related Tools**: Links to complementary skills in the repository.
24. **Official Repository**: Direct link to the open-source repository.
25. **Official Documentation**: Direct link to official docs.
26. **References**: Citations, papers, or official announcements.
27. **FAQ**: Frequently asked questions.
28. **License & Contributors**: Licensing details and contributor acknowledgments.

---

## Metadata Schema & Validation

`metadata.json` must validate cleanly against `schemas/metadata.schema.json`.

- **Do Not Duplicate Narrative**: Keep descriptions concise.
- **Required Fields**: `name`, `slug`, `description`, `category`, `tags`, `difficulty`, `license`, `official`, `official_repository`, `supported_models`, `supported_platforms`, `supported_ides`, `version`, `status`, `maintainer`, `last_updated`.
- **Status Values**: Must be one of `"Active"`, `"Limited Maintenance"`, `"Archived"`.

---

## Mermaid Diagram Guidelines

- `workflow.mmd` is the canonical source for architecture flowcharts.
- Use clean `graph TD` or `sequenceDiagram` syntax.
- Quote all node labels containing special characters: `id["Label (Details)"]`.
- Compile `workflow.mmd` to vector graphic `workflow.svg`.

---

## Writing Style & Content Guidelines

- **Technical & Neutral**: Write for senior developers and systems engineers. Avoid marketing jargon or hype words ("revolutionary", "game-changing").
- **Evidence-Based**: Only document verified features. Never fabricate benchmark scores. Use qualitative ratings (Low, Medium, High, Very High) when empirical numbers are unavailable.
- **Link Integrity**: Use relative Markdown links for all internal files: `[standards.md](file:///docs/standards.md)`.

---

## Pull Request Submission Checklist

Before submitting a PR, verify:

- [ ] Tool is placed in one of the 13 canonical categories under `skills/<category>/<tool-slug>/`.
- [ ] Directory contains EXACTLY the 7 required files (`README.md`, `metadata.json`, `workflow.mmd`, `workflow.svg`, `Tool-Guide.pdf`, `LICENSE`).
- [ ] `README.md` contains all 28 mandatory template sections.
- [ ] `metadata.json` passes schema validation against `schemas/metadata.schema.json`.
- [ ] All relative file links use the `file:///` format and point to valid files.
- [ ] Qualitative impact ratings are used instead of invented benchmark scores.
- [ ] PR description specifies the tool name, category, and official repository.

---

## Code of Conduct

All contributors are expected to uphold our [Code of Conduct](file:///CODE_OF_CONDUCT.md) (Contributor Covenant v2.1).
