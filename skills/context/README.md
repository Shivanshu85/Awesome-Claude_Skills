# Context Management (`skills/context/`)

Welcome to the **Context Management** category index. This category documents techniques, tools, and protocols for maximizing context window utility, token compression, and sliding context mechanisms.

---

## Category Overview

Context window space is a finite resource. Context Management skills focus on token pruning, prompt compression, sliding history windows, and context serialization to maximize model recall while minimizing token costs.

For detailed domain boundaries and inclusion rules, see [docs/taxonomy.md](file:///docs/taxonomy.md#2-context-context-management).

---

## Target Audience

- Developers optimizing token budgets in LLM API calls.
- AI Engineers managing large context window limits in Cursor, Claude Code, or custom agent loops.
- Authors of context-packing tools.

---

## Recommended Learning Order

1. **Token Window Basics**: Understanding token counting, limits, and cost dynamics.
2. **Context Pruning**: Strategies for dropping low-relevance conversation turns.
3. **Semantic Compression**: AST and embedding-based context compression.

---

## Related Categories

- [skills/memory/](file:///skills/memory/README.md): Persistent multi-session memory systems.
- [skills/repository-intelligence/](file:///skills/repository-intelligence/README.md): Bundling codebase files into context.

---

## Contained Skills Index

*No skills are populated in this skeleton repository yet. Contributions welcome!*

To add a new skill to this category:
1. Review [CONTRIBUTING.md](file:///CONTRIBUTING.md).
2. Copy `templates/README.template.md` to `skills/context/<skill-slug>/README.md`.
3. Validate `metadata.json` against `schemas/metadata.schema.json`.

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
