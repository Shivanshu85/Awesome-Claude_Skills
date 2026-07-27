# Central AI Terminology Glossary

To ensure single-source documentation and maintain consistency across all skill READMEs, core AI concepts and technical terminology are defined once in this central glossary.

Skill documentation pages should link directly to entries in this file (e.g., `[RAG](file:///docs/glossary.md#rag)`) rather than repeating generic definitions locally.

---

## Terms Index

- [Agent](#agent)
- [Context Window](#context-window)
- [Prompt Cache](#prompt-cache)
- [Embedding](#embedding)
- [RAG (Retrieval-Augmented Generation)](#rag-retrieval-augmented-generation)
- [MCP (Model Context Protocol)](#mcp-model-context-protocol)
- [Semantic Search](#semantic-search)
- [Knowledge Graph](#knowledge-graph)
- [Planner](#planner)
- [Reasoner](#reasoner)
- [Tool Calling](#tool-calling)
- [Context Compression](#context-compression)
- [Memory](#memory)

---

## Definitions

### Agent
An autonomous or semi-autonomous software loop driven by a Large Language Model (LLM) that can evaluate inputs, break down goals into sub-tasks, invoke external tools or APIs, inspect results, and iteratively solve problems without human intervention at every step.

### Context Window
The maximum token limit (including system instructions, conversation history, retrieved documents, tool outputs, and response budget) that an LLM can process within a single inference call.

### Prompt Cache
A hardware- or API-level optimization mechanism that stores pre-tokenized states of static prompt prefixes (such as system instructions or repository context), allowing faster inference latency and reduced token costs for repeated requests.

### Embedding
A dense numerical vector representation of text, code, or media in a continuous high-dimensional space, engineered such that semantically similar concepts reside physically close to one another.

### RAG (Retrieval-Augmented Generation)
An architecture that enhances LLM generation by retrieving relevant external facts, documentation, or code snippets from a database (vector, graph, or relational) and appending them into the model's context window prior to generating a response.

### MCP (Model Context Protocol)
An open, standardized protocol developed to enable secure, bi-directional communication between AI applications (clients) and external data sources, tools, and prompts (servers) over standard transport layers (stdio, SSE).

### Semantic Search
A search technique that uses vector embeddings and distance metrics (e.g., cosine similarity) to retrieve documents based on their underlying meaning and intent, rather than matching exact keyword strings.

### Knowledge Graph
A structured graph database representing real-world entities (nodes) and their semantic relationships (edges), enabling complex multi-hop queries and contextual reasoning over interconnected domain data.

### Planner
A dedicated LLM or prompt workflow responsible for analyzing a complex user request, decomposing it into an ordered Directed Acyclic Graph (DAG) of actionable sub-tasks, and defining verification criteria for each milestone.

### Reasoner
An LLM reasoning mode or structured prompt protocol (such as Chain-of-Thought or Tree-of-Thought) designed to systematically evaluate logical hypotheses, verify edge cases, and validate intermediate steps before outputting a final answer.

### Tool Calling
The capability of an LLM to recognize when an external function or API needs to be invoked, format a structured JSON call matching a predefined schema, and consume the tool's execution result back into its context window.

### Context Compression
The practice of reducing token count in prompt context through semantic summarization, AST filtering, prompt pruning, or embedding-based token selection while preserving crucial semantic information.

### Memory
The architectural subsystem responsible for storing, indexing, retrieving, and updating state information (such as user preferences, past decisions, conversation history, or codebase summaries) across multiple LLM interactions over time.
