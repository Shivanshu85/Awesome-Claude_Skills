# Memory Systems (`skills/memory/`)

Welcome to the **Memory Systems** category index. This category documents open-source memory frameworks, temporal knowledge graph engines, and state persistence protocols designed to give AI coding assistants long-term memory across sessions.

---

## What is Memory Systems?

Standard LLM interactions are stateless — every new chat or session clears context history. Memory Systems provide persistent key-value state, vector retrieval (RAG), and graph-based entity memory to preserve architectural decisions, past bug fixes, and developer coding preferences over extended project lifecycles.

---

## Why Memory Systems Matters

- **Eliminates Re-hydration Costs**: Stops developers from repeatedly explaining project conventions or architectural decisions.
- **Prevents Recurring Bugs**: Retains history of past bug resolutions and code refactoring choices.
- **Enables Multi-Session Agents**: Powers autonomous agentic workflows requiring persistent state retention.

---

## When to Use Memory Systems

- When working on large multi-week software engineering projects.
- When building multi-agent developer workflows where agents share state.
- When configuring personalized AI assistants that must remember developer coding styles.

---

## Recommended Learning Order

1. **Session State Retention**: Local key-value store state retention.
2. **Vector Memory (RAG)**: Storing embeddings of past developer interactions and code commits.
3. **Temporal Knowledge Graphs**: Advanced entity-relationship graphs for deep codebase relationship modeling.

---

## Related Categories

- 📦 [skills/context/](file:///skills/context/README.md): Context window assembly and token packing.
- 🔍 [skills/codebase-intelligence/](file:///skills/codebase-intelligence/README.md): Codebase indexing and AST symbol graphs.
- 🔌 [skills/mcp/](file:///skills/mcp/README.md): Model Context Protocol servers for memory tools.

---

## Documented Tools

Below are the open-source memory tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **[Mem0](file:///skills/memory/mem0/README.md)** | Universal memory layer for AI agents & coding assistants | ✅ Active | *[View Guide](file:///skills/memory/mem0/guide.html)* |
| **Graphiti** | Temporal knowledge graph memory engine | ✅ Active | *[View Guide](file:///skills/memory/README.md)* |
| **OpenMemory** | Local vector memory engine for session state retention | ✅ Active | *[View Guide](file:///skills/memory/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
