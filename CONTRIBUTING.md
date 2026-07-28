# Contributing to Awesome-Claude_Skills

Thank you for your interest in contributing to **Awesome-Claude_Skills**! This repository is designed to be the canonical documentation library for AI Coding Skills across all AI models, IDEs, and frameworks.

To maintain professional quality and long-term sustainability as we scale to thousands of skills, every contribution must adhere strictly to these guidelines.

---

## Table of Contents

- [Repository Philosophy](#repository-philosophy)
- [How to Add a New Skill](#how-to-add-a-new-skill)
- [Folder & Slug Naming Rules](#folder--slug-naming-rules)
- [Documentation Standards](#documentation-standards)
- [Metadata Rules & Schema Validation](#metadata-rules--schema-validation)
- [Workflow Diagram Rules](#workflow-diagram-rules)
- [Pull Request Checklist](#pull-request-checklist)
- [Code of Conduct](#code-of-conduct)

---

## Repository Philosophy

Before contributing, keep our core principles in mind:

1. **Documentation-First**: We document AI skills; we do not write software implementations or tutorials here.
2. **Single Source of Truth**: All narrative information belongs inside a skill's single `README.md`. Never split content into separate `installation.md` or `troubleshooting.md` files.
3. **Derived PDFs**: Do not create or edit PDFs manually. PDFs (`<SkillName>-Guide.pdf`) are compiled automatically from the master `README.md`.
4. **Machine/Human Separation**: `README.md` is written for humans. `metadata.json` is written for machines (search, CLI, APIs, AI agents). Never copy narrative paragraphs into `metadata.json`.
5. **No Speculation**: Use verifiable facts and official documentation links. Do not invent benchmark numbers or unverified claims.

---

## How to Add a New Skill

Follow these steps to contribute a new skill:

### Step 1: Check Taxonomy
Review [docs/taxonomy.md](file:///docs/taxonomy.md) to identify the correct category for your skill (e.g., `memory`, `mcp`, `context`, `prompt-engineering`). If uncertain, open a [New Skill Request Issue](file:///.github/ISSUE_TEMPLATE/new_skill_request.yml).

### Step 2: Create Skill Folder
Create a directory under the selected category:
```bash
skills/<category>/<skill-slug>/
```
Example: `skills/memory/graphiti/`

### Step 3: Copy Templates
Copy the starter templates from the `templates/` directory:
- Copy `templates/README.template.md` to `skills/<category>/<skill-slug>/README.md`
- Copy `templates/metadata.template.json` to `skills/<category>/<skill-slug>/metadata.json`
- Copy `templates/workflow.template.mmd` to `skills/<category>/<skill-slug>/workflow.mmd`

### Step 4: Populate Skill Files
1. Fill out `README.md` following all 28 mandatory sections. Do not alter section names or order.
2. Fill out `metadata.json` with machine keywords, tags, supported platforms, and URLs.
3. Edit `workflow.mmd` to model the skill flow (`Input -> Processing -> Core Components -> Output -> Result`).

### Step 5: Render Workflow SVG
Compile `workflow.mmd` to `workflow.svg` using standard Mermaid tools (e.g., `@mermaid-js/mermaid-cli`).

### Step 6: Validate Metadata
Validate `metadata.json` against `schemas/metadata.schema.json` to ensure zero schema errors.

### Step 7: Submit Pull Request
Open a PR using [.github/PULL_REQUEST_TEMPLATE.md](file:///.github/PULL_REQUEST_TEMPLATE.md).

---

## Folder & Slug Naming Rules

- **Lowercase Hyphenated**: Folder names must use lowercase alphanumeric characters separated by hyphens (kebab-case).
  - ✅ `graphiti`
  - ✅ `memory-bank`
  - ✅ `github-mcp`
  - ❌ `Graphiti_Skill` (no uppercase or underscores)
  - ❌ `01-graphiti` (never use numeric prefixes)
- **Self-Contained**: Every skill directory must contain exactly:
  ```
  skills/<category>/<skill-slug>/
  ├── README.md
  ├── metadata.json
  ├── workflow.mmd
  ├── workflow.svg
  ├── <SkillName>-Guide.pdf  (compiled export)
  └── LICENSE
  ```

---

## Documentation Standards

All README files must strictly follow the section structure defined in [templates/README.template.md](file:///templates/README.template.md) and style rules in [docs/standards.md](file:///docs/standards.md):

- **Quick Facts Table**: Placed immediately after the `# <Skill Name>` title. Contains 13 standardized fields.
- **Section Order**: Overview, Quick Facts, Problem Statement, Why this Skill Exists, When Should You Use It, When Should You NOT Use It, Key Features, Architecture Overview, Workflow Overview, Installation, Configuration, Supported Platforms, Supported AI Models, Supported IDEs, Usage (Basic & Advanced), Real-World Use Cases, Performance Notes, Comparison Table, Advantages, Limitations, Best Practices, Common Mistakes, Troubleshooting, Security Considerations, Related Skills, References, FAQ, License, Contributors.
- **Glossary Linking**: Use definitions in [docs/glossary.md](file:///docs/glossary.md) for terms like RAG, MCP, Context Window, and Prompt Cache instead of redefining them locally.
- **Tone**: Professional, clear, objective, and factual. Avoid marketing hype, excessive exclamation marks, or unnecessary emojis.

---

## Metadata Rules & Schema Validation

`metadata.json` powers search engines, CLI utilities, and AI indexing.

- Must strictly adhere to `schemas/metadata.schema.json`.
- `slug` must match the directory name.
- `category` must match the parent folder name.
- Keep description under 200 characters.
- Do not repeat full paragraphs from `README.md`.

Validate locally:
```bash
npx ajv-cli validate -s schemas/metadata.schema.json -d skills/<category>/<skill-slug>/metadata.json
```

---

## Workflow Diagram Rules

- Source file is `workflow.mmd`.
- Diagram must use top-down (`TD`) layout.
- Standard flow layout:
  ```mermaid
  graph TD
      Input["Input Layer"] --> Processing["Processing Engine"]
      Processing --> Core["Core Components"]
      Core --> Output["Output Handler"]
      Output --> Result["Final Result"]
  ```
- Keep node labels clear and concise.
- Output SVG must be named `workflow.svg`.

---

## Pull Request Checklist

Before submitting a PR, verify:

- [ ] Folder name follows kebab-case without numbers or special characters.
- [ ] `README.md` contains all 28 required sections in exact order.
- [ ] Quick Facts table is complete with all required properties.
- [ ] Terms link to [docs/glossary.md](file:///docs/glossary.md) where appropriate.
- [ ] `metadata.json` validates clean against `schemas/metadata.schema.json`.
- [ ] `workflow.mmd` compiles cleanly to `workflow.svg`.
- [ ] Navigation links (`← Previous Skill | Category Home | Next Skill →`) are correctly configured.
- [ ] Category `README.md` is updated to index the new skill.
- [ ] No extra or extraneous files are included in the skill folder.

---

## Code of Conduct

All contributors are expected to uphold our [CODE_OF_CONDUCT.md](file:///CODE_OF_CONDUCT.md). Please report unacceptable behavior to security or repository maintainers.
