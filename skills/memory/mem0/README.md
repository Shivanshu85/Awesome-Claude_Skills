<div align="center">

# Mem0

The Memory Layer for Personalized AI Applications, Autonomous Agents, and Enterprise LLM Workflows

Provides an intelligent, self-improving memory layer that retains facts, user preferences, and cross-session context across LLM interactions.

[Official Website](https://mem0.ai) • [Documentation](https://docs.mem0.ai) • [GitHub Repository](https://github.com/mem0ai/mem0) • [📖 Open Interactive Guide](https://Shivanshu85.github.io/awesome-ai-skills/skills/memory/mem0/guide.html)

![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
![Category](https://img.shields.io/badge/Category-AI_Memory_Infrastructure-orange)
![Language](https://img.shields.io/badge/Language-Python%20%7C%20TypeScript-blue)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

</div>

---

## Overview

**Mem0** ("Memory Zero") is an open-source memory orchestration engine designed to give Large Language Models (LLMs), AI coding assistants, and autonomous agents persistent, cross-session memory[cite: 1]. Standard LLM conversations are inherently stateless, requiring developers to either re-inject full chat logs—inflating token costs and latency—or rely on naive vector chunking, which fails to update changing user facts[cite: 1].

Mem0 resolves this by dynamically extracting atomic facts from natural language conversations, deduplicating them against historic records, and maintaining a structured, hybrid vector-graph store[cite: 1]. When users update their preferences or state over time, Mem0 automatically mutates existing memories rather than appending duplicate or contradictory vectors[cite: 1].

Designed for AI application developers, agent engineers, and developer tool creators, Mem0 provides a scalable memory infrastructure that reduces prompt context overhead, lowers API token costs, and delivers hyper-personalized AI responses[cite: 1].

---

## Repository Information

| Property | Details |
| :--- | :--- |
| **Category** | AI Memory Infrastructure & Context Optimization |
| **Subcategory** | Vector-Graph Hybrid Store / LLM Orchestration Layer |
| **Interactive Guide** | [📖 Open Guide HTML](https://Shivanshu85.github.io/awesome-ai-skills/skills/memory/mem0/guide.html) |
| **License** | Apache 2.0 License |
| **Primary Languages** | Python, TypeScript |
| **Repository** | [github.com/mem0ai/mem0](https://github.com/mem0ai/mem0) |
| **Documentation** | [docs.mem0.ai](https://docs.mem0.ai) |
| **Official Website** | [mem0.ai](https://mem0.ai) |
| **Latest Release** | v1.1.26 |
| **Open Source** | Yes |
| **Status** | Production Ready |
| **Maintainer** | Mem0 Core Team & Community |

---

## GitHub Statistics

| Metric | Value |
| :--- | :--- |
| **⭐ Stars** | 26,500+ |
| **🍴 Forks** | 2,800+ |
| **👀 Watchers** | 310+ |
| **📦 Releases** | 120+ |
| **🐞 Open Issues** | 45 |
| **👥 Contributors** | 85+ |
| **📅 Last Commit** | July 2026 |
| **Repository Size** | ~48 MB |

---

## Why Developers Use It

* **Drastic Cost & Token Reduction:** Cuts prompt payload size by up to 90% by replacing raw message logs with compressed atomic facts[cite: 1].
* **Cross-Session Persistence:** Maintains user preferences, coding habits, and project architectural choices indefinitely across sessions[cite: 1].
* **Multi-Tenant Partitioning:** Built-in isolation for `user_id`, `agent_id`, and `run_id` scope configurations[cite: 1].
* **Model Context Protocol (MCP) Support:** Connects directly to AI coding tools like Claude Code, Cursor, and Windsurf[cite: 1].
* **Self-Hostable & Air-Gapped:** Can be run 100% locally with Ollama and local Qdrant/Chroma databases for complete data privacy[cite: 1].

---

## Problems Solved

* **LLM Amnesia:** Prevents AI tools from forgetting user preferences and decisions between chat sessions[cite: 1].
* **Context Window Bloat:** Stops exponential token usage caused by stuffing full chat histories into prompts[cite: 1].
* **Contradictory Memories:** Automatically updates or deletes outdated facts when user state changes[cite: 1].
* **High Inference Latency:** Accelerates Time-To-First-Token (TTFT) by reducing prompt payload lengths[cite: 1].
* **Memory Duplication:** Consolidates redundant conversational facts into clean atomic entries[cite: 1].

---

## Key Features

* **LLM-Driven Fact Extraction:** Automatically parses natural language to extract key preferences, traits, and facts[cite: 1].
* **Dynamic Memory Mutation:** Executes `ADD`, `UPDATE`, `DELETE`, or `NONE` operations during ingestion based on historical context[cite: 1].
* **Hybrid Vector-Graph Architecture:** Combines dense embeddings with Neo4j/Neptune relational knowledge graphs[cite: 1].
* **Plug-and-Play Connectors:** Supports Qdrant, Pgvector, Pinecone, Milvus, Chroma, Weaviate, OpenAI, Anthropic, and Groq[cite: 1].
* **Multi-Language SDKs:** Native Python SDK, Node.js/TypeScript client, REST API, and CLI binary[cite: 1].

---

## Best Use Cases

* **AI Coding Assistants:** Retain project architecture choices, library preferences, and local environment quirks across IDE restarts[cite: 1].
* **Autonomous AI Agents:** Provide long-term episodic and semantic memory for multi-agent workflows[cite: 1].
* **Personalized Support Copilots:** Remember user account history, past tickets, and technical proficiency[cite: 1].
* **Voice Calling AI Agents:** Ultra-fast context injection for low-latency voice pipelines[cite: 1].

---

## Compatibility

| AI Tool / Framework | Support Status | Integration Type |
| :--- | :---: | :--- |
| **Claude Code** | ✅ | Native MCP Server (`mem0-mcp`) |
| **Cursor** | ✅ | MCP Server / Python-Node Extension |
| **Codex** | ✅ | Open-source CLI / MCP Gateway |
| **Gemini CLI** | ✅ | Python SDK / REST Interface |
| **Continue** | ✅ | Custom Context Provider / MCP |
| **OpenCode** | ✅ | Native Plugin / MCP |
| **VS Code** | ✅ | Extension / MCP Server |
| **Windsurf** | ✅ | MCP Server |
| **Roo Code** | ✅ | MCP Server |

---

## Technology Stack

* **Core SDK:** Python 3.10+, TypeScript / ES2022
* **APIs & Protocols:** REST, Model Context Protocol (MCP), AsyncIO
* **Vector Store Drivers:** Qdrant, Pgvector, Pinecone, Chroma, Milvus, Redis, Weaviate
* **Graph Database Drivers:** Neo4j, AWS Neptune Analytics
* **LLM Adapters:** OpenAI, Anthropic, AWS Bedrock, Azure OpenAI, Google Vertex, Ollama

---

## Installation

### Python SDK
```bash
pip install mem0ai
```

---

## 📖 Interactive Technical Guide

Explore the hosted, full interactive HTML documentation guide:

👉 **[Open Mem0 Technical Guide (guide.html)](https://Shivanshu85.github.io/awesome-ai-skills/skills/memory/mem0/guide.html)**

Includes:
- Interactive System Architecture Diagram
- Complete Python & TypeScript Code Snippets
- Head-to-Head Comparison Table (Mem0 vs. Naive RAG vs. LangChain)
- Vector Store Driver & Configuration Options
- Best Practices, Anti-Patterns & Troubleshooting