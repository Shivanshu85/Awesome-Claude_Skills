# Category Taxonomy & Scope Guide

This document defines the official domain taxonomy for **AI-Skills-Library**. Every skill contributed to the repository must be placed into exactly one primary category folder under `skills/`.

Categorization is based on **functional capability and architectural role** within AI coding workflows, never by vendor name or arbitrary numbering.

---

## Taxonomy Overview Matrix

| Category Folder | Domain Name | Core Focus |
| :--- | :--- | :--- |
| `skills/memory/` | Memory Systems | Persistent state, graph memory, cross-session RAG |
| `skills/context/` | Context Management | Context assembly, window packing, token pruning |
| `skills/prompt-engineering/` | Prompt Engineering | System prompts, sub-agent templates, guardrails |
| `skills/mcp/` | Model Context Protocol | MCP server tools, resources, prompts, transport protocols |
| `skills/automation/` | Automation & CI/CD | Autonomous task loops, trigger scripts, dev workflows |
| `skills/planning/` | Task Planning | Step-by-step task breakdown, milestone tracking |
| `skills/reasoning/` | Reasoning Protocols | Chain-of-thought, tree-of-thought, decision trees |
| `skills/developer-tools/` | Developer Tools | IDE extensions, CLI agent helpers, linters |
| `skills/repository-intelligence/` | Repository Intelligence | AST parsing, code graph packing, Repomix |
| `skills/security/` | Security & Safety | Prompt injection defense, secret detection |
| `skills/testing/` | Automated Testing | Test generation, dynamic assertion verification |
| `skills/evaluation/` | LLM Evaluation | Output bench-marking, eval datasets, scoring |
| `skills/observability/` | Observability & Tracing | Agent tracing, token counters, span logging |
| `skills/agent-frameworks/` | Agent Frameworks | Multi-agent coordination patterns, swarms |
| `skills/ai-ides/` | AI IDE Integrations | Cursor rules, Claude Code configs, Windsurf |
| `skills/productivity/` | Developer Productivity | Velocity macros, boilerplate generators |
| `skills/code-generation/` | Code Generation | Code synthesis, refactoring, pattern migration |

---

## Category Specifications

### 1. `memory/` (Memory Systems)
- **Purpose**: Document mechanisms that preserve conversational state, developer preferences, and codebase knowledge across multiple sessions.
- **Scope**: Graph databases, persistent key-value memory banks, long-term vector RAG stores.
- **Examples**: Graphiti, Mem0, Memory Bank.
- **Belongs Here**: Long-term memory tools, knowledge graph RAG for code.
- **Does NOT Belong**: Single-prompt context windows (use `context/`), prompt templates (use `prompt-engineering/`).

### 2. `context/` (Context Management)
- **Purpose**: Document techniques and tools for optimizing LLM context window space and retrieval precision.
- **Scope**: Context packing, token compression, prompt pruning, sliding window mechanisms.
- **Examples**: LLMLingua, Compact Context, Window Truncators.
- **Belongs Here**: Token counters, compression algorithms, context window serializers.
- **Does NOT Belong**: Codebase packagers that generate repository ASTs (use `repository-intelligence/`).

### 3. `prompt-engineering/` (Prompt Engineering)
- **Purpose**: Document standardized prompt structures, system prompts, and instruction formats for AI coders.
- **Scope**: System instruction designs, few-shot prompting patterns, agent personas, output formatting constraints.
- **Examples**: XML Prompt Enclosures, Chain-of-Thought System Prompts, Guardrail Prompts.
- **Belongs Here**: Reusable prompt templates, persona instructions.
- **Does NOT Belong**: Automated prompt execution loops (use `automation/`).

### 4. `mcp/` (Model Context Protocol)
- **Purpose**: Document Model Context Protocol (MCP) server specifications, tools, resources, and client integration patterns.
- **Scope**: Standardized MCP servers providing external tools, filesystem access, database tools, and API connectors.
- **Examples**: GitHub MCP Server, Filesystem MCP Server, PostgreSQL MCP Server.
- **Belongs Here**: Native MCP protocol servers and tool schemas.
- **Does NOT Belong**: Generic REST APIs that lack MCP transport compliance.

### 5. `automation/` (Automation)
- **Purpose**: Document autonomous execution loops, background agent triggers, and CI/CD AI pipeline integrations.
- **Scope**: Task automation loops, cron-triggered agent workflows, auto-fixing build agents.
- **Examples**: GitHub Actions AI workflows, Background Refactoring Loops.
- **Belongs Here**: Execution scripts, automated PR reviewers, background worker loops.
- **Does NOT Belong**: Pure task decomposition plans without execution (use `planning/`).

### 6. `planning/` (Task Planning)
- **Purpose**: Document architectures and templates for breaking complex developer requests into verifiable implementation steps.
- **Scope**: Implementation plans, task DAGs, milestone verification criteria.
- **Examples**: Architectural Plan Generators, Step-by-Step Task Breakdown Protocols.
- **Belongs Here**: Plan formats, task breakdown templates, execution roadmaps.
- **Does NOT Belong**: Dynamic reasoning algorithms (use `reasoning/`).

### 7. `reasoning/` (Reasoning Protocols)
- **Purpose**: Document formal cognitive and logical frameworks used by AI models to solve complex algorithmic tasks.
- **Scope**: Chain-of-Thought (CoT), Tree-of-Thought (ToT), Self-Correction loops, ReAct patterns.
- **Examples**: Reflection Loops, Verification Checkers, Multi-Path Reasoning.
- **Belongs Here**: Algorithmic reasoning steps, verification loops.
- **Does NOT Belong**: Multi-agent orchestration frameworks (use `agent-frameworks/`).

### 8. `developer-tools/` (Developer Tools)
- **Purpose**: Document CLI utilities, agent extensions, and helper tools built to enhance developer interaction with AI.
- **Scope**: CLI wrappers, terminal bridges, local webview inspect tools.
- **Examples**: Agent CLI Wrappers, Dev Server Bridges, Terminal Assistants.
- **Belongs Here**: Interactive developer utilities, helper CLIs.
- **Does NOT Belong**: Pure IDE rule files (use `ai-ides/`).

### 9. `repository-intelligence/` (Repository Intelligence)
- **Purpose**: Document codebase analysis, AST parsing, dependency mapping, and file bundling for LLM ingestion.
- **Scope**: Codebase packing, symbol graph generation, dependency tree extraction.
- **Examples**: Repomix, Tree-Sitter AST Packers, Symbol Graph Builders.
- **Belongs Here**: Repo packers, file bundlers, call-graph extractors.
- **Does NOT Belong**: Vector databases for memory (use `memory/`).

### 10. `security/` (Security & Safety)
- **Purpose**: Document security patterns, threat mitigation, prompt injection defense, and secret scanning for AI systems.
- **Scope**: Guardrails, input sanitizers, privilege escalation prevention, secret detectors.
- **Examples**: Prompt Injection Sanitizers, Secret Redaction Guardrails, Policy Enforcers.
- **Belongs Here**: Security policies, threat models, input validators.
- **Does NOT Belong**: Code testing frameworks (use `testing/`).

### 11. `testing/` (Automated Testing)
- **Purpose**: Document AI-assisted test generation, assertion verification, and dynamic execution verification loops.
- **Scope**: Unit test generators, integration test loops, assertion verifiers.
- **Examples**: TestSprite, Pytest Generation Agents, Coverage Verification Loops.
- **Belongs Here**: Test generation patterns, test runner integration tools.
- **Does NOT Belong**: Benchmark scoring of LLM accuracy (use `evaluation/`).

### 12. `evaluation/` (LLM Evaluation)
- **Purpose**: Document scoring, benchmarking, and quality assessment frameworks for evaluating AI coding outputs.
- **Scope**: Eval datasets, pass@k metrics, LLM-as-a-judge scoring protocols.
- **Examples**: Coding Benchmark Evaluators, Output Precision Scoring.
- **Belongs Here**: Evaluation benchmarks, quality scoring tools.
- **Does NOT Belong**: Code unit testing (use `testing/`).

### 13. `observability/` (Observability & Tracing)
- **Purpose**: Document telemetry, token usage tracking, span tracing, and execution logging for AI agents.
- **Scope**: Token loggers, OpenTelemetry trace collectors, agent execution monitors.
- **Examples**: Agent Trace Collectors, Token Usage Meters, Cost Logging Spans.
- **Belongs Here**: Telemetry integrations, tracing protocols.
- **Does NOT Belong**: Security audit logs (use `security/`).

### 14. `agent-frameworks/` (Agent Frameworks)
- **Purpose**: Document multi-agent coordination topologies, delegation patterns, and agent communication protocols.
- **Scope**: Supervisor-agent architectures, agent swarms, tool-delegation graphs.
- **Examples**: Hierarchical Supervisor Patterns, Peer-to-Peer Agent Swarms.
- **Belongs Here**: Multi-agent system architectures, delegation rules.
- **Does NOT Belong**: Single-agent system prompt files (use `prompt-engineering/`).

### 15. `ai-ides/` (AI IDE Integrations)
- **Purpose**: Document configuration rules, native skills, and setup guidelines for AI-native IDEs and editor extensions.
- **Scope**: Cursor `.cursorrules`, Claude Code `.clauderc`, Windsurf configurations, VS Code AI settings.
- **Examples**: Cursor Custom Rules, Claude Code Tool Integrations.
- **Belongs Here**: Native IDE configuration files and editor settings.
- **Does NOT Belong**: Standalone CLI binaries (use `developer-tools/`).

### 16. `productivity/` (Developer Productivity)
- **Purpose**: Document workflow accelerators, velocity macros, and automated task shortcuts for developers.
- **Scope**: Git commit message generators, PR description builders, boilerplate expanders.
- **Examples**: Auto-Commit Message Generators, PR Summary Automation.
- **Belongs Here**: Developer productivity macros and workflow shortcuts.
- **Does NOT Belong**: Automated test generators (use `testing/`).

### 17. `code-generation/` (Code Generation)
- **Purpose**: Document code synthesis, pattern transformation, boilerplate generation, and migration templates.
- **Scope**: Code synthesis instructions, API migration patterns, refactoring templates.
- **Examples**: Pattern Transpilers, Refactoring Synthesis Rules, Migration Generators.
- **Belongs Here**: Code translation and refactoring templates.
- **Does NOT Belong**: Repository-wide AST bundlers (use `repository-intelligence/`).
