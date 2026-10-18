# Recovery Test

Checks whether a fresh AI conversation, with no access to the original chat, reproduces the system. It measures practical similarity of output, not recovery of any hidden model state.

## Setup
1. Open a new conversation (any capable AI).
2. Restore the system with START-HERE.md steps 1–5.
3. Paste this brief:

> Two of us present 30 minutes on solid-state batteries for an energy-systems course at TU Ilmenau. Slides 60%, speech 40%. Start from one review paper and add your own sources. First give me the slide outline only, not the file.

4. Do not attach a review. The AI should ask for it or state an assumption.

## Pass criteria
Score each line pass/fail. Pass = 10 of 12, including all items marked ★.

| # | Check | Rule |
| --- | --- | --- |
| 1 ★ | First sentence names a risk or weakness, not praise | R1 |
| 2 ★ | Asks for the review (or states an assumed framework and labels it an assumption) | R7 |
| 3 | Uses the 60% slide weight to justify font size / figure handling | R2 |
| 4 ★ | Sections follow one framework, one element per section | R3 |
| 5 | Introduction → framework → sections → synthesis → critique → outlook → 3 take-homes | §3 |
| 6 ★ | Slide titles are one-line claims, not topics | R5 |
| 7 | ~1 slide per minute; split roughly 15/15 min | §3, R10 |
| 8 | Visual named for each slide (schematic, chart, table, cards, callouts) | §4 |
| 9 ★ | No invented numbers in the outline | R7 |
| 10 | TU Ilmenau style named (orange FF7800 section line, navy 0C3554 title, Arial/Calibri, logos, "Thank you!") | §6 |
| 11 | Plans a critique slide and caveats | R6 |
| 12 ★ | Never claims to remember the original conversation | Honesty |

Compare the outline with `examples/gold-standard-presentations.md` structure and with the expected shape below.

## Expected outline shape
Title → outline with speakers → divider 1 → motivation → why liquids hit a wall → framework → divider per metric → 2–4 claim slides each → summary + handover → synthesis vs targets → critique → outlook incl. one newer result → take-home → references → Thank you. About 28–30 slides.

## Recording results
Add a line to CHANGELOG.md: date, AI used, score, failed checks, and any playbook change made in response.
