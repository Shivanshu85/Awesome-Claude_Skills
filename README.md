<p align="center">
  <img src="assets/banner.png" alt="Awesome-Claude_Skills Banner" width="100%" />
</p>

<h1 align="center">Awesome-Claude_Skills</h1>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/Docs_License-CC_BY_4.0-blue.svg" alt="License: CC BY 4.0"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/Tools_License-MIT-yellow.svg" alt="License: MIT"></a>
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="schemas/metadata.schema.json"><img src="https://img.shields.io/badge/Schema-Draft_07-informational.svg" alt="Schema Version"></a>
  <a href="docs/standards.md"><img src="https://img.shields.io/badge/Standard-v1.0-purple.svg" alt="Documentation Standard"></a>
</p>

> Build the world's best curated documentation library for AI context optimisation, token optimisation, memory systems, MCP servers, prompt engineering, repository intelligence, and developer productivity techniques that make AI coding assistants cheaper, faster, smarter, and more accurate.

---

## Table of Contents

- [Overview](#overview)
- [Mission](#mission)
- [Repository Philosophy](#repository-philosophy)
- [Why This Repository Exists](#why-this-repository-exists)
- [Who It Helps](#who-it-helps)
- [Repository Structure](#repository-structure)
- [Search by Goal ("I want to...")](#search-by-goal-i-want-to)
- [Browse by Problem](#browse-by-problem)
- [Browse by Category](#browse-by-category)
- [Most Popular Tools](#most-popular-tools)
- [Learning Path](#learning-path)
- [Repository Standards](#repository-standards)
- [Contributing](#contributing)
- [Roadmap & FAQ](#roadmap--faq)
- [Community & License](#community--license)

---

## Overview

**Awesome-Claude_Skills** is an authoritative, documentation-first open-source library dedicated to optimizing AI coding assistants, agents, and IDE integrations. Rather than listing generic AI tools or random prompt snippets, this repository provides complete, standardized knowledge packages for open-source tools, protocols, MCP servers, memory systems, and context optimization techniques.

Every documented tool in this repository follows a rigid, 7-file specification (`README.md`, `metadata.json`, `workflow.mmd`, `workflow.svg`, `Tool-Guide.pdf`, `LICENSE`), giving developers predictable, comprehensive, and evidence-based guidance.

---

## Mission

> Build the world's best curated documentation library for AI context optimisation, token optimisation, memory systems, MCP servers, prompt engineering, repository intelligence, and developer productivity techniques that make AI coding assistants cheaper, faster, smarter, and more accurate.

This repository exists to help developers discover and adopt tools that:

- **✓ Reduce token usage** and API expenses
- **✓ Reduce API costs** without sacrificing response precision
- **✓ Improve context quality** and eliminate noisy, irrelevant context
- **✓ Improve long-context handling** across massive prompt windows
- **✓ Improve memory** and multi-session state retention
- **✓ Improve reasoning** through structured thinking protocols
- **✓ Improve repository understanding** via AST indexing and graph search
- **✓ Improve AI coding assistants** across Claude Code, Cursor, Windsurf, Roo Code, Continue, and CLI agents
- **✓ Improve prompt efficiency** with systematic compression
- **✓ Improve retrieval** performance in RAG and memory pipelines
- **✓ Improve workflow quality** with reliable tool automation

---

## Repository Philosophy

This repository is governed by 7 strict architectural principles:

1. **Quality Over Quantity**: We only document important, useful, trusted open-source projects.
2. **Documentation First**: This is a documentation repository, not a code library or file dumper.
3. **Single Source of Truth**: The skill `README.md` is the authoritative single source of truth for narrative documentation.
4. **No Duplicate Documentation**: We never maintain parallel text files or duplicate prose.
5. **Consistency Over Creativity**: Every tool documentation follows an identical 28-section structure.
6. **Problem-First Navigation**: Developers search by the problem they face, not by arbitrary tool names.
7. **Evidence-Based Documentation**: We never invent benchmarks, fake metric scores, or marketing claims. All content is derived from official documentation and verifiable testing.

---

## Why This Repository Exists

Modern AI coding assistants are powerful, but developers frequently face severe friction:

- **Excessive Token Costs**: Bloated prompts and full-file dumps waste millions of tokens.
- **Context Limits & Degradation**: LLMs suffer from "lost in the middle" attention loss as context windows grow.
- **Stateless Agent Sessions**: Coding assistants forget previous bug fixes, design decisions, and coding standards between sessions.
- **Superficial Codebase Knowledge**: Assistants fail to navigate multi-repo dependencies or AST symbol graphs.
- **Unverifiable Prompt Quality**: Lack of evaluation and regression testing leads to brittle prompt designs.

**Awesome-Claude_Skills** solves these challenges by providing curated, production-grade documentation for open-source tools designed specifically to optimize AI efficiency.

---

## Who It Helps

- 👨‍💻 **Developers & Software Engineers**: Discover proven techniques to make IDE assistants faster and cheaper.
- 🤖 **AI & LLM Engineers**: Implement robust memory RAG, context compression, and MCP server integrations.
- ⚡ **Prompt Engineers & Vibe Coders**: Adopt structured prompt frameworks, evaluation tools, and guardrails.
- 🎓 **Students & Researchers**: Study state-of-the-art AI reasoning, sequential thinking, and codebase intelligence.
- 🌐 **Open Source Contributors**: Add standardized documentation for emerging AI optimization tools.

---

## Repository Structure

```
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
├── .github/                           <- Issue Forms & PR Templates
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── ISSUE_TEMPLATE/
│       ├── new_tool_request.yml
│       └── tool_update.yml
│
├── LICENSES/                          <- Full Legal Text Files
│   ├── CC-BY-4.0.txt
│   └── MIT.txt
│
├── assets/                            <- Repository Visual Assets & Banners
│   └── banner.png                     <- Official Banner Graphic
│
├── docs/                              <- Repository Core Knowledge Infrastructure
│   ├── taxonomy.md                    <- Category Scope & Boundaries Definition
│   ├── glossary.md                    <- Single-source AI Terminology Definitions
│   └── standards.md                   <- Comprehensive Documentation Style Guide
│
├── schemas/                           <- Machine Schemas
│   └── metadata.schema.json           <- JSON Schema (Draft 07) for tool metadata
│
├── templates/                         <- Reusable Skill Generation Starters
│   ├── README.template.md             <- 28-Section Canonical README Template
│   ├── metadata.template.json         <- Validated Starter JSON Metadata
│   └── workflow.template.mmd          <- Standardized Mermaid Flowchart Template
│
└── skills/                            <- Categorized Knowledge Domain Packages
    ├── memory/                        <- Persistent memory, graph memory, vector RAG
    ├── context/                       <- Context assembly, window packing, context injection
    ├── context-compression/           <- Prompt compression, LLMLingua, context truncation
    ├── token-optimization/            <- Token economy, cost reduction, input pruning
    ├── prompt-engineering/            <- System prompts, templates, guardrails
    ├── codebase-intelligence/         <- Repository packing, AST parsing, symbol graphs
    ├── mcp/                           <- Model Context Protocol servers & tools
    ├── developer-productivity/        <- Developer workflow acceleration, CLI companions
    ├── agent-workflows/               <- Sequential thinking, planning, ReAct, reasoning
    ├── security/                      <- Prompt injection defense, sandboxing, permissions
    ├── evaluation/                    <- LLM benchmarks, prompt evals, quality metrics
    ├── testing/                       <- Prompt regression testing, AI test suites
    └── observability/                 <- Telemetry, token counters, span tracing
```

---

## Search by Goal ("I want to...")

Quickly find documentation based on your immediate engineering objective:

- **I want to [Reduce Context Size](file:///skills/context-compression/README.md)**: Compress long prompts using tools like [LLMLingua](file:///skills/context-compression/README.md) and [LongLLMLingua](file:///skills/context-compression/README.md).
- **I want to [Reduce Token Usage](file:///skills/token-optimization/README.md)**: Prune redundant whitespace, AST nodes, and repetitive system prompts.
- **I want to [Reduce API Cost](file:///skills/token-optimization/README.md)**: Optimize input token economy to lower API spending.
- **I want to [Improve Memory](file:///skills/memory/README.md)**: Implement graph memory and session retention using [Mem0](file:///skills/memory/README.md), [Graphiti](file:///skills/memory/README.md), or [OpenMemory](file:///skills/memory/README.md).
- **I want to [Understand Large Codebases](file:///skills/codebase-intelligence/README.md)**: Pack and index entire repositories using [Repomix](file:///skills/codebase-intelligence/README.md) or [RepoPrompt](file:///skills/codebase-intelligence/README.md).
- **I want to [Improve Prompt Quality](file:///skills/prompt-engineering/README.md)**: Design structured system prompts with clear constraints and guardrails.
- **I want to [Compress Prompts](file:///skills/context-compression/README.md)**: Remove low-information tokens while preserving semantic intent.
- **I want to [Improve AI Reasoning](file:///skills/agent-workflows/README.md)**: Use multi-step reasoning protocols like [Sequential Thinking MCP](file:///skills/agent-workflows/README.md).
- **I want to [Connect MCP Servers](file:///skills/mcp/README.md)**: Integrate standardized tools like [Filesystem MCP](file:///skills/mcp/README.md), [Git MCP](file:///skills/mcp/README.md), and [GitHub MCP](file:///skills/mcp/README.md).
- **I want to [Improve Repository Understanding](file:///skills/codebase-intelligence/README.md)**: Extract AST symbol graphs and file trees for context windows.
- **I want to [Optimise RAG](file:///skills/memory/README.md)**: Build hybrid vector and knowledge-graph retrieval systems for codebase search.
- **I want to [Reduce Hallucinations](file:///skills/agent-workflows/README.md)**: Enforce verification loops, reflection, and step-by-step reasoning protocols.
- **I want to [Improve Workflow](file:///skills/developer-productivity/README.md)**: Automate assistant workflows, IDE bindings, and CLI agent triggers.

---

## Browse by Problem

Find solutions curated by specific engineering bottlenecks:

| Problem Statement | Root Cause | Recommended Category | Key Solution Tools |
| :--- | :--- | :--- | :--- |
| **High Token Costs & Large Context Windows** | Raw codebase files exceed model context limits, ballooning API costs. | [`skills/context-compression/`](file:///skills/context-compression/README.md)<br>[`skills/token-optimization/`](file:///skills/token-optimization/README.md) | LLMLingua, LongLLMLingua, Repomix |
| **Stateless AI Sessions & Lost Context** | Assistants forget architectural decisions and user preferences between chats. | [`skills/memory/`](file:///skills/memory/README.md) | Mem0, Graphiti, OpenMemory |
| **Massive Repository Complexity** | AI assistants struggle to map cross-file dependencies and AST symbol trees. | [`skills/codebase-intelligence/`](file:///skills/codebase-intelligence/README.md) | Repomix, RepoPrompt |
| **Superficial Reasoning & Hallucinations** | AI jumps to incorrect coding solutions without multi-step plan verification. | [`skills/agent-workflows/`](file:///skills/agent-workflows/README.md) | Sequential Thinking MCP |
| **Disconnected Tools & File Access** | Assistant cannot inspect local files, run git commands, or fetch web data safely. | [`skills/mcp/`](file:///skills/mcp/README.md) | Filesystem MCP, Git MCP, Fetch MCP, GitHub MCP |
| **Brittle Prompts & Regression Errors** | Prompt edits break assistant behavior without automated test feedback. | [`skills/evaluation/`](file:///skills/evaluation/README.md)<br>[`skills/testing/`](file:///skills/testing/README.md) | PromptEval, Ragas |
| **Prompt Injection & Tool Security** | Untrusted repository inputs or web content attempt to hijack tool calls. | [`skills/security/`](file:///skills/security/README.md) | PromptGuard, ToolSandbox |

---

## Browse by Category

The repository is organized into 13 core domain categories:

| Category | Description | Focus Area | Status / Tools |
| :--- | :--- | :--- | :--- |
| 🧠 **[Memory](file:///skills/memory/README.md)** | Persistent memory systems, graph memory & multi-session RAG | Session state, entity graphs, memory retrieval | *3 Tools Documented* |
| 📦 **[Context](file:///skills/context/README.md)** | Context window management, packing & context injection | Token windows, dynamic assembly, context hydration | *2 Tools Documented* |
| ⚡ **[Context Compression](file:///skills/context-compression/README.md)** | Prompt compression & long-context truncation | LLMLingua, token pruning, semantic compression | *2 Tools Documented* |
| 💰 **[Token Optimization](file:///skills/token-optimization/README.md)** | Token economy, prompt pruning & API cost reduction | Input cost reduction, whitespace pruning, AST reduction | *2 Tools Documented* |
| ✍️ **[Prompt Engineering](file:///skills/prompt-engineering/README.md)** | System prompts, structured instructions & guardrails | System instructions, few-shot templates, output schemas | *3 Tools Documented* |
| 🔍 **[Codebase Intelligence](file:///skills/codebase-intelligence/README.md)** | Repository packing, AST parsing & symbol graph search | Codebase maps, Repomix, AST indexers, RepoPrompt | *3 Tools Documented* |
| 🔌 **[MCP](file:///skills/mcp/README.md)** | Model Context Protocol servers & standardized tool interfaces | Filesystem, Git, GitHub, Fetch, Sequential Thinking | *5 Tools Documented* |
| 🚀 **[Developer Productivity](file:///skills/developer-productivity/README.md)** | Workflow acceleration & AI assistant developer tooling | Dev workflow macros, CLI helpers, assistant bindings | *2 Tools Documented* |
| 🔄 **[Agent Workflows](file:///skills/agent-workflows/README.md)** | Multi-step reasoning, planning, reflection & ReAct loops | Sequential thinking, task planning, decision trees | *3 Tools Documented* |
| 🛡️ **[Security](file:///skills/security/README.md)** | Prompt injection defense, tool permissions & sandboxing | Security boundaries, secret scanning, execution sandboxes | *2 Tools Documented* |
| 📊 **[Evaluation](file:///skills/evaluation/README.md)** | Prompt evaluation, LLM benchmarks & quality metrics | Output scoring, accuracy benchmarks, eval pipelines | *2 Tools Documented* |
| 🧪 **[Testing](file:///skills/testing/README.md)** | Prompt testing, regression suites & automated validation | Assertions, regression test loops, unit testing prompts | *2 Tools Documented* |
| 🔭 **[Observability](file:///skills/observability/README.md)** | Assistant tracing, token analytics & execution telemetry | Token counters, span logging, telemetry dashboards | *2 Tools Documented* |

---

## Most Popular Tools

Highlighted open-source tools documented across our categories:

- 📂 **[Filesystem MCP](file:///skills/mcp/README.md)**: Secure local file reading, writing, and directory traversal for Claude and MCP-compatible assistants.
- 📑 **[Context7](file:///skills/context/README.md)**: Dynamic context window assembler for live documentation and code snippets.
- 🕸️ **[Graphiti](file:///skills/memory/README.md)**: Temporal knowledge graph memory engine for continuous assistant memory.
- 📦 **[Repomix](file:///skills/codebase-intelligence/README.md)**: Packed codebase representation tool designed for LLM context windows.
- 🧠 **[Mem0](file:///skills/memory/README.md)**: Universal memory layer for AI agents and coding assistants.
- ⚡ **[LLMLingua](file:///skills/context-compression/README.md)**: Small language model-based prompt compressor reducing prompt tokens by up to 20x.
- 🔬 **[LongLLMLingua](file:///skills/context-compression/README.md)**: Context compression specifically tuned for long-context LLMs to mitigate attention loss.
- 🔄 **[Sequential Thinking MCP](file:///skills/agent-workflows/README.md)**: Dynamic, multi-step problem solving server providing step-by-step reasoning for AI assistants.
- 🐙 **[Git MCP](file:///skills/mcp/README.md)**: Standardized Model Context Protocol server for inspecting git history, diffs, and commits.
- 🌐 **[Fetch MCP](file:///skills/mcp/README.md)**: Web fetching and markdown conversion server for real-time web content retrieval.
- 🐙 **[GitHub MCP](file:///skills/mcp/README.md)**: GitHub API integration server for pull requests, issues, and code search.
- 💾 **[OpenMemory](file:///skills/memory/README.md)**: Open-source local vector memory engine for session state retention.
- 💻 **[RepoPrompt](file:///skills/codebase-intelligence/README.md)**: Interactive codebase prompt generator and repository packer.

---

## Learning Path

Recommended progression for mastering AI coding assistant optimization:

```
1. Basics & Context Window Fundamentals
   ├── Learn Token Economy (skills/token-optimization/)
   └── Master Prompt Compression (skills/context-compression/)
        │
2. Repository Intelligence & Context Assembly
   ├── Pack Codebases with Repomix (skills/codebase-intelligence/)
   └── Manage Context Windows with Context7 (skills/context/)
        │
3. Standard Tool Interfaces & Memory Systems
   ├── Connect MCP Servers (skills/mcp/)
   └── Implement Graph Memory with Mem0/Graphiti (skills/memory/)
        │
4. Reasoning Protocols & Production Security
   ├── Adopt Sequential Thinking (skills/agent-workflows/)
   ├── Enforce Security Guardrails (skills/security/)
   └── Set Up Prompt Testing & Observability (skills/testing/ & skills/observability/)
```

---

## Repository Standards

Every tool documentation in this repository strictly adheres to our core guidelines:

- 📐 **[Documentation Style Guide (`docs/standards.md`)](file:///docs/standards.md)**: Mandatory 28-section structure, heading rules, and formatting standards.
- 📖 **[Category Taxonomy Guide (`docs/taxonomy.md`)](file:///docs/taxonomy.md)**: Domain inclusion and exclusion rules.
- 📚 **[Glossary (`docs/glossary.md`)](file:///docs/glossary.md)**: Single-source definitions for RAG, MCP, Context Window, Prompt Cache, AST Parsing, and Sequential Thinking.
- 🤖 **[Metadata Schema (`schemas/metadata.schema.json`)](file:///schemas/metadata.schema.json)**: Machine-readable schema validating `metadata.json` for all tools.

---

## Contributing

We welcome contributions from developers, AI engineers, and open-source maintainers! Adding a new tool to **Awesome-Claude_Skills** requires copying pre-built templates and providing validated information:

1. Read [CONTRIBUTING.md](file:///CONTRIBUTING.md) for complete submission criteria.
2. Choose the correct category under `skills/<category>/`.
3. Copy `templates/README.template.md`, `templates/metadata.template.json`, and `templates/workflow.template.mmd`.
4. Validate `metadata.json` against `schemas/metadata.schema.json`.
5. Ensure your tool folder follows the exact 7-file structure:
   `README.md`, `metadata.json`, `workflow.mmd`, `workflow.svg`, `Tool-Guide.pdf`, `LICENSE`.
6. Submit a Pull Request using our [.github/PULL_REQUEST_TEMPLATE.md](file:///.github/PULL_REQUEST_TEMPLATE.md).

---

## Roadmap & FAQ

### Roadmap

- [x] Establish canonical 13-category architecture and core standards.
- [x] Release Draft 07 JSON Schema and 28-section tool README templates.
- [ ] Expand tool documentation across all 13 categories to 50+ open-source tools.
- [ ] Implement automated CI workflows for PDF generation and link validation.
- [ ] Launch web index site powered by `metadata.json` schemas.

### FAQ

**Q: Is this repository an AI coding assistant or software library?**  
A: No. **Awesome-Claude_Skills** is a documentation-first repository. It contains comprehensive guides, schemas, diagrams, and metadata for open-source AI optimization tools.

**Q: Can I add a proprietary or closed-source tool?**  
A: No. We exclusively document trusted open-source tools, open standards (like MCP), and open-access techniques.

**Q: Why are non-coding tools excluded?**  
A: To maintain razor-sharp focus and quality, we only include tools that directly improve AI coding assistants, token economy, context management, memory, and developer productivity.

---

## Community & License

- 📜 **[Code of Conduct](file:///CODE_OF_CONDUCT.md)**: Community guidelines (Contributor Covenant v2.1).
- 🔒 **[Security Policy](file:///SECURITY.md)**: Vulnerability disclosure and reporting procedures.
- 📜 **[Changelog](file:///CHANGELOG.md)**: Track version history and architectural changes.

### Dual Licensing

- **Documentation & Content**: Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](file:///LICENSES/CC-BY-4.0.txt).
- **Schemas, Templates & Tooling**: Licensed under the [MIT License](file:///LICENSES/MIT.txt).

See [LICENSE](file:///LICENSE) for detailed license boundary specifications.
