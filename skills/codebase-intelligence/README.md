# Codebase Intelligence (`skills/codebase-intelligence/`)

Welcome to the **Codebase Intelligence** category index. This category documents repository packing utilities, AST parsers, codebase mappers, and symbol graph tools that enable AI assistants to navigate large codebases efficiently.

---

## What is Codebase Intelligence?

Codebase Intelligence tools extract structural meaning from software repositories. Instead of treating code as unstructured plain text, these tools analyze Abstract Syntax Trees (AST), symbol import/export graphs, file trees, and git histories to provide compact, highly informative repository representations for LLM prompts.

---

## Why Codebase Intelligence Matters

- **Solves Cross-File Dependency Bottlenecks**: Helps AI assistants understand how functions, classes, and types relate across hundreds of files.
- **Reduces Context Payload Size**: Packs repositories into clean, single-file representations formatted specifically for LLM context windows.
- **Accelerates Code Navigation**: Enables instant symbol lookup without scanning thousands of lines of irrelevant code.

---

## When to Use Codebase Intelligence

- When onboarding AI assistants to large, multi-directory legacy repositories.
- When packing a repository into a single file for Claude Code, ChatGPT, or Gemini context windows.
- When generating codebase summaries, architecture maps, or AST dependency graphs.

---

## Recommended Learning Order

1. **Repository Packing Basics**: Using tools like Repomix to generate single-file codebase context.
2. **AST Symbol Extraction**: Extracting function signatures, type definitions, and interface maps.
3. **Graph-Based Code Search**: Building dependency graphs for multi-repo cross-referencing.

---

## Related Categories

- 📦 [skills/context/](file:///skills/context/README.md): Context window assembly and token packing.
- 🔌 [skills/mcp/](file:///skills/mcp/README.md): Model Context Protocol servers for codebase access.
- 🧠 [skills/memory/](file:///skills/memory/README.md): Knowledge graph RAG and memory systems.

---

## Documented Tools

Below are the open-source codebase intelligence tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **Repomix** | Packed codebase representation tool designed for LLM context windows | ✅ Active | *[View Guide](file:///skills/codebase-intelligence/README.md)* |
| **RepoPrompt** | Interactive codebase prompt generator and repository packer | ✅ Active | *[View Guide](file:///skills/codebase-intelligence/README.md)* |
| **ASTGrapher** | AST symbol graph extractor for cross-file dependency mapping | ✅ Active | *[View Guide](file:///skills/codebase-intelligence/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
