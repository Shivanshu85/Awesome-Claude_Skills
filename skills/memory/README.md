# Memory Systems (`skills/memory/`)

Welcome to the **Memory Systems** category index. This category documents skills, frameworks, and protocols designed to give AI coding assistants and autonomous agents persistent memory across sessions.

---

## Category Overview

Standard LLM interactions are stateless—each prompt reset clears previous context. Memory Systems provide graph memory, vector retrieval, and state persistence to preserve code insights, architectural decisions, and developer preferences over long development cycles.

For detailed domain boundaries and inclusion rules, see [docs/taxonomy.md](file:///docs/taxonomy.md#1-memory-memory-systems).

---

## Target Audience

- AI Systems Engineers building agentic workflows requiring multi-session state.
- Developers looking to eliminate context re-hydration costs in complex codebases.
- Maintainers integrating knowledge graph RAG into IDE assistants.

---

## Recommended Learning Order

1. **Stateful Session Memory**: Basics of key-value and local state retention.
2. **Vector Memory & RAG**: Storing embeddings of past developer interactions.
3. **Graph-Based Knowledge Memory**: Advanced temporal entity graphs for deep code relationship modeling.

---

## Related Categories

- [skills/context/](file:///skills/context/README.md): Token window optimization and context packing.
- [skills/repository-intelligence/](file:///skills/repository-intelligence/README.md): Codebase AST parsing and symbol graph extraction.
- [skills/mcp/](file:///skills/mcp/README.md): Model Context Protocol servers for memory tools.

---

## Contained Skills Index

*No skills are populated in this skeleton repository yet. Contributions welcome!*

To add a new skill to this category:
1. Review [CONTRIBUTING.md](file:///CONTRIBUTING.md).
2. Copy `templates/README.template.md` to `skills/memory/<skill-slug>/README.md`.
3. Validate `metadata.json` against `schemas/metadata.schema.json`.

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
