## Description

Briefly describe the new skill or documentation update being submitted.

- **Skill Category**: `skills/<category>/`
- **Skill Slug**: `<skill-slug>`

---

## Skill Checklist

Please verify the following requirements before submitting:

- [ ] Folder is located at `skills/<category>/<skill-slug>/` using kebab-case with no numeric prefixes.
- [ ] `README.md` strictly follows all 28 mandatory sections in the exact order specified in [templates/README.template.md](file:///templates/README.template.md).
- [ ] Quick Facts table is fully populated with accurate, verified information.
- [ ] Terms link to definitions in [docs/glossary.md](file:///docs/glossary.md) where applicable.
- [ ] `metadata.json` validates clean against [schemas/metadata.schema.json](file:///schemas/metadata.schema.json).
- [ ] `workflow.mmd` uses the standard `TD` layout (`Input -> Processing -> Core -> Output -> Result`).
- [ ] `workflow.svg` is compiled and renders clearly.
- [ ] Navigation footer (`← Previous Skill | Category Home | Next Skill →`) is included and links work.
- [ ] Category landing page (`skills/<category>/README.md`) has been updated to index this skill.
- [ ] No extraneous files (e.g. `installation.md`, `troubleshooting.md`) are present in the skill folder.

---

## Verification

Describe how you validated `metadata.json` and compiled `workflow.svg`:

```bash
# Example validation command run:
npx ajv-cli validate -s schemas/metadata.schema.json -d skills/<category>/<skill-slug>/metadata.json
```
