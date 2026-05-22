# Design Operating Stack - Design Spec

Date: 2026-05-22
Status: approved for specification, pending implementation
Workspace: `D:\HB\Rhizome\sexy_design`
Target folder: `design-operating-stack/`

## Goal

Build an independent agent-facing design operating stack. It is not a Hallmark fork.
It should give an AI coding agent a stronger taste system for web and mobile UI:
reference study, UI audit, generation rules, mobile interaction grammar, and a future
path toward CLI or visual-board tooling.

The first usable artifact is a document-based skill/rulepack. It should work before
any CLI, browser board, or automation exists.

## Why This Exists

Hallmark is useful as an anti-slop landing page skill, but it is too broad and too
conventional for this taste direction. The reference set points to a more specific
visual language:

- object-first heroes instead of generic hero-copy-card compositions
- large brand gestures: wordmarks, numbers, product objects, charts, and controls
- material surfaces: grain, halftone, blur, dot matrix, paper lines, industrial gray
- restrained accent systems with one dominant color move
- operational sexiness: dashboards, specs, financial states, alarm controls, timelines
- mobile screens treated as first-class design objects, not only responsive outputs

## Non-Goals For V1

- Do not copy any reference image pixel-for-pixel.
- Do not build a CLI in V1.
- Do not build the visual board in V1.
- Do not modify the existing `hallmark/` repo.
- Do not create a generic SaaS landing generator.
- Do not make a theme catalogue that only swaps colors.

## V1 Deliverable

Create a standalone folder:

```text
design-operating-stack/
  SKILL.md
  README.md
  references/
    taste-principles.md
    reference-study.md
    generation-flow.md
    audit-flow.md
    anti-slop-gates.md
  genres/
    dark-technical-editorial.md
    warm-institutional-serif.md
    atmospheric-product-cinema.md
    academic-handdrawn-editorial.md
    industrial-swiss-object.md
    mobile-kinetic-finance.md
  mobile-patterns/
    oversized-number-screen.md
    tactile-control-surface.md
    card-stack-wallet.md
    alarm-time-picker.md
    transaction-dashboard.md
    bottom-action-system.md
  web-patterns/
    object-first-hero.md
    giant-wordmark-hero.md
    cinematic-product-fold.md
    editorial-logo-wall.md
    operational-dashboard-surface.md
  reference-dna/
    refs-image-analysis.md
    dna-schema.md
  future-tools/
    cli-plan.md
    visual-board-plan.md
```

V1 is complete when an agent can read `SKILL.md`, route a user request, load only
the needed references, and produce a taste-aligned study, audit, or generation plan.

## Core Modes

### study

Extract design DNA from screenshots, URLs, or local reference folders. Output should
describe transferable structure, not copyable pixels.

Required output:

- source summary
- genre classification
- surface system
- type roles
- object or hero gesture
- mobile grammar if present
- reusable components
- anti-patterns to avoid
- candidate build rules

### audit

Evaluate an existing UI against this taste system.

The audit must prioritize:

- generic SaaS structure
- weak object presence
- weak type hierarchy
- fake polish such as blobs, glows, and unmotivated cards
- mobile screens that feel like compressed web pages
- controls without tactile state logic
- too many accent colors
- fabricated metrics, logos, testimonials, or proof

### generate

Generate or guide a web/mobile UI using the stack.

Generation must start by choosing:

- surface family
- genre
- dominant gesture
- type pairing role
- accent footprint
- web or mobile pattern
- interaction stance

### systemize

Convert new references into reusable rules.

This mode should update the mental model, not blindly append examples. It should
ask whether a new reference creates:

- a new genre
- a variant of an existing genre
- a new component pattern
- a new anti-slop gate
- a one-off exception that should not become a rule

## Reference DNA From Current Images

The initial folder `<private-reference-folder>/` contains 17 screenshots. The set clusters into six
families.

### Dark Technical Editorial

Reference signal: Reference A.

Traits:

- black paper
- white serif display
- mono or uppercase labels
- dotted grid and hairline frames
- small hot orange accent
- dashboard or command-center surface
- logos and metrics presented as operational proof

Transferable rule:

Use darkness, precision, and restrained heat. The page should feel like a control
room, not like a generic AI SaaS landing page.

### Warm Institutional Serif

Reference signal: Reference B.

Traits:

- ivory paper
- rust red flood sections
- large editorial serif
- clinical or institutional trust signals
- logo wall and stat strip
- blurred warm media
- calm, high-trust pacing

Transferable rule:

Make authority feel human and institutional. Avoid futuristic medical AI cliches.

### Atmospheric Product Cinema

Reference signal: Reference C.

Traits:

- dark landscape or cinematic backdrop
- cyan, lavender, purple, and green light
- product mockup as the main scene
- soft modern sans
- black lower sections
- sparse copy

Transferable rule:

Sell the product as a place or mood first, then explain it.

### Academic Hand-Drawn Editorial

Reference signal: Reference D.

Traits:

- off-white paper
- large serif headline
- hand-drawn illustration
- university logo proof
- blue notebook surface
- lined paper metaphor
- friendly academic intelligence

Transferable rule:

Use intelligence without making it sterile. The interface should feel studied,
human, and paper-adjacent.

### Industrial Swiss Object

Reference signal: References E and F.

Traits:

- giant wordmark or engineered logotype
- black, white, gray
- mono technical annotations
- huge product object
- extreme negative space
- minimal navigation
- high physicality

Transferable rule:

Let the object carry authority. Copy should annotate, not decorate.

### Mobile Kinetic Finance

Reference signal: alarm, wallet, banking, crypto screens.

Traits:

- oversized numbers
- tactile controls
- pill buttons and bottom actions
- card stacks
- phone-native surfaces
- dot matrix and timer systems
- one bold accent move: yellow, red, blue, or lavender
- stateful screens over static compositions

Transferable rule:

Mobile UI must feel operated. Screens should expose state, time, amount, selection,
motion, or gesture.

## Taste Principles

### 1. Object First

Every strong output needs a dominant object, not just a layout:

- product render
- phone surface
- card stack
- chart system
- clock or number
- wordmark
- handwritten illustration
- dashboard surface

If no object exists, the design must create a typographic object.

### 2. One Dominant Gesture

Each first viewport gets exactly one primary visual move:

- one giant wordmark
- one oversized number
- one product object
- one cinematic screenshot
- one flood color
- one paper/diagram metaphor

Secondary elements must support the move.

### 3. Accent Footprint Discipline

Accent color must be assigned a footprint:

- pin: below 3 percent of viewport
- signal: 3 to 10 percent
- field: 10 to 35 percent
- flood: above 35 percent

Do not use accent color casually. It must have a role.

### 4. Material Surface

Flat color is not enough unless the type or object is doing all the work. Prefer
motivated surfaces:

- grain
- halftone
- dot matrix
- lined paper
- frosted blur
- product shadow
- chart grid
- industrial gray block

### 5. Type As Product

Typography must behave as part of the product experience. Display type can be:

- editorial serif
- giant grotesque
- condensed technical sans
- mono annotation
- oversized numeric
- engineered wordmark

Generic Inter-style hierarchy is not enough on its own.

### 6. Operational Sexiness

Interfaces should show work happening:

- transactions
- charts
- tasks
- timers
- alarms
- card states
- workflow runs
- specs
- controls

Decoration should be backed by state, data, or interaction.

### 7. Mobile Is Not A Shrunk Website

Mobile patterns must be designed around:

- thumb zones
- bottom action systems
- dynamic type and numbers
- sheet and card depth
- state transitions
- input focus states
- device-safe spacing

## Anti-Slop Gates

V1 should define gates that reject:

- centered SaaS hero with paragraph, two buttons, and three feature cards by default
- purple-blue gradient blobs without product reason
- rounded cards used as filler
- fake browser chrome
- fake metrics
- fake testimonials
- generic logo walls with no brand context
- hover scale as the only interaction
- mobile layouts that are only stacked desktop sections
- too many accent colors
- decorative charts that do not encode anything
- buttons without pressed, disabled, loading, and success states
- product screenshots framed as decoration rather than evidence

## Implementation Strategy

V1 should be implemented as documentation first:

1. Create the folder and baseline files.
2. Write `SKILL.md` as a router with four modes: study, audit, generate, systemize.
3. Write the initial reference DNA from `<private-reference-folder>/`.
4. Write the six genre files.
5. Write the mobile pattern files.
6. Write the web pattern files.
7. Write anti-slop gates.
8. Add future plans for CLI and visual board without implementing them.

## Future CLI

The future CLI can provide:

- `dos study <private-reference-folder>/`
- `dos audit <url-or-path>`
- `dos generate --mode mobile --genre industrial-swiss-object`
- `dos board <private-reference-folder>/`

The CLI should consume the same markdown rules rather than inventing a second
source of truth.

## Future Visual Board

The visual board can show:

- reference thumbnails
- detected genre
- color footprint
- dominant gesture
- extracted patterns
- accepted rules
- rejected slop patterns

This is a future convenience layer. The skill must remain useful without it.

## Open Decisions

- Final package name: `design-operating-stack` is a working name.
- Whether to use a shorter invocation alias such as `dos`.
- Whether Korean explanations should be included in the files or only in chat.
- Whether V1 should include generated example HTML screens or stay purely rule-based.

## Acceptance Criteria

- The new stack lives outside `hallmark/`.
- The stack has explicit web and mobile coverage.
- The initial 17 screenshots are represented as DNA, not copied.
- The skill can study, audit, generate, and systemize.
- The mobile rules are first-class, not appended as responsive guidance.
- The rulepack rejects generic AI/SaaS visual defaults.
- Future CLI and board plans are documented but not implemented in V1.

