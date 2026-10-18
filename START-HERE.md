# Start Here: Restore the System in a New Chat

## Full recovery (recommended)
1. **Open a new conversation** with the AI you want to use.
2. **Paste `prompts/02-reconstruction-prompt.md`** (everything below its line).
3. **Provide `system/master-playbook.md`**: paste it where the prompt says, or attach the file.
4. **Provide supporting material if relevant:** `examples/gold-standard-presentations.md` for a similar talk; your institution's template or logos if you have them. The other `system/` files are already inside the playbook; you don't need to paste them.
5. **Ask the AI to confirm the rules:** "List the CONFIRMED rules you will follow and the TU Ilmenau style values, in under 15 lines." Check them against the playbook. If anything is wrong or invented, correct it before continuing.
6. **Give the brief:** fill in `prompts/04-slide-generation-prompt.md` and attach the source paper or document.
7. **Review the result** with `system/quality-checklist.md`. Optionally score it with `tests/presentation-evaluation.md`.
8. **Record corrections:** your exact words go in `examples/feedback-examples.md`. If a correction changes a rule, edit `system/master-playbook.md`, re-copy the affected extract files, and add a `CHANGELOG.md` entry.

## Minimal recovery (little context available)
1. Paste `prompts/03-compact-prompt.md`.
2. Paste your brief (fields from `prompts/04-slide-generation-prompt.md`).
3. Before accepting the result, check it against the five ★ items in `tests/recovery-test.md`: risk named first, framework spine, claim titles, no invented numbers, no false claims of memory.
4. Move to full recovery as soon as more context is available.

## First-time check
After restoring the first time, run `tests/recovery-test.md` once and log the score in `CHANGELOG.md`.
