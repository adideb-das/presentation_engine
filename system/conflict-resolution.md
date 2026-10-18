# Conflict Resolution

> **Extract of `system/master-playbook.md` (sections 12, 13).** If this file and the playbook ever differ, the playbook wins. Edit the playbook first, then re-copy.

## 12. Conflict-resolution rules

1. The user's latest explicit instruction.
2. Rubric or formal brief requirements.
3. Saved institutional style spec (for that institution).
4. Standing communication preferences.
5. INFERRED rules in this playbook.
6. General good practice.

Known conflict: "terse, concise" vs requests for full deliverables (a 48-slide deck, this playbook). Resolution: the requested deliverable gets full depth; the chat message around it stays terse.

## 13. Context-dependent adaptations

| Context | Adaptation | Status |
| --- | --- | --- |
| TU Ilmenau talk | Full style spec in Section 6 | CONFIRMED |
| Other institution or company | Ask for their template or state a neutral palette | UNKNOWN |
| Solo vs team | Team: shared template, split by framework, ownership warning | INFERRED |
| Short talk (≤ 20 min) | One flagship per element; others to backup | INFERRED |
| Long talk (45–50 min) | Secondary examples get their own slides | INFERRED |
| Non-specialist audience | Fewer equations, more analogies | UNKNOWN |
| Graded vs ungraded | Weight by rubric when graded | CONFIRMED (graded) |

## Precedence between repository files

1. `system/master-playbook.md` is authoritative.
2. Files in `system/` are extracts of it and must match it word for word.
3. `prompts/` must not introduce rules that are not in the playbook. `prompts/03-compact-prompt.md` is a summary and must be re-checked whenever the playbook changes.
4. `examples/` show rules applied; they never override the playbook.
