# Changelog

Version numbers: MAJOR.MINOR.PATCH.
- **MAJOR** — a CONFIRMED rule is removed or reversed.
- **MINOR** — a rule is added, or its label changes (e.g. INFERRED → CONFIRMED).
- **PATCH** — wording, typos, layout; no rule change.

## Entry format
```markdown
## [X.Y.Z] - YYYY-MM-DD
### Changed rules
- R5 claim titles: INFERRED → CONFIRMED (feedback: "[exact words]", see examples/feedback-examples.md)
### Added / Removed
- ...
### Files touched
- system/master-playbook.md, system/writing-rules.md, prompts/03-compact-prompt.md
### Tests
- Recovery test: [AI], [score]/12
```

## [1.0.0] - 2026-10-18
### Added
- Initial system reconstructed from the TU Ilmenau van der Waals materials seminar project (October 2026).
- Master playbook with 13 core rules (R1–R13), labelled CONFIRMED / INFERRED / CONTEXT-DEPENDENT / UNKNOWN.
- Reconstruction, compact, slide-generation and reverse-engineering prompts.
- Topic extracts in `system/`, quality checklist, recovery test, evaluation rubric, backup guide.
- One gold-standard example (approved) and four real feedback entries.
### Known gaps
- No corrections recorded yet; most structural rules are INFERRED. See `system/known-unknowns.md`.
- Logo files not included.
