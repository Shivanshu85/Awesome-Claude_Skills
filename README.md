# AI-Skills-Library

[![License: CC BY 4.0](https://img.shields.io/badge/Docs_License-CC_BY_4.0-blue.svg)](file:///LICENSE)
[![License: MIT](https://img.shields.io/badge/Tools_License-MIT-yellow.svg)](file:///LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](file:///CONTRIBUTING.md)
[![Schema Version](https://img.shields.io/badge/Schema-Draft_07-informational.svg)](file:///schemas/metadata.schema.json)
[![Documentation Standard](https://img.shields.io/badge/Standard-v1.0-purple.svg)](file:///docs/standards.md)

> The canonical, production-grade documentation library for AI Coding Skills across every AI coding ecosystem.

---

## Table of Contents

- [Overview & Mission](#overview--mission)
- [Repository Philosophy](#repository-philosophy)
- [Visual Architecture Map](#visual-architecture-map)
- [Knowledge Categories](#knowledge-categories)
- [Skill Package Specification](#skill-package-specification)
- [Central Knowledge Infrastructure](#central-knowledge-infrastructure)
- [Navigation Guide](#navigation-guide)
- [Contribution Entry Point](#contribution-entry-point)
- [Licensing](#licensing)
- [Community & Governance](#community--governance)

---

## Overview & Mission

**AI-Skills-Library** is a curated, vendor-neutral knowledge base that documents AI Coding Skills in a standard, predictable, and maintainable format. 

As AI coding assistants, agents, and IDE integrations evolve, developers require an authoritative reference to understand **how to structure memory, handle context windows, design prompt systems, implement MCP servers, and orchestrate agent workflows**.

This repository is **documentation-first**. It contains no software implementations or tutorials; instead, it provides complete knowledge packages that enable developers and AI agents to discover, evaluate, and adopt AI coding skills effortlessly.

---

## Repository Philosophy

Designed with standards used by open-source foundations (OpenAI Cookbook, MDN, Kubernetes Docs, LangChain), this repository follows strict design principles:

1. **Knowledge First**: We optimize for developer learning and machine indexing, not file proliferation.
2. **README is the Product**: The `README.md` within each skill contains the entire narrative single source of truth. No split `installation.md` or `troubleshooting.md` files.
3. **Single Source of Truth**: PDFs (`<SkillName>-Guide.pdf`) are compiled exports derived automatically from Markdown. We never edit PDFs manually.
4. **Human vs. Machine Separation**: `README.md` serves human readers; `metadata.json` powers AI agents, CLI tools, search engines, and web APIs.
5. **Domain Taxonomy over Numbering**: Skills are organized into functional domain categories (`skills/memory/`, `skills/mcp/`) rather than fragile numeric prefixes (`01`, `02`).
6. **Diagrams as Code**: Workflows use Mermaid (`workflow.mmd`) as the canonical source, compiled to vector graphics (`workflow.svg`).
7. **Strict Consistency**: Every skill follows an identical section hierarchy, metadata schema, and Quick Facts layout.

---

## Visual Architecture Map

```
AI-Skills-Library/
│
├── README.md                          <- Root Landing Page & Central Index
├── LICENSE                            <- Dual Licensing Guide (CC BY 4.0 + MIT)
├── CONTRIBUTING.md                    <- Contributor Manual & Review Workflow
├── CODE_OF_CONDUCT.md                 <- Community Guidelines (Contributor Covenant v2.1)
├── SECURITY.md                        <- Security & Disclosure Policy
├── CHANGELOG.md                        <- Repository Release & Architectural History
├── .gitignore                         <- Clean Repository Exclusions
│
├── .github/                           <- Issue Forms & PR Templates
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── ISSUE_TEMPLATE/
│       ├── new_skill_request.yml
│       └── skill_update.yml
│
├── LICENSES/                          <- Full Legal Text Files
│   ├── CC-BY-4.0.txt
│   └── MIT.txt
│
├── docs/                              <- Repository Core Knowledge Infrastructure
│   ├── taxonomy.md                    <- Category Scope & Boundaries Definition
│   ├── glossary.md                    <- Single-source AI Terminology Definitions
│   └── standards.md                   <- Comprehensive Documentation Style Guide
│
├── schemas/                           <- Machine Schemas
│   └── metadata.schema.json           <- JSON Schema (Draft 07) for skill metadata
│
├── templates/                         <- Reusable Skill Generation Starters
│   ├── README.template.md             <- 28-Section Canonical README Template
│   ├── metadata.template.json         <- Validated Starter JSON Metadata
│   └── workflow.template.mmd          <- Standardized Mermaid Flowchart Template
│
└── skills/                            <- Categorized Knowledge Domain Packages
    ├── memory/                        <- Context retention, knowledge graphs, RAG memory
    ├── context/                       <- Context assembly, compression, windowing
    ├── prompt-engineering/            <- System prompts, sub-agent templates, guardrails
    ├── mcp/                           <- Model Context Protocol server specs & tools
    ├── automation/                    <- Autonomous task loops & CI/CD workflows
    ├── planning/                      <- Step-by-step task decomposition & plans
    ├── reasoning/                     <- Chain-of-thought, tree-of-thought protocols
    ├── developer-tools/               <- IDE extensions, CLI companions, linters
    ├── repository-intelligence/       <- Repo packing, AST analysis, symbol graphs
    ├── security/                      <- Prompt injection defence, secret scanning
    ├── testing/                       <- Test suite generation & verification loops
    ├── evaluation/                    <- LLM benchmark metrics & eval datasets
    ├── observability/                 <- Agent tracing, token metrics, telemetry
    ├── agent-frameworks/              <- Multi-agent orchestration architectures
    ├── ai-ides/                       <- Cursor, Claude Code, Windsurf integrations
    ├── productivity/                  <- Developer velocity & workflow acceleration
    └── code-generation/               <- Code synthesis, refactoring, boilerplate
```

---

## Knowledge Categories

The repository organizes skills across 17 domain categories. Detailed boundaries and inclusion rules are defined in [docs/taxonomy.md](file:///docs/taxonomy.md).

| Category | Description | Primary Focus | Landing Page |
| :--- | :--- | :--- | :--- |
| **Memory** | Long-term memory & knowledge representation | Graph memory, vector RAG, state persistence | [skills/memory/README.md](file:///skills/memory/README.md) |
| **Context** | Context window optimization & retrieval | Packing, truncation, token compression | [skills/context/README.md](file:///skills/context/README.md) |
| **Prompt Engineering** | System prompts & prompt architectures | Few-shot templates, instructions, guardrails | [skills/prompt-engineering/README.md](file:///skills/prompt-engineering/README.md) |
| **MCP** | Model Context Protocol servers & tools | Protocol tools, resources, prompts, server specs | [skills/mcp/README.md](file:///skills/mcp/README.md) |
| **Automation** | Autonomous execution loops & scripts | Task triggers, background processing | [skills/automation/README.md](file:///skills/automation/README.md) |
| **Planning** | Multi-step task decomposition | Architectural plans, milestone tracking | [skills/planning/README.md](file:///skills/planning/README.md) |
| **Reasoning** | Formal reasoning & decision strategies | Chain-of-thought, tree-of-thought, verification | [skills/reasoning/README.md](file:///skills/reasoning/README.md) |
| **Developer Tools** | CLI utilities & IDE extensions | Agent toolkits, dev server bridges | [skills/developer-tools/README.md](file:///skills/developer-tools/README.md) |
| **Repository Intelligence** | Codebase mapping & indexing | AST parsing, dependency graphs, repomix | [skills/repository-intelligence/README.md](file:///skills/repository-intelligence/README.md) |
| **Security** | AI security & safety protocols | Prompt injection protection, policy enforcement | [skills/security/README.md](file:///skills/security/README.md) |
| **Testing** | Automated test generation & validation | Unit test loops, dynamic assertions | [skills/testing/README.md](file:///skills/testing/README.md) |
| **Evaluation** | LLM benchmark & output assessment | Eval benchmarks, accuracy metrics | [skills/evaluation/README.md](file:///skills/evaluation/README.md) |
| **Observability** | Agent tracing & telemetry | Token counters, execution logging, span tracing | [skills/observability/README.md](file:///skills/observability/README.md) |
| **Agent Frameworks** | Multi-agent coordination patterns | Swarms, supervisor-agent topologies | [skills/agent-frameworks/README.md](file:///skills/agent-frameworks/README.md) |
| **AI IDEs** | IDE configuration & native skills | Cursor rules, Claude Code configs | [skills/ai-ides/README.md](file:///skills/ai-ides/README.md) |
| **Productivity** | Developer velocity acceleration | Workflow macros, boilerplate generators | [skills/productivity/README.md](file:///skills/productivity/README.md) |
| **Code Generation** | Code synthesis & refactoring patterns | Pattern transformation, migration templates | [skills/code-generation/README.md](file:///skills/code-generation/README.md) |

---

## Skill Package Specification

Every skill directory in this repository adheres to a strict 6-file specification:

```
skills/<category>/<skill-slug>/
├── README.md              <- Canonical 28-section single source of truth
├── metadata.json          <- Machine-readable metadata matching metadata.schema.json
├── workflow.mmd           <- Source Mermaid diagram (Input -> Processing -> Output)
├── workflow.svg           <- Rendered SVG diagram generated from workflow.mmd
├── <SkillName>-Guide.pdf  <- Automatically compiled PDF derived from README.md
└── LICENSE                <- Skill licensing reference
```

---

## Central Knowledge Infrastructure

To maintain consistency and eliminate repetitive definitions across thousands of skills, review our core reference documentation:

- 📖 **[Taxonomy Guide (`docs/taxonomy.md`)](file:///docs/taxonomy.md)**: Standardized criteria defining what belongs in each category.
- 📚 **[Glossary (`docs/glossary.md`)](file:///docs/glossary.md)**: Universal definitions for core concepts (RAG, MCP, Context Window, etc.).
- 📐 **[Documentation Standards (`docs/standards.md`)](file:///docs/standards.md)**: Style rules for Markdown, Quick Facts tables, Mermaid diagrams, and links.

---

## Navigation Guide

Browse the repository hierarchy seamlessly:

1. **Category Overview**: Navigate to any category landing page (e.g., [skills/memory/README.md](file:///skills/memory/README.md)) to explore skill indices, target audiences, and recommended learning orders.
2. **Individual Skill**: Each skill directory contains a self-contained `README.md` answering overview, problem statement, key features, architecture, installation, configuration, use cases, troubleshooting, and comparisons.
3. **Skill Navigation**: Every skill README features a navigation footer allowing step-by-step traversal:
   `← Previous Skill | Category Home | Next Skill →`

---

## Contribution Entry Point

We welcome contributions from developers, AI engineers, and researchers! Adding a new skill requires copying pre-built templates and filling in validated information:

1. Read [CONTRIBUTING.md](file:///CONTRIBUTING.md) for full submission guidelines.
2. Copy `templates/README.template.md`, `templates/metadata.template.json`, and `templates/workflow.template.mmd`.
3. Validate `metadata.json` against `schemas/metadata.schema.json`.
4. Submit a Pull Request using our [.github/PULL_REQUEST_TEMPLATE.md](file:///.github/PULL_REQUEST_TEMPLATE.md).

---

## Licensing

This repository uses a dual licensing model:

- **Documentation & Guides**: Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](file:///LICENSES/CC-BY-4.0.txt).
- **Schemas, Templates & Tooling**: Licensed under the [MIT License](file:///LICENSES/MIT.txt).

See [LICENSE](file:///LICENSE) for detailed license boundaries.

---

## Community & Governance

- 📜 **[Code of Conduct](file:///CODE_OF_CONDUCT.md)**: Principles governing community interactions.
- 🔒 **[Security Policy](file:///SECURITY.md)**: Security reporting and disclosure procedures.
- 📜 **[Changelog](file:///CHANGELOG.md)**: Track version history and repository updates.
