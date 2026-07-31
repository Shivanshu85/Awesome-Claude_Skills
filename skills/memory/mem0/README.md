# Mem0 — The Memory Layer for Personalized AI

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](file:///skills/memory/mem0/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/mem0ai/mem0?style=social)](https://github.com/mem0ai/mem0)
[![GitHub Forks](https://img.shields.io/github/forks/mem0ai/mem0?style=social)](https://github.com/mem0ai/mem0)
[![PyPI version](https://img.shields.io/pypi/v/mem0ai?color=%2334D058&label=pypi%20package)](https://pypi.org/project/mem0ai)
[![Npm package](https://img.shields.io/npm/v/mem0ai)](https://www.npmjs.com/package/mem0ai)

**Mem0** ("mem-zero") is an intelligent, multi-layer memory retention system that equips AI assistants, agents, and IDE extensions with continuous long-term memory across sessions, users, and projects.

---

## Project Snapshot

| Property | Details |
| :--- | :--- |
| **Category** | [Memory Systems](file:///skills/memory/README.md) |
| **Primary Language** | Python (SDK), TypeScript/Node.js (SDK), Rust / CLI |
| **License** | Apache License 2.0 |
| **GitHub Stars** | ⭐ 30k+ |
| **GitHub Forks** | 🍴 2.8k+ |
| **Contributors** | 100+ open-source contributors |
| **Maintenance Status** | ✅ Active (Supported by Y Combinator S24) |
| **Official Repository** | [github.com/mem0ai/mem0](https://github.com/mem0ai/mem0) |
| **Official Documentation** | [docs.mem0.ai](https://docs.mem0.ai) |
| **Official Website** | [mem0.ai](https://mem0.ai) |

---

## Problems Solved

- **Stateless AI Chat Sessions**: Standard LLM calls reset history on every prompt, forcing developers to repeatedly paste context, code standards, and project preferences.
- **Context Window Inflation & High API Costs**: Appending full conversation transcripts balloon token usage, driving up API invoices and slowing response times.
- **Loss of Cross-Session Entity Relationships**: Basic vector RAG fails to link entities, user choices, and historical decisions over time.

---

## Key Features

- **Multi-Level Memory Scope**: Seamlessly tracks memory across three distinct scopes: **User**, **Session**, and **Agent**.
- **Single-Pass ADD-Only Extraction**: Accumulates memories safely without destructive overwrites.
- **Multi-Signal Parallel Retrieval**: Combines semantic embeddings, BM25 keyword matching, and entity linking for hybrid search.
- **Temporal Reasoning**: Time-aware ranking accurately resolves queries about current state, past events, and future schedules.
- **Cross-Platform SDKs & CLI**: Native support for Python (`mem0ai`), Node.js (`mem0ai`), and instant CLI integration (`@mem0/cli`).

---

## Best Use Cases

1. **Personalized AI Coding Assistants**: Train IDE assistants (Claude Code, Cursor, Windsurf) to remember coding standards, local dev setups, and past bug resolutions.
2. **Autonomous Developer Agents**: Provide agent swarms with shared, persistent memory across multi-step execution loops.
3. **Customer Support Bots**: Retain customer interaction history, past support tickets, and individual preferences.
4. **Adaptive Productivity Environments**: Build workflows that automatically adjust to developer habits over time.

---

## Supported Integrations

- **LLM Providers**: OpenAI, Anthropic Claude, Google Gemini, Ollama, Groq, Cohere.
- **Vector Stores**: Qdrant, Milvus, Pinecone, PGVector, Chroma, Weaviate.
- **Agent Frameworks**: LangChain, LlamaIndex, CrewAI, AutoGen.

---

## Installation

### Python SDK
```bash
pip install mem0ai
```

### Node.js / TypeScript SDK
```bash
npm install mem0ai
```

### CLI Agent Setup
```bash
npm install -g @mem0/cli
mem0 init --agent --agent-caller claude-code
```

---

## Quick Start Example (Python)

```python
from mem0 import Memory

# 1. Initialize Memory Client
m = Memory()

# 2. Add memories for a user or coding session
m.add(
    "User prefers TypeScript with strict mode and uses Tailwind CSS",
    user_id="dev_user_101"
)

# 3. Search relevant memory context
relevant_memories = m.search(
    query="What styling library does the user prefer?",
    user_id="dev_user_101"
)

print(relevant_memories)
```

---

## Detailed Documentation & Interactive Guide

For comprehensive architecture diagrams, advanced configuration, vector store bindings, benchmark metrics, and head-to-head comparisons, view the complete **[Mem0 Technical Guide (guide.html)](file:///skills/memory/mem0/guide.html)**.

---

## Official Resources

- 📦 **GitHub Repository**: [github.com/mem0ai/mem0](https://github.com/mem0ai/mem0)
- 📖 **Official Documentation**: [docs.mem0.ai](https://docs.mem0.ai)
- 🌐 **Official Website**: [mem0.ai](https://mem0.ai)
- 📄 **Research Benchmarks**: [mem0.ai/research](https://mem0.ai/research)
