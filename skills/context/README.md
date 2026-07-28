# Context Management (`skills/context/`)

Welcome to the **Context Management** category index. This category documents tools and frameworks designed to optimize prompt context windows, assemble dynamic context payloads, and inject relevant documentation and code snippets into AI coding assistants.

---

## What is Context Management?

Context Management focuses on structuring, filtering, and assembling the information sent to an LLM prompt window. Instead of dumping arbitrary files into a prompt, context management tools select precisely the right files, documentation, and metadata needed for a specific coding task.

---

## Why Context Management Matters

- **Prevents Context Degradation**: Mitigates "lost in the middle" attention loss by keeping prompts clean and focused.
- **Reduces Unnecessary Token Inflation**: Eliminates irrelevancies before they enter the model context.
- **Improves Assistant Precision**: Ensures the model receives exact function signatures, dependency types, and active files.

---

## When to Use Context Management

- When working with complex codebases where full file injection exceeds token limits.
- When injecting external API documentation or library reference files dynamically into assistant context.
- When optimizing context assembly for Cursor, Claude Code, or IDE plugins.

---

## Recommended Learning Order

1. **Context Assembly Basics**: Understanding token budgets and context window limits.
2. **Dynamic Context Hydration**: Selective snippet and documentation injection.
3. **Automated Window Packing**: Multi-file context prioritization algorithms.

---

## Related Categories

- ⚡ [skills/context-compression/](file:///skills/context-compression/README.md): Prompt compression and token pruning.
- 💰 [skills/token-optimization/](file:///skills/token-optimization/README.md): Token economy and input cost reduction.
- 🔍 [skills/codebase-intelligence/](file:///skills/codebase-intelligence/README.md): Repository indexing and AST symbol graphs.

---

## Documented Tools

Below are the open-source context management tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **Context7** | Dynamic context window assembler for live docs and code snippets | ✅ Active | *[View Guide](file:///skills/context/README.md)* |
| **PromptPack** | Context payload bundler for multi-file IDE tasks | ✅ Active | *[View Guide](file:///skills/context/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
