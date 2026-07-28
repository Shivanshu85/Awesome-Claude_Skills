# Token Optimization (`skills/token-optimization/`)

Welcome to the **Token Optimization** category index. This category documents token economy tools, input optimization techniques, whitespace/AST pruning utilities, and cost reduction strategies for AI coding workflows.

---

## What is Token Optimization?

Token Optimization involves engineering input prompts, system instructions, and codebase payloads to consume the minimal possible number of tokens while preserving 100% of functional logic and instructions required by the LLM.

---

## Why Token Optimization Matters

- **Direct Cost Savings**: Every token saved directly reduces monthly LLM API invoices.
- **Higher Throughput**: Lower token payloads allow more queries within rate limits (RPM/TPM).
- **Cleaner Model Outputs**: Well-structured, token-efficient inputs lead to clearer, more deterministic code outputs.

---

## When to Use Token Optimization

- When deploying AI coding assistants across large development teams.
- When running automated CI/CD code review bots that process hundreds of PRs daily.
- When building CLI companions or background agent loops.

---

## Recommended Learning Order

1. **Token Cost Modeling**: Calculating input vs. output token economics.
2. **Structural Pruning**: Stripping redundant comments, formatting whitespace, and unused imports.
3. **Prompt Cache Optimization**: Structuring prompts to maximize provider prompt caching hits.

---

## Related Categories

- ⚡ [skills/context-compression/](file:///skills/context-compression/README.md): Algorithmic prompt compression.
- 🔍 [skills/codebase-intelligence/](file:///skills/codebase-intelligence/README.md): Efficient repository packing and AST extraction.
- ✍️ [skills/prompt-engineering/](file:///skills/prompt-engineering/README.md): Structured prompt design.

---

## Documented Tools

Below are the open-source token optimization tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **TokenPrune** | AST-aware code & whitespace token minimizer | ✅ Active | *[View Guide](file:///skills/token-optimization/README.md)* |
| **CacheOptimizer** | Provider prompt cache layout optimizer | ✅ Active | *[View Guide](file:///skills/token-optimization/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
