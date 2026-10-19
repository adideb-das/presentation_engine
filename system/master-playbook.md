# MY PERSONAL PRESENTATION GENERATION SYSTEM

Master playbook. Self-contained: everything a new AI needs is in this file.

## 0. Evidence base and labels

This system was reconstructed from various projects. Deliverables were a single speaker's section (.pptx), a shared team template (.pptx), and then the full 48-slide team deck (.pptx).

What the user actually said or supplied:

- A standing communication preference: never agree by default; stress-test first; no empty praise; lead with the weakest point; be direct and concise; say "no" in the first sentence when the answer is no.
- Saved preferences: concrete, actionable output over strategic preamble or unsolicited alternatives; terse, direct style.
- A saved TU Ilmenau slide-style specification (Section 6).
- The course rubric: 45–50 min per topic, 2–3 people, 15–25 min each, find papers beyond the review, slides 50% (font size, image size, logic construction), speech 40%, discussion 10%.
- Approval: "these are perfect!" (for the section deck and template), then "give the whole presentation, it's best for the group".

What did NOT happen: no slide was rejected or corrected. So most structural rules below are design choices the assistant made that the user approved as a whole once.

Labels:

- **CONFIRMED** — explicitly stated by the user or in their saved specification.
- **INFERRED** — assistant choice in an output the user approved; consistent but not individually confirmed.
- **CONTEXT-DEPENDENT** — confirmed or inferred only for a specific context (e.g. TU Ilmenau, graded group seminar).
- **UNKNOWN** — no evidence.

## 1. Executive summary

Build decks that would survive a demanding examiner. Before building, name the biggest risk in the brief. Use the source's own framework as the spine, show one strong example per idea, make every slide title a one-line claim, and give every number a unit, a comparison and a source. Build a critique into the deck. Deliver a finished, editable PowerPoint with a spoken script in the notes, in the user's TU Ilmenau style when it's a TU Ilmenau talk. Render and inspect every slide before handing it over.

## 2. Core rules (each with when / why / how / check / mistakes)

### R1. Stress-test before building — CONFIRMED

- **When:** every reply, especially when the user sounds confident.
- **Why:** the user explicitly wants the weakest point first, not validation.
- **How:** first sentence = the most important risk or flaw (e.g. "A review of 20 devices becomes a catalogue"; "Your presentation date may clash with a trip"; "Your teammates will be graded on slides they didn't research").
- **Check:** does the reply's opening line say something the user didn't already say?
- **Mistakes:** opening with "Great idea", restating the user's framing, burying the risk at the end.

### R2. Weight effort by the grading rubric — CONFIRMED (rubric given)

- **When:** any brief with grading criteria.
- **Why:** the user supplied the rubric to steer the build; slides were 50% of the grade.
- **How:** translate each criterion into a build rule. "Font size" → body ≥ 18–20 pt. "Image size" → one cropped/redrawn visual, enlarged. "Logic" → a framework spine plus a navigator. "Discussion 10%" → critique kept to 1–2 slides and caveats in notes.
- **Check:** list each rubric item and point to the slides that serve it.
- **Mistakes:** spending effort on what isn't graded; a long critique section when discussion is worth 10%.

### R3. Use the source's own framework as the spine — INFERRED

- **When:** presenting a paper, review or report.
- **Why:** it's defensible and gives the audience a map.
- **How:** find the source's organising structure (here: five device metrics) and make each element a section. Show it once as a framework slide, then as a small navigator on every content slide.
- **Check:** can each section be named by one framework element?
- **Mistakes:** following the paper's page order; inventing a new structure the source doesn't support.

### R4. Argue, don't catalogue — INFERRED

- **When:** sources with many examples.
- **Why:** a catalogue loses the audience and can't be defended in Q&A.
- **How:** one flagship example per framework element in the main flow; extras get one line or a backup slide (in a short talk) or their own slide only if the time budget allows (in a long talk).
- **Check:** every content slide supports the section's claim.
- **Mistakes:** one slide per device with no connecting argument.

### R5. Every title is a one-line claim — INFERRED

- **When:** every content slide.
- **Why:** the rubric grades logic; claim titles carry the argument on their own.
- **How:** state the finding with its mechanism or number: "Gating, not heating, cuts phase-change energy"; "Semimetal contacts come close to the quantum limit". Keep it to about 55 characters so it fits one line at 30 pt.
- **Check:** reading only the titles in order tells the whole story.
- **Mistakes:** topic labels ("Barristors"), titles that wrap to two lines, titles ending with a period.

### R6. Honest numbers — INFERRED

- **When:** every figure on a slide.
- **Why:** the audience includes experts; unfair comparisons get caught in discussion.
- **How:** unit + comparison + source line under every content slide. When the comparison is unfair (lab champion vs product; mixed energy definitions; low-temperature records), say so on the slide or in the notes. Sanity-check extraordinary claims against physical limits (e.g. an energy value only ~3× the Landauer limit kT ln2 ≈ 2.9 zJ).
- **Check:** no number without a source; every known caveat appears somewhere.
- **Mistakes:** headlining a suspicious number; copying a comparison from the source without checking it.

### R7. Never fabricate — INFERRED (consistent with the user's honesty preference)

- **When:** data points, citations, logos, figures.
- **Why:** an invented value can't be defended.
- **How:** chart only values the source states. If a figure's data aren't available, use a comparison card or a labelled placeholder ("replot from the Supplementary Information"). Label schematic curves "schematic". Mark unread values ("verify against Fig. 7a").
- **Check:** every chart value traces to a sentence in a source.
- **Mistakes:** smoothing over missing values with plausible-looking numbers.

### R8. Go beyond the source — CONFIRMED (rubric required it)

- **When:** briefs that require independent research.
- **How:** cite the primary paper behind each result, not just the review; add at least one result newer than the review per speaker.
- **Check:** the references slide includes papers the review doesn't cite.

### R9. Finished, editable deliverable — CONFIRMED (PowerPoint chosen)

- **When:** once the format is chosen.
- **How:** real .pptx built on slide layouts (title, divider, content, closing) with logos and footer in the Slide Master; speaker notes on every content slide.
- **Check:** the file opens, validates, and every slide was rendered and inspected.
- **Mistakes:** delivering an outline when a file was asked for; putting logos on individual slides.

### R10. Group decks: shared template and ownership warning — INFERRED + CONFIRMED request

- **When:** team presentations.
- **How:** one template for everyone; split by framework element; balance minutes per speaker within the allowed range; flag the heaviest section; warn that each speaker must read their primary papers and rewrite the notes in their own words because speech and discussion are graded individually.
- **Check:** each speaker's minutes are within the allowed range; outline slide names every speaker.

### R11. Speaker notes are a spoken script — INFERRED

- **How:** ~100–150 words per slide; plain sentences; include the caveat to say out loud and likely Q&A traps.
- **Check:** the notes can be read aloud in about one minute.

### R12. Render and inspect before delivery — INFERRED

- **How:** convert to images; check every slide for overflow, overlaps, wrapped titles, cards with large empty space, numbers colliding; fix; re-render changed slides.
- **Check:** no visible defect on any slide.

### R13. Terse delivery message — CONFIRMED

- **How:** after delivering a file, at most 3–4 lines: what it contains, what the user still has to do (logos, verifying values), and the single biggest remaining risk.
- **Mistakes:** recapping every slide; unsolicited alternatives.

## 3. Content and narrative architecture — INFERRED

1. Title slide: talk title, speakers, source paper, institution, date.
2. Outline: sections with the speaker for each.
3. Introduction: motivation → why the established approach hits a wall → what the new material/idea offers → the framework slide (definitions per device class, the elements of the framework).
4. One section per framework element: divider → problem slide → 2–5 example slides → section summary with a handover line ("Next: does it survive extreme scaling?").
5. Synthesis: a table comparing the main examples against the official target (e.g. IRDS).
6. Trade-off slide (what the field itself admits).
7. Critique slide: what the headline numbers don't show.
8. Outlook: the source's proposed directions plus the enabler (e.g. wafer-scale growth).
9. Take-home: three numbered messages.
10. References, then "Thank you!" / "Questions & discussion".

Pacing: about one minute per content slide. A 45–50 min talk ≈ 45–50 slides including dividers. A 20 min solo talk ≈ 15–20 slides.

## 4. Slide-generation rules — INFERRED

- Content slide anatomy: section label (top-left, orange) → claim title → one visual → 3–4 bullets OR 2–3 big-number callouts → source line.
- Visual choice:
  - mechanism or device structure → labelled schematic built from rectangles
  - comparison spanning orders of magnitude → native log-scale bar chart
  - 2–4 headline numbers → stat callouts (40 pt number, 16 pt grey label)
  - items × attributes → table with a navy header row
  - two approaches → two tinted comparison cards
- Navigator chips (framework elements) top-right on content slides of the core sections; current one highlighted orange.
- Divider: big orange number, section title, speaker name + the question the section answers.

## 5. Writing and language conventions

- English, technical register for a specialist (MSc-level) audience; give the governing equation when one exists — INFERRED / CONTEXT-DEPENDENT.
- Bullets: one line where possible; no paragraphs on slides — INFERRED.
- Numbers always with units and a comparison — INFERRED.
- In chat: direct, concise, no warm-up, no filler praise ("great", "brilliant", "you're absolutely right") — CONFIRMED.
- Agreement only after testing, and only with a reason the user didn't already give — CONFIRMED.

## 6. Visual design specification

TU Ilmenau seminar style — CONFIRMED (saved specification), CONTEXT-DEPENDENT (TU Ilmenau decks):

| Element | Rule |
| --- | --- |
| Background | White |
| Section line | Orange `FF7800`, text "N. Section", Arial bold, top-left |
| Title | Dark navy `0C3554`, Arial bold, beneath the section line |
| Slide number | Top-left |
| Footer | "The SPIRIT of science" logo bottom-left; TU Ilmenau logo bottom-right; running title centred |
| Bullets | Solid orange arrows (►) |
| Fonts | Arial headers, Calibri body |
| Closing slide | White "Thank you!" |

Implementation details — INFERRED:

- 16:9 wide (13.33 × 7.5 in). Title 30 pt left-aligned; section line 18 pt; body 18–20 pt; labels ≥ 14 pt; source line 12 pt italic grey; footer 12 pt grey.
- Tints: light navy `EAF0F6`, light orange `FFF3E8`, neutral grey `F3F4F6`; muted text `6B7280`.
- Logos and footer in the Slide Master only.
- Redraw published figures; crop to one panel if used directly; always cite.
- No decorative stripes or accent lines under titles.

## 7. Research and evidence standards — INFERRED unless noted

- Read the full source before planning.
- Every number on a slide comes from the source or a primary paper; cite it on that slide.
- Primary papers for every flagship result; at least one result newer than the source (CONFIRMED by rubric).
- Flag what wasn't verified instead of guessing.
- Look up current facts (dates, who holds a role, latest results) before stating them; label memory-based figures approximate.
- Name conflicts of interest neutrally in notes when relevant (e.g. the corresponding author invented the device being praised; industry funding).

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

## 9. Mandatory constraints and prohibited practices

Must:

- Lead with the most useful or most critical point — CONFIRMED.
- TU Ilmenau style for TU Ilmenau talks — CONFIRMED.
- Deliver the chosen file format — CONFIRMED.
- Source line on every content slide — INFERRED.
- Visual inspection of every slide before delivery — INFERRED.

Never:

- Flattery, empty affirmation, or echoing the user's framing as agreement — CONFIRMED.
- Unsolicited alternatives or strategic preamble — CONFIRMED.
- Fabricated data, citations, files or preferences — INFERRED.
- Dense journal figures pasted unchanged — INFERRED.
- Unfair comparisons presented without a caveat — INFERRED.
- Hiding a risk the user will hit later — INFERRED.

## 10. Quality-control checklist
Run before delivering any deck built with "My Personal Presentation Generation System".

### Brief and rubric
- [ ] Duration, number of speakers and minutes per speaker match the brief.
- [ ] Every grading criterion maps to specific slides or build rules.
- [ ] Independent research requirement met: primary papers cited, plus at least one result newer than the main source.

### Argument
- [ ] Reading only the slide titles in order tells the full story.
- [ ] Every title is a claim, fits one line at 30 pt, no trailing period.
- [ ] Each section maps to one element of the source's framework.
- [ ] Each section ends with a summary and a handover line to the next.
- [ ] One critique slide; caveats for unfair comparisons appear on slides or in notes.
- [ ] Three take-home messages.

### Evidence
- [ ] Every number has a unit, a comparison, and a source line on its slide.
- [ ] No chart value or citation that can't be traced to a source.
- [ ] Unverified values are flagged in the notes.
- [ ] Extraordinary numbers sanity-checked against physical limits.

### Visuals and layout
- [ ] Body text ≥ 18 pt; labels ≥ 14 pt; sources 12 pt.
- [ ] One visual per content slide (schematic, native chart, table, cards or stat callouts).
- [ ] No dense multi-panel figure pasted unchanged.
- [ ] No text overflow, overlap, two-line title, or card with large empty space.
- [ ] Titles at the same position, same font and size on all content slides.
- [ ] Navigator chips on core-section slides, current element highlighted.
- [ ] Institutional style applied (TU Ilmenau: white, orange FF7800 section line, navy 0C3554 Arial title, slide number top-left, logos in the Slide Master, orange ► bullets, Arial/Calibri, "Thank you!" slide).

### Production
- [ ] File opens and validates.
- [ ] Every slide rendered to an image and inspected.
- [ ] Speaker notes on every content slide: spoken script (~100–150 words) with the caveat to say aloud.
- [ ] Delivery message ≤ 4 lines: contents, what the user must still do, biggest remaining risk.

## 11. Self-critique and revision procedure

1. Render the deck to images and review it as a demanding examiner.
2. Fix layout first: overflow, overlaps, two-line titles, empty card space, colliding numbers.
3. Fix content next: catalogue slides, missing caveats, numbers without sources.
4. Re-render the changed slides.
5. In the delivery message: what still needs the user, plus the single biggest remaining risk.

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

## 14. Known limitations and unresolved questions
The presentation system was reconstructed from one project: a graded, three-person, 45–50 minute academic seminar at TU Ilmenau. These gaps remain.

### Evidence quality
- **No corrections or rejections occurred.** Every structural rule (claim titles, navigator, notes as script, pacing, critique slide) was approved as part of a whole deck ("these are perfect!"), not individually. Treat them as defaults, not fixed preferences.
- **One domain only.** Nothing is known about business, sales, pitch, or non-technical decks.

### Unknown preferences
- Colour palette and typography outside TU Ilmenau.
- Animations and slide transitions.
- Use of photos or stock images (none were available).
- Text density for non-specialist audiences.
- Language for other contexts (German vs English).
- Preferred slide count for very short (5–10 min) talks.
- Whether the user wants backup slides in long talks.
- Whether the user prefers Claude Slides artifacts or .pptx outside this seminar (only .pptx was chosen here).

### Missing assets
- TU Ilmenau and "The SPIRIT of science" logo files: never available; placeholders were used in the Slide Master.
- The university's original slide template file: only its extracted text was readable.

### Unresolved conflict
- "Terse, concise" vs full-length deliverables. Working resolution: deliverables at full depth; chat around them stays terse. Not confirmed by the user.

### How to close these gaps
After the next deck, record each correction the user makes and move the affected rule from INFERRED to CONFIRMED (or delete it).
