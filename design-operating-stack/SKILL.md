---
name: design-operating-stack
description: "Agent-facing design operating stack for taste-driven web and mobile UI: reference study, audit, generation, and systemization with object-first, mobile-native, anti-generic-SaaS rules."
version: 0.1.0
---

# Design Operating Stack

Design Operating Stack is a taste system for AI coding agents. It is not a
Hallmark fork. It is broader and sharper: web pages, mobile screens, reference
analysis, audits, generation rules, and future tooling all share one source of
truth.

The core stance: make interfaces feel made, operated, and physically specific.
Default AI SaaS layouts are the failure case.

## Modes

Route every request into one mode.

| Mode | Use when | Output |
| --- | --- | --- |
| `study` | The user gives screenshots, URLs, local images, or a reference folder. | Transferable design DNA, not copied pixels. |
| `audit` | The user asks why an existing UI feels weak, generic, or not sexy enough. | Ranked issues, taste-axis scoring, and repair directions. |
| `generate` | The user asks to build or redesign web or mobile UI. | A design plan or implementation using this stack. |
| `systemize` | The user wants new references folded into the rulepack. | New or updated rules, genres, patterns, or gates. |

If the user is ambiguous, ask one short question: "Study this reference, audit an
existing UI, or generate a new one?"

## File Loading

Load only the files needed for the current mode.

- Global principles: `references/taste-principles.md`
- Study flow: `references/reference-study.md`
- Audit flow: `references/audit-flow.md`
- Generation flow: `references/generation-flow.md`
- Rejection gates: `references/anti-slop-gates.md`
- Reference schema: `reference-dna/dna-schema.md`
- Current reference analysis: `reference-dna/refs-image-analysis.md`
- Genre choices: `genres/*.md`
- Mobile grammar: `mobile-patterns/*.md`
- Web grammar: `web-patterns/*.md`

Do not bulk-load every file unless the user asks for a full-stack review.

## Non-Negotiables

1. No pixel copying. Extract structure, taste, rhythm, and roles.
2. No fake proof. Do not invent metrics, testimonials, logos, awards, or users.
3. No generic SaaS default. The centered headline, paragraph, two buttons, and
   three rounded feature cards is a failure unless explicitly requested.
4. Mobile is first-class. A phone screen is not a narrow landing page.
5. Every strong output needs a dominant object: product render, phone surface,
   chart, timer, wordmark, card stack, dashboard, or typographic object.
6. Accent color has a footprint. It is a pin, signal, field, or flood.
7. Controls need states: default, pressed, focus, disabled, loading, error, and
   success when relevant.
8. Material surfaces need purpose: grain, blur, dot matrix, paper lines, chart
   grids, industrial blocks, or product shadows must support the concept.

## Mode Protocols

### study

1. Identify source type: screenshot, URL, local folder, or mixed set.
2. If a URL is private, auth-walled, or template-marketplace-like, ask for a
   screenshot or permission to diagnose only.
3. Load `references/reference-study.md` and `reference-dna/dna-schema.md`.
4. Classify the closest genre from `genres/`.
5. Extract surface, type, dominant gesture, object, mobile grammar, interaction
   stance, anti-patterns, and transferable rules.
6. Return DNA. Do not offer implementation until the diagnosis is clear.

### audit

1. Load `references/audit-flow.md`, `references/taste-principles.md`, and
   `references/anti-slop-gates.md`.
2. Score the UI on the audit axes.
3. Lead with findings, ordered by severity.
4. Name which genre or pattern would repair the weakness.
5. Do not edit unless the user asks to implement fixes.

### generate

1. Load `references/generation-flow.md`, `references/taste-principles.md`, and
   `references/anti-slop-gates.md`.
2. Decide whether the target is web, mobile, or both.
3. Pick one genre.
4. Pick one dominant gesture.
5. Pick one web or mobile pattern.
6. Define surface, type, accent footprint, and interaction stance.
7. Run anti-slop gates before emitting.
8. For code work, follow the host repo's framework and tokens first.

### systemize

1. Load `references/reference-study.md`, `reference-dna/dna-schema.md`, and the
   closest existing genre or pattern.
2. Decide whether the new reference creates a new genre, a variant, a component
   pattern, an anti-slop gate, or a one-off exception.
3. Update the smallest possible file.
4. Preserve the rulepack's boundaries: docs first, tooling later.

## Taste Shortlist

Start from these genre families:

- `genres/dark-technical-editorial.md`
- `genres/warm-institutional-serif.md`
- `genres/atmospheric-product-cinema.md`
- `genres/academic-handdrawn-editorial.md`
- `genres/industrial-swiss-object.md`
- `genres/mobile-kinetic-finance.md`

For mobile work, also load one pattern from `mobile-patterns/`.
For web work, also load one pattern from `web-patterns/`.

## Completion Check

Before claiming a design is ready, answer:

- What is the dominant object?
- What is the dominant gesture?
- What is the accent footprint?
- What surface material is doing real work?
- Which mobile or web pattern is active?
- Which anti-slop gates were most relevant?

If any answer is vague, revise before responding.
