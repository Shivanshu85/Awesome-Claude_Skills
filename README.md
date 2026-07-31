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

**Awesome-Claude_Skills** is a documentation-first repository containing curated open-source tools for AI coding optimization. It provides standardized, evidence-based documentation for Model Context Protocol (MCP) servers, persistent memory systems, prompt compression algorithms, codebase intelligence tools, and prompt engineering frameworks across all 13 canonical domain categories.

---

## 📚 Skills Library

### 🧠 [Memory](skills/memory/)



---

### 📦 [Context](skills/context/)


---

### ⚡ [Context Compression](skills/context-compression/)


---

### 💰 [Token Optimization](skills/token-optimization/)

---

### ✍️ [Prompt Engineering](skills/prompt-engineering/)


---

### 🔍 [Codebase Intelligence](skills/codebase-intelligence/)


---

### 🔌 [Model Context Protocol (MCP)](skills/mcp/)


---

### 🚀 [Developer Productivity](skills/developer-productivity/)

---

### 🔄 [Agent Workflows](skills/agent-workflows/)


---

### 🛡️ [Security](skills/security/)


---

### 📊 [Evaluation](skills/evaluation/)


---

### 🧪 [Testing](skills/testing/)


---

### 🔭 [Observability](skills/observability/)


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
- [x] Launch standardized 28-section tool documentation templates.
- [ ] Expand tool documentation coverage across all 13 categories to 100+ open-source tools.
- [ ] Implement automated CI workflows for link checking and SVG/PDF validation.
- [ ] Launch interactive web search index powered by `metadata.json`.

### FAQ

**Q: Is this repository an AI coding assistant software library?**  
A: No. **Awesome-Claude_Skills** is a documentation-first repository. It provides standardized guides, schemas, diagrams, and metadata for open-source AI optimization tools.

**Q: Why are tool rankings and star counts omitted from the root README?**  
A: To maintain a clean, scalable landing page. Tool comparisons, star metrics, and recommendation tables belong inside category `README.md` files where they can be evaluated in domain context.

**Q: Can proprietary tools be documented?**  
A: No. We exclusively document open-source projects, open protocols (like MCP), and open standards.

**Q: How do I add a new tool?**  
A: Review [CONTRIBUTING.md](CONTRIBUTING.md), copy the templates in `templates/`, and submit a Pull Request.

---

## 📄 License

This repository uses a dual licensing model:

- **Documentation & Content**: Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSES/CC-BY-4.0.txt).
- **Schemas, Templates & Tooling**: Licensed under the [MIT License](LICENSES/MIT.txt).

See [LICENSE](LICENSE) for full licensing boundaries.
