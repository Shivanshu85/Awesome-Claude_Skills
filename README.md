<p align="center">
  <img src="assets/banner.png" alt="Awesome-Claude_Skills Banner" width="100%" />
</p>

<h1 align="center">Awesome-Claude_Skills</h1>

<p align="center">
  <strong>The canonical open-source documentation library for AI context optimization, token economy, memory systems, MCP servers, prompt engineering, and developer productivity tools.</strong>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/Docs_License-CC_BY_4.0-blue.svg" alt="License: CC BY 4.0"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/Tools_License-MIT-yellow.svg" alt="License: MIT"></a>
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="schemas/metadata.schema.json"><img src="https://img.shields.io/badge/Schema-Draft_07-informational.svg" alt="Schema Version"></a>
  <a href="docs/standards.md"><img src="https://img.shields.io/badge/Standard-v1.0-purple.svg" alt="Documentation Standard"></a>
</p>

---

## 📖 Overview

**Awesome-Claude_Skills** is a documentation-first knowledge base dedicated to optimizing AI coding assistants, agents, and IDE integrations. Rather than acting as an arbitrary tool list or commercial directory, this repository provides standardized, vendor-neutral documentation for open-source AI optimization tools across 13 core domain categories.

---

## 🎯 Mission

> Build the world's best curated documentation library for AI context optimization, token economy, memory systems, Model Context Protocol (MCP) servers, prompt engineering, codebase intelligence, and developer productivity techniques that make AI coding assistants cheaper, faster, smarter, and more accurate.

This repository exists to help developers, software engineers, AI engineers, and prompt engineers discover proven open-source solutions to:
- Reduce token consumption and API costs
- Improve context quality and long-context window handling
- Implement persistent agent memory and knowledge graphs
- Integrate standardized Model Context Protocol (MCP) servers
- Enforce prompt security, evaluation, and regression testing

---

## 💡 Philosophy

This repository adheres to six core architectural principles:

1. **Documentation-First**: This is a documentation repository, not a code library or file collector.
2. **Single Source of Truth**: Every tool is documented in a single `README.md` file adhering to a strict 28-section standard.
3. **Category Delegation**: Tool rankings, comparisons, GitHub star counts, maintenance statuses, and installation guides belong exclusively inside category `README.md` files and individual tool pages — not in the root landing page.
4. **No Invented Tools**: Only existing, verified open-source projects are documented. Fake or placeholder tool entries are strictly forbidden.
5. **Problem-First Navigation**: Navigation directs users to domain categories based on technical bottlenecks.
6. **Evidence-Based Content**: Documentation relies on verifiable official documentation and technical facts rather than marketing claims.

---

## 📚 Skills Library

Explore open-source AI coding optimization tools across our 13 domain categories. Click any category to view its complete tool index, head-to-head comparisons, and learning guide:

- 🧠 **[Memory](skills/memory/README.md)**: Persistent memory systems, temporal knowledge graphs, and multi-session RAG state retention.
- 📦 **[Context](skills/context/README.md)**: Context window management, token payload packing, and dynamic documentation assembly.
- ⚡ **[Context Compression](skills/context-compression/README.md)**: SLM-based prompt compression, token pruning algorithms, and context truncation.
- 💰 **[Token Optimization](skills/token-optimization/README.md)**: Token economy, prompt whitespace/AST stripping, and API cost reduction techniques.
- ✍️ **[Prompt Engineering](skills/prompt-engineering/README.md)**: System prompt frameworks, structured instruction templates, and output guardrails.
- 🔍 **[Codebase Intelligence](skills/codebase-intelligence/README.md)**: Repository packing, AST parsing, symbol graph extraction, and codebase maps.
- 🔌 **[Model Context Protocol (MCP)](skills/mcp/README.md)**: Standardized MCP servers for local files, git, APIs, web fetching, and reasoning.
- 🚀 **[Developer Productivity](skills/developer-productivity/README.md)**: Developer workflow acceleration, CLI companions, and automation macros.
- 🔄 **[Agent Workflows](skills/agent-workflows/README.md)**: Multi-step reasoning protocols, sequential thinking, reflection, and ReAct loops.
- 🛡️ **[Security](skills/security/README.md)**: Prompt injection defense, MCP tool permission sandboxing, and secret scanning guardrails.
- 📊 **[Evaluation](skills/evaluation/README.md)**: LLM quality benchmarks, prompt accuracy scoring, and evaluation pipelines.
- 🧪 **[Testing](skills/testing/README.md)**: Prompt regression test suites, dynamic assertion libraries, and AI test automation.
- 🔭 **[Observability](skills/observability/README.md)**: Assistant telemetry, token usage analytics, span tracing, and execution logging.

---

## 🏷 Browse by Problem

Find the appropriate category based on your immediate engineering bottleneck:

| Technical Problem / Need | Go To Category |
| :--- | :--- |
| **Reduce Token Usage** | [Context Compression](skills/context-compression/README.md) |
| **Reduce API Costs** | [Token Optimization](skills/token-optimization/README.md) |
| **Improve Memory & State Retention** | [Memory](skills/memory/README.md) |
| **Understand Large Codebases** | [Codebase Intelligence](skills/codebase-intelligence/README.md) |
| **Connect External Tools & APIs** | [Model Context Protocol (MCP)](skills/mcp/README.md) |
| **Improve Prompt Design & Schemas** | [Prompt Engineering](skills/prompt-engineering/README.md) |
| **Improve AI Reasoning & Planning** | [Agent Workflows](skills/agent-workflows/README.md) |
| **Secure Tool Usage & Guardrails** | [Security](skills/security/README.md) |
| **Evaluate Prompt Quality & Benchmarks** | [Evaluation](skills/evaluation/README.md) |
| **Test AI Workflows & Assertions** | [Testing](skills/testing/README.md) |
| **Observe Token Usage & Telemetry** | [Observability](skills/observability/README.md) |

---

## 📂 Repository Structure

```text
Awesome-Claude_Skills/
│
├── README.md                          <- Root Landing Page & Central Index
├── LICENSE                            <- Dual Licensing Guide (CC BY 4.0 + MIT)
├── CONTRIBUTING.md                    <- Contributor Manual & Review Workflow
├── CODE_OF_CONDUCT.md                 <- Community Guidelines (Contributor Covenant v2.1)
├── SECURITY.md                        <- Security & Disclosure Policy
├── CHANGELOG.md                       <- Repository Release & Architectural History
├── .gitignore                         <- Clean Repository Exclusions
│
├── .github/
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── ISSUE_TEMPLATE/
│       ├── new_tool_request.yml
│       └── tool_update.yml
│
├── LICENSES/
│   ├── CC-BY-4.0.txt
│   └── MIT.txt
│
├── assets/
│   └── banner.png
│
├── docs/
│   ├── taxonomy.md
│   ├── glossary.md
│   └── standards.md
│
├── schemas/
│   └── metadata.schema.json
│
├── templates/
│   ├── README.template.md
│   ├── metadata.template.json
│   └── workflow.template.mmd
│
└── skills/
    ├── memory/
    ├── context/
    ├── context-compression/
    ├── token-optimization/
    ├── prompt-engineering/
    ├── codebase-intelligence/
    ├── mcp/
    ├── developer-productivity/
    ├── agent-workflows/
    ├── security/
    ├── evaluation/
    ├── testing/
    └── observability/
```

### Directory Responsibilities

- **`skills/`**: Contains every documented AI optimization tool organized by category.
- **`docs/`**: Core repository knowledge infrastructure, including documentation standards, domain taxonomy, and glossary.
- **`templates/`**: Starter templates (`README.template.md`, `metadata.template.json`, `workflow.template.mmd`) used to document every tool.
- **`schemas/`**: Machine-readable JSON Schema (`metadata.schema.json`) for tool indexing and AI agent validation.
- **`assets/`**: Repository visual assets, branding, and diagrams.
- **`.github/`**: Contribution workflow automation, issue forms, and PR templates.

### Individual Tool Specifications

Every tool documented under `skills/<category>/<tool-slug>/` adheres strictly to a standardized 5-file specification:

```text
skills/<category>/<tool-slug>/
│
├── README.md              <- Authoritative 28-section documentation
├── metadata.json          <- Machine-readable metadata schema
├── workflow.mmd           <- Source Mermaid diagram
├── workflow.svg           <- Rendered vector SVG diagram
└── LICENSE                <- Skill-level license file
```

Detailed rankings, tool comparisons, stars, maintenance statuses, and learning orders are maintained inside each category's [`README.md`](skills/memory/README.md) file.

---

## 📏 Repository Standards

Review our core standards before reading or contributing tool documentation:

- 📐 **[Documentation Standards](docs/standards.md)**: Rules for writing, section hierarchy, and qualitative impact ratings.
- 📖 **[Category Taxonomy Guide](docs/taxonomy.md)**: Category definitions, boundaries, and inclusion rules.
- 📚 **[AI Optimization Glossary](docs/glossary.md)**: Universal definitions for RAG, MCP, Context Window, Prompt Cache, AST Parsing, and Sequential Thinking.
- 🤖 **[Metadata Schema](schemas/metadata.schema.json)**: Draft 07 JSON Schema for machine indexing.
- 📑 **[README Template](templates/README.template.md)**: Mandatory 28-section starter template for tool pages.

---

## 🤝 Contributing

We welcome contributions for open-source AI optimization tools and MCP servers!

1. Select the appropriate category under `skills/<category>/`.
2. Copy `templates/README.template.md` and `templates/metadata.template.json` to your tool directory.
3. Validate `metadata.json` against `schemas/metadata.schema.json`.
4. Submit a Pull Request following [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md).

For complete submission criteria and writing guidelines, read [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 🗺 Roadmap & FAQ

### Roadmap

- [x] Establish canonical 13-category architecture and schema standards.
- [x] Release Draft 07 JSON Schema and 28-section tool documentation templates.
- [ ] Expand category indexes with comprehensive open-source tool documentation.
- [ ] Deploy automated CI workflows for link checking and SVG/PDF validation.
- [ ] Launch web index site powered by `metadata.json` schemas.

### FAQ

**Q: Is this repository an AI coding assistant software library?**  
A: No. **Awesome-Claude_Skills** is a documentation-first repository. It provides standardized guides, schemas, diagrams, and metadata for open-source AI optimization tools.

**Q: Why are tool rankings and star counts omitted from the root README?**  
A: To maintain a clean, scalable landing page. Tool comparisons, star metrics, and recommendation tables belong inside category `README.md` files where they can be evaluated in domain context.

**Q: Can proprietary tools be documented?**  
A: No. We exclusively document open-source projects, open protocols (like MCP), and open standards.

---

## 📄 License

This repository uses a dual licensing model:

- **Documentation & Content**: Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSES/CC-BY-4.0.txt).
- **Schemas, Templates & Tooling**: Licensed under the [MIT License](LICENSES/MIT.txt).

See [LICENSE](LICENSE) for full licensing boundaries.
