# Prompt 01: Reverse-Engineer a Presentation System

Use this in a conversation where you have trained an AI on presentations and want to extract the system again (for example, to update this repository after several new decks). This is the exact prompt used to create the current version.

---

# REVERSE-ENGINEER MY PERSONAL PRESENTATION SYSTEM

## Role

Act as an expert prompt engineer, presentation architect, behavioral analyst, and AI workflow reverse engineer.

Throughout this conversation, I have trained you through instructions, examples, feedback, corrections, revisions, and repeated interactions to create presentations according to my specific preferences.

Your task is to reconstruct that trained presentation-generation method as a detailed, portable, executable specification.

Do not give me a generic presentation guide. Recover the specific system that I have developed with you.

## 1. Analyze all accessible conversation history

Extract and document my preferences concerning:

- Presentation objectives, audience, and communication philosophy.
- Narrative structure, storytelling, and logical progression.
- Slide sequencing, slide count, and information distribution.
- Slide titles, headlines, key messages, supporting arguments, and takeaways.
- Writing style, tone, vocabulary, sentence structure, and content density.
- Visual design, layouts, typography, colors, spacing, and visual hierarchy.
- Charts, tables, diagrams, images, illustrations, and other visual elements.
- Research methods, data accuracy, citations, and source quality.
- PowerPoint production, formatting, speaker notes, and other deliverables.
- My repeated corrections, rejected approaches, accepted outputs, and recurring instructions.
- Rules for handling ambiguity, missing information, conflicting requirements, and revisions.

Look for explicit instructions, repeated patterns, and implicit decision rules.

Use the full accessible conversation history to the extent available. Do not claim to have analyzed content you cannot access.

## 2. Reconstruct my actual decision-making process

Determine not only WHAT I prefer, but HOW the presentation should be constructed.

For every important rule, explain:

1. The rule itself.
2. When the rule applies.
3. Why it matters.
4. How to implement it.
5. How to check whether it has been followed.
6. What mistakes to avoid.

Convert abstract preferences into practical, actionable instructions.

For example, replace vague guidance such as "make slides compelling" with concrete criteria for strong headlines, logical argument progression, appropriate evidence, visual communication, and useful conclusions, based on my actual feedback.

Do not treat illustrative examples as established personal preferences unless the conversation supports them.

## 3. Classify the evidence

Label findings as:

- CONFIRMED: Explicitly stated or repeatedly demonstrated.
- INFERRED: Supported by recurring behavior but not explicitly stated.
- UNKNOWN: Insufficient evidence to determine my preference.
- CONTEXT-DEPENDENT: Changes according to topic, audience, or deliverable.

When preferences conflict, prioritize explicit instructions and later corrections where appropriate. Document unresolved conflicts instead of silently inventing a solution.

## 4. Build the complete presentation algorithm

Create an executable workflow covering:

1. Interpret the brief.
2. Determine the audience, purpose, and desired outcome.
3. Identify the central argument or narrative.
4. Research and verify necessary evidence.
5. Design the slide architecture.
6. Define the purpose of every slide.
7. Generate slide headlines and content.
8. Select appropriate visual forms and layouts.
9. Apply my writing and design rules.
10. Verify factual accuracy and source quality.
11. Review narrative coherence and slide-to-slide transitions.
12. Check visual consistency, information density, and redundancy.
13. Critique and revise weak slides.
14. Validate the final deliverable against my requirements.

For each stage, specify inputs, decisions, actions, outputs, and quality checks.

## 5. Produce the master playbook

Create a document titled:

MY PERSONAL PRESENTATION GENERATION SYSTEM

Include:

- Executive summary.
- Core presentation principles.
- Confirmed preferences and inferred rules.
- Content and narrative architecture.
- Slide-generation rules.
- Writing and language conventions.
- Visual design specifications.
- Research and evidence standards.
- End-to-end generation algorithm.
- Mandatory constraints and prohibited practices.
- Quality-control checklist.
- Self-critique and revision procedure.
- Conflict-resolution rules.
- Context-dependent adaptations.
- Known limitations and unresolved questions.

Make it self-contained. Avoid references such as "as discussed earlier." Include the actual rules.

## 6. Produce a reconstruction prompt

Create a separate prompt that I can paste into a brand-new AI conversation alongside the master playbook.

It must instruct the new AI to:

- Treat the playbook as the authoritative specification of my presentation preferences.
- Follow the documented generation workflow.
- Preserve confirmed rules while handling inferred rules cautiously.
- Ask clarifying questions only when genuinely necessary.
- Apply my preferences to future topics and briefs.
- Review its output against the quality checklist.
- Correct obvious weaknesses before delivering the result.
- Never pretend to remember the original conversation.
- Never fabricate missing preferences or undocumented rules.

The prompt must be operational, not merely descriptive.

## 7. Create a compact version

Produce a concise version of the presentation system for situations where context or prompt length is limited.

It must preserve the highest-priority rules and tell the AI to consult the complete playbook whenever available.

## 8. Create a validation test

Design a hypothetical presentation topic that is not merely copied from an example in the conversation.

Use the reconstructed system to produce a proposed slide outline. Explain how the documented rules influenced the narrative, headlines, content, and visual choices.

Identify any assumptions that the test required.

## 9. Final output requirements

Return these deliverables in clearly separated sections:

A. Master playbook.
B. New-chat reconstruction prompt.
C. Compact reconstruction prompt.
D. Quality-control checklist.
E. Validation test.
F. Outstanding unknowns and missing evidence.

Make every deliverable independently copyable and saveable as a Markdown file.

If the complete output is too long, divide it into numbered parts and continue until every deliverable is complete.

Do not omit important details simply to keep the answer short.

## Final objective

I want to preserve the presentation-generation system I have developed with you so that, if this conversation disappears, I can reconstruct the closest possible equivalent in a new chat with Claude or another AI.

Start by analyzing the accessible conversation. Then generate the complete deliverables.
