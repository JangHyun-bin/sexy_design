# Design Operating Stack

Design Operating Stack is an independent agent-facing rulepack for taste-driven
web and mobile UI. It was created because generic anti-slop landing page rules
are not enough for a sharper visual direction.

The stack favors object-first composition, large type, physical surfaces,
operational evidence, and mobile-native interaction grammar.

## What It Does

- Studies reference images and extracts transferable design DNA.
- Audits existing UI against a stricter taste system.
- Guides generation for web pages and mobile screens.
- Systemizes new references into reusable rules.

## How It Differs From Hallmark

Hallmark is primarily a landing-page anti-slop skill. This stack is wider:

- web and mobile are both first-class
- mobile screens have their own patterns
- reference DNA is meant to accumulate over time
- object, number, state, gesture, and material are core primitives
- generic SaaS patterns are treated as failure modes
- future CLI and visual-board tooling are planned but not required

## Folder Layout

```text
design-operating-stack/
  SKILL.md
  README.md
  references/
  genres/
  mobile-patterns/
  web-patterns/
  reference-dna/
  future-tools/
  docs/superpowers/
```

## Modes

Use `study` for references:

```text
study <private-reference-folder>/
```

Use `audit` for existing interfaces:

```text
audit this landing page against Design Operating Stack
```

Use `generate` for new UI:

```text
generate a mobile finance onboarding screen in the industrial/mobile kinetic direction
```

Use `systemize` when a new reference should become part of the rulepack:

```text
systemize these screenshots into the closest existing genre or a new variant
```

## V1 Status

V1 is markdown-first. There is no CLI and no visual board yet. Those are planned
in `future-tools/`, but the skill must remain useful without them.

## Current Reference Base

The first reference base is the local `<private-reference-folder>/` folder in the workspace. Its
analysis lives in `reference-dna/refs-image-analysis.md`.

## First Dogfood Example

The first generated concept lives in
`examples/mobile-kinetic-finance/index.html`. It tests the mobile finance side of
the stack with an oversized balance, card stack, transaction sheet, and bottom
action system.

## Shotgun Board

The first multi-direction comparison board lives in
`examples/mobile-shotgun-board/index.html`. It contains six mobile UI directions
in one HTML file and can be served locally with Python's static server.

The second-stage mutation board lives in
`examples/mobile-shotgun-board-v2/index.html`. It keeps the strongest V1
directions and deepens their state, touch, and operational logic.
