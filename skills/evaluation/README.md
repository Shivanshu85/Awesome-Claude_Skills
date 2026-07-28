# Evaluation (`skills/evaluation/`)

Welcome to the **Evaluation** category index. This category documents prompt evaluation frameworks, LLM accuracy benchmarks, quality scoring tools, and evaluation datasets for AI software development.

---

## What is Evaluation?

Evaluation tools measure the factual accuracy, code compilation rate, instruction adherence, and token efficiency of AI assistant outputs. Instead of relying on subjective impressions, evaluation frameworks provide repeatable quantitative scoring.

---

## Why Evaluation Matters

- **Measures Real-World Assistant Quality**: Tests whether system prompt edits improve or degrade code accuracy.
- **Prevents Silent Degradation**: Detects prompt regression before deploying system prompts to team members.
- **Enables Benchmark Comparisons**: Compares performance across Claude, GPT-4o, and Gemini models.

---

## When to Use Evaluation

- When designing or updating system prompts for AI IDEs or custom agent frameworks.
- When selecting LLM models for specific software engineering tasks.
- When validating RAG retrieval precision for codebase search.

---

## Recommended Learning Order

1. **Assertion-Based Scoring**: Validating code output syntax, compilation, and unit tests.
2. **LLM-as-a-Judge Evals**: Using reference models to score instruction compliance.
3. **Automated Evaluation Pipelines**: Running eval suites in CI/CD pipelines.

---

## Related Categories

- 🧪 [skills/testing/](file:///skills/testing/README.md): Prompt regression testing and test suites.
- ✍️ [skills/prompt-engineering/](file:///skills/prompt-engineering/README.md): System prompt design and templates.
- 🔭 [skills/observability/](file:///skills/observability/README.md): Execution telemetry and logging.

---

## Documented Tools

Below are the open-source evaluation tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **PromptEval** | Automated prompt evaluation and accuracy benchmark framework | ✅ Active | *[View Guide](file:///skills/evaluation/README.md)* |
| **Ragas** | RAG evaluation framework measuring retrieval precision and fidelity | ✅ Active | *[View Guide](file:///skills/evaluation/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
