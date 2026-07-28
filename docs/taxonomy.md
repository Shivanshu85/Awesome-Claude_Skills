# Category Taxonomy & Scope Guide

This document defines the official domain taxonomy for **Awesome-Claude_Skills**. Every tool contributed to the repository must be placed into exactly one primary category folder under `skills/`.

Categorization is based on **functional capability and architectural role** within AI coding workflows, never by vendor name or arbitrary numbering.

---

## Taxonomy Overview Matrix

| Category Folder | Domain Name | Core Focus | Inclusion Criteria |
| :--- | :--- | :--- | :--- |
| `skills/memory/` | Memory Systems | Persistent state, graph memory, cross-session RAG | Tools providing persistent memory, temporal entity graphs, or multi-session state for agents. |
| `skills/context/` | Context Management | Context assembly, window packing, snippet injection | Frameworks optimizing context payload selection, dynamic doc injection, and window assembly. |
| `skills/context-compression/` | Context Compression | Prompt compression, token pruning, LLMLingua | SLM compressors, prompt truncation algorithms, and semantic token reduction tools. |
| `skills/token-optimization/` | Token Optimization | Input cost reduction, whitespace pruning, token economy | Utilities reducing input token count, stripping AST boilerplate, or optimizing prompt caching. |
| `skills/prompt-engineering/` | Prompt Engineering | System prompts, guardrails, structured outputs | System instruction frameworks, output schemas, and guardrail patterns. |
| `skills/codebase-intelligence/` | Codebase Intelligence | Repository packing, AST parsing, symbol graphs | Tools parsing ASTs, packing repos into context files (Repomix), or building code dependency graphs. |
| `skills/mcp/` | Model Context Protocol | MCP servers, tools, resources, prompts | Open-source MCP servers providing file access, git integration, API fetching, or reasoning. |
| `skills/developer-productivity/` | Developer Productivity | Workflow acceleration, CLI companions, macros | Developer workflow bridges, CLI helpers, PR description automation, and terminal shortcuts. |
| `skills/agent-workflows/` | Agent Workflows | Sequential thinking, planning, ReAct, reasoning | Reasoning protocols, multi-step task decomposition, reflection loops, and dynamic thinking trees. |
| `skills/security/` | Security | Prompt injection defense, sandboxing, permissions | Guardrails preventing prompt injection, MCP permission gates, and secret scanning utilities. |
| `skills/evaluation/` | Evaluation | Prompt evaluation, LLM benchmarks, quality scoring | Frameworks measuring code accuracy, instruction compliance, and retrieval precision. |
| `skills/testing/` | Testing | Prompt regression testing, assertion suites | Test suites validating system prompts, tool call schemas, and response assertions. |
| `skills/observability/` | Observability | Assistant tracing, token analytics, telemetry | Telemetry frameworks logging token consumption, span tracing, and assistant cost analytics. |

---

## Explicit Exclusions

To maintain high quality and razor-sharp focus, the following items are **strictly excluded** from all categories:

- **AI IDEs & Editors**: Closed-source or general IDE applications (Cursor, Windsurf) do not belong as categories; individual open-source skills *working with* them belong in appropriate categories.
- **General LLM Frameworks**: Generic chatbot wrappers or web UI interfaces.
- **Non-Coding AI Tools**: Image generators, audio AI, video synthesis, or social media bots.
- **Raw Datasets & Model Weights**: Weights files, fine-tuning datasets, or GPU optimization kernels.
