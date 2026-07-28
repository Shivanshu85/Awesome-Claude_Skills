# Changelog

All notable changes to the **Awesome-Claude_Skills** project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to Semantic Versioning where applicable to schemas and standards.

---

## [1.0.0] - 2026-07-27

### Added
- Initialized production-ready GitHub repository skeleton for **Awesome-Claude_Skills**.
- Created root landing page `README.md` with visual repository architecture map and category matrix.
- Established hybrid licensing model (`LICENSES/CC-BY-4.0.txt` for documentation, `LICENSES/MIT.txt` for schemas, templates, and tooling).
- Added core documentation infrastructure:
  - `docs/taxonomy.md`: Defined official 17 domain categories, scope, boundaries, and inclusion/exclusion rules.
  - `docs/glossary.md`: Established single-source definitions for core AI concepts (RAG, MCP, Context Window, Prompt Cache, Memory, Reasoning).
  - `docs/standards.md`: Created authoritative style guide for Markdown, Quick Facts tables, Mermaid layouts, and link integrity.
- Created JSON Schema validator `schemas/metadata.schema.json` (Draft 07).
- Created reusable skill generation templates in `templates/`:
  - `templates/README.template.md` (28 mandatory sections with navigation footer).
  - `templates/metadata.template.json` (Schema-compliant starter JSON).
  - `templates/workflow.template.mmd` (Mermaid flowchart starter).
- Created category landing pages across 17 domain directories (`skills/memory/`, `skills/mcp/`, `skills/context/`, etc.).
- Added community governance files: `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `.gitignore`, and GitHub issue/PR templates (`.github/`).
