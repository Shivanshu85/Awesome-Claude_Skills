# AI Optimization Glossary & Terminology Index

This glossary provides single-source definitions for core AI context optimization, token economy, memory, and protocol concepts used across **Awesome-Claude_Skills**.

---

## Terminology Index

### Context Window
The maximum number of tokens (input prompt + output completion) an LLM can process in a single inference call. Optimizing context window usage prevents attention loss and token inflation.

### Model Context Protocol (MCP)
An open specification that standardizes how AI models discover and execute local tools, inspect resources, and load system prompts. MCP replaces ad-hoc wrappers with standardized stdio and SSE transports.

### Prompt Compression
The process of reducing input token count using rule-based pruning, AST parsing, or small language model (SLM) compression (e.g. LLMLingua) without altering the underlying semantic meaning of instructions.

### Retrieval-Augmented Generation (RAG)
An architecture that retrieves relevant document or code snippets from an external knowledge base or vector database and injects them into the model's prompt context prior to generation.

### Graph Memory
A persistent memory architecture that stores entities, code concepts, and architectural relationships as nodes and edges in a temporal graph (e.g. Graphiti), allowing agents to retain long-term state across sessions.

### Sequential Thinking
A multi-step reasoning protocol where an AI assistant dynamically formulates, tests, revises, and verifies hypotheses before generating code edits.

### AST Parsing
Abstract Syntax Tree parsing converts raw source code into a structured syntax tree, allowing AI tools to extract function signatures, interfaces, and import graphs while discarding formatting boilerplate.

### Prompt Injection
A security vulnerability where untrusted input text overrides system prompt instructions, forcing the LLM assistant to execute unauthorized actions or bypass safety guardrails.

### Prompt Caching
A provider-level optimization (e.g., Anthropic Prompt Caching) that caches static prompt prefixes (like system prompts and codebase maps) to reduce latency and lower input token costs by up to 90%.

### Token Economy
The engineering discipline of minimizing input and output token consumption to reduce API expenses while maintaining maximum output quality and precision.
