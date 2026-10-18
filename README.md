# my-presentation-engine

A portable, version-controlled specification of how I want AI assistants to build presentations. It lets me restore the same way of working in any new AI conversation, even if the original chat is gone.

## What's inside

| Path | Purpose |
| --- | --- |
| `START-HERE.md` | Step-by-step recovery in a new chat |
| `CHANGELOG.md` | History of meaningful changes |
| `prompts/01-reverse-engineer.md` | Re-extracts the system from a chat after more training |
| `prompts/02-reconstruction-prompt.md` | Paste first in a new chat, with the playbook |
| `prompts/03-compact-prompt.md` | Short version for tools with little context |
| `prompts/04-slide-generation-prompt.md` | Fill-in brief for each new presentation |
| `system/master-playbook.md` | **Authoritative** specification |
| `system/*.md` (other files) | Extracts of the playbook by topic: algorithm, writing, visuals, evidence, checklist, conflicts, unknowns |
| `examples/` | Approved decks and real feedback |
| `tests/` | Recovery test and evaluation rubric |
| `backups/backup-and-restore.md` | GitHub setup, local and independent backups, privacy rules |

## How it works
The playbook labels every rule:
- **CONFIRMED** — I stated it or it's in my saved style spec.
- **INFERRED** — the assistant chose it in work I approved.
- **CONTEXT-DEPENDENT** — applies only in a stated context (e.g. TU Ilmenau talks).
- **UNKNOWN** — no evidence yet.

Current state (v1.0.0): built from one project, a graded three-person TU Ilmenau seminar. Communication preferences, the TU Ilmenau style and rubric-driven choices are confirmed; most structural rules are inferred. See `system/known-unknowns.md`.

## Usage
1. Restore: follow `START-HERE.md`.
2. For each deck: fill `prompts/04-slide-generation-prompt.md`.
3. Review: `system/quality-checklist.md`; score with `tests/presentation-evaluation.md`.
4. Improve: log feedback in `examples/feedback-examples.md`, update the playbook, record it in `CHANGELOG.md`.

## Maintenance principles
1. `system/master-playbook.md` is the single source of truth.
2. The other `system/` files are word-for-word extracts; they never introduce or change rules on their own.
3. Every new preference gets a label (confirmed, inferred, unknown, context-dependent).
4. A rule becomes CONFIRMED only after explicit feedback or consistent evidence across several decks.
5. Every significant change goes in `CHANGELOG.md` with a version number.
6. Approved decks are added to `examples/` with confidential material removed.
7. `prompts/03-compact-prompt.md` is re-checked after every playbook change.

## Setup
See `backups/backup-and-restore.md` for creating the private GitHub repository through the website, uploading, updating and keeping an independent backup. Keep the repository **private**.
