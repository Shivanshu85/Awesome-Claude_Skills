# Testing (`skills/testing/`)

Welcome to the **Testing** category index. This category documents prompt regression testing suites, dynamic assertion libraries, and unit testing frameworks for AI coding assistant prompts.

---

## What is Testing?

Testing tools bring traditional software engineering rigor to AI prompts and agent workflows. They allow developers to write automated test suites that run prompts against input scenarios and assert expected behavior, code formatting, and tool execution.

---

## Why Testing Matters

- **Prevents Prompt Breakage**: Ensures system prompt edits do not break existing tool calls or code generation capability.
- **Enables CI/CD Validation**: Integrates prompt testing directly into GitHub Actions or local pre-commit hooks.
- **Validates Edge Cases**: Verifies that AI assistants handle invalid inputs, missing context, or boundary conditions cleanly.

---

## When to Use Testing

- When maintaining shared `.cursorrules` or system prompt repositories for development teams.
- When updating MCP server tool descriptions or argument schemas.
- When building autonomous AI agents that perform automatic code refactoring.

---

## Recommended Learning Order

1. **Unit Testing Prompts**: Writing deterministic test cases for system instructions.
2. **Regression Suite Automation**: Running prompt tests automatically on code pushes.
3. **Mocking MCP Tool Responses**: Simulating environment responses for test isolation.

---

## Related Categories

- 📊 [skills/evaluation/](file:///skills/evaluation/README.md): LLM quality benchmarks and evals.
- ✍️ [skills/prompt-engineering/](file:///skills/prompt-engineering/README.md): System prompt design.
- 🔄 [skills/agent-workflows/](file:///skills/agent-workflows/README.md): Reasoning protocols and verification loops.

---

## Documented Tools

Below are the open-source testing tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **PromptTest** | Unit testing and regression framework for LLM prompts | ✅ Active | *[View Guide](file:///skills/testing/README.md)* |
| **ToolAssert** | Assertions library validating tool call arguments and sequences | ✅ Active | *[View Guide](file:///skills/testing/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
