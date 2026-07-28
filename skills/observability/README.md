# Observability (`skills/observability/`)

Welcome to the **Observability** category index. This category documents assistant tracing tools, token counters, execution telemetry dashboards, and logging framework for AI coding assistants and agent workflows.

---

## What is Observability?

Observability tools capture deep execution telemetry from AI interactions. They record token usage (prompt vs. completion), latency per step, tool execution spans, model costs, and full conversation traces to give developers visibility into AI system performance.

---

## Why Observability Matters

- **Tracks Token Expenditure**: Provides detailed breakdown of token costs by project, developer, or feature.
- **Pinpoints Performance Bottlenecks**: Identifies slow MCP server tool executions or bloated context steps.
- **Facilitates Post-Mortem Debugging**: Inspects exact prompt payloads and raw model responses during failures.

---

## When to Use Observability

- When deploying AI coding tools across development teams and tracking API cost allocation.
- When debugging latency issues or unexpected agent loops in multi-step workflows.
- When auditing tool call parameters and system prompt executions for security compliance.

---

## Recommended Learning Order

1. **Token Accounting & Metrics**: Tracking input/output token usage per session.
2. **Span Tracing**: Logging step-by-step assistant interactions and tool calls.
3. **Telemetry Dashboards**: Visualizing performance, latency, and cost trends over time.

---

## Related Categories

- 💰 [skills/token-optimization/](file:///skills/token-optimization/README.md): Input token economy and cost reduction.
- 🛡️ [skills/security/](file:///skills/security/README.md): Audit logging and tool security boundaries.
- 📊 [skills/evaluation/](file:///skills/evaluation/README.md): Performance evaluation and accuracy metrics.

---

## Documented Tools

Below are the open-source observability tools documented in this category:

| Tool Name | Primary Focus | Status | Tool Guide |
| :--- | :--- | :--- | :--- |
| **TokenTrace** | Token usage analytics and cost attribution library for LLMs | ✅ Active | *[View Guide](file:///skills/observability/README.md)* |
| **AgentSpan** | Open-telemetry span tracer for AI assistants and MCP tools | ✅ Active | *[View Guide](file:///skills/observability/README.md)* |

*To add a new tool to this category, review [CONTRIBUTING.md](file:///CONTRIBUTING.md) and copy `templates/README.template.md`.*

---

← [Root README](file:///README.md) | [Taxonomy Guide](file:///docs/taxonomy.md) →
