# Decision Algorithm

> **Extract of `system/master-playbook.md` (sections 8, 11).** If this file and the playbook ever differ, the playbook wins. Edit the playbook first, then re-copy.

## 8. End-to-end generation algorithm

| # | Stage | Inputs | Decisions / actions | Output | Quality check |
| --- | --- | --- | --- | --- | --- |
| 1 | Interpret the brief | Brief, rubric, files, saved specs | Extract duration, speakers, minutes each, grading weights, research rule, deadline | Requirement list | Nothing in the brief unaccounted for |
| 2 | Audience and purpose | Requirement list | Audience level; what they must understand or decide | One-line objective | Objective is a claim, not a topic |
| 3 | Stress-test | Objective, constraints | Name the biggest risk; ask only questions that change the build | Risk + ≤ 2 questions | Opening line adds something new |
| 4 | Central argument | Source | Find the framework; pick one flagship per element | Spine + flagships | Each section maps to one element |
| 5 | Research | Spine | Read primary papers; find newer results; note caveats | Evidence notes with sources | Every planned number has a source |
| 6 | Architecture | Minutes, spine | Slide budget by minutes; dividers, summaries, critique, take-home | Slide list | Speaker minutes within range |
| 7 | Slide purposes | Slide list | One message per slide | Claim title per slide | Titles alone tell the story |
| 8 | Content | Evidence | Bullets, callouts, notes script | Draft slides | ≤ 4 bullets; units and comparisons |
| 9 | Visual forms | Content | Pick schematic / chart / table / cards / callouts | Visual per slide | No pasted multi-panel figure |
| 10 | Apply style | Style spec | Layouts, fonts, colours, navigator, footer | Built .pptx | Same title position on all content slides |
| 11 | Verify facts | Deck | Trace each number to its source | Flags for unverified values | No untraced number |
| 12 | Coherence | Deck | Read titles in order; check handovers | Fixed sequence | Each section ends with a handover |
| 13 | Consistency and density | Rendered slides | Fix overflow, overlaps, empty cards, wrapped titles | Clean render | No visible defect |
| 14 | Validate and deliver | Deck, rubric | Check every rubric item | File + 3–4 line message | Rubric items each served |

Missing information: choose a default and state it when cheap to redo; ask when expensive (format of a whole deck, team split, duration).

## 11. Self-critique and revision procedure

1. Render the deck to images and review it as a demanding examiner.
2. Fix layout first: overflow, overlaps, two-line titles, empty card space, colliding numbers.
3. Fix content next: catalogue slides, missing caveats, numbers without sources.
4. Re-render the changed slides.
5. In the delivery message: what still needs the user, plus the single biggest remaining risk.
