# Context Compression (`skills/context-compression/`)

Welcome to the **Context Compression** category index. This category documents algorithms, small language model compressors, and prompt reduction techniques designed to compress long contexts without losing key semantic intent.

---

## What is Context Compression?

Context Compression uses specialized algorithms or small language models (SLMs) to analyze raw prompts and prune low-information tokens, repetitive prose, and redundant boilerplate before passing the compressed prompt to a primary LLM.

---

## Why Context Compression Matters

- **Drastically Lowers API Spending**: Reduces token payloads by up to 20x, saving thousands of dollars on long-context queries.
- **Speeds Up Inference Time**: Smaller prompts result in faster Time-To-First-Token (TTFT) and overall model response times.
- **Enhances Model Attention**: Removes noise, allowing the LLM to focus on critical constraints and code logic.

---

## When to Use Context Compression

- When feeding massive logs, stack traces, or documentation into an LLM prompt.
- When processing long-context repositories or multi-file prompts.
- When operating under strict API cost budgets or rate limits.

---

## Recommended Learning Order

1. **Rule-Based Truncation**: Whitespace, comment, and AST node stripping.
2. **SLM Prompt Compression**: Using models like LLMLingua to score and prune tokens.
3. **Long-Context Attention Tuning**: Applying LongLLMLingua to preserve critical context positioning.

---

## Related Categories

- 💰 [skills/token-optimization/](file:///skills/token-optimization/README.md): Input token economy and cost reduction.
- 📦 [skills/context/](file:///skills/context/README.md): Context window assembly and token packing.
- ✍️ [skills/prompt-engineering/](file:///skills/prompt-engineering/README.md): System prompt design and efficiency.

---

## Documented Tools

Below are the open-source context compression tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **LLMLingua** | SLM-based prompt compression reducing tokens up to 20x | ✅ Active | *[View Guide](file:///skills/context-compression/README.md)* |
| **LongLLMLingua** | Compression tuned for long-context LLMs to prevent attention loss | ✅ Active | *[View Guide](file:///skills/context-compression/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
