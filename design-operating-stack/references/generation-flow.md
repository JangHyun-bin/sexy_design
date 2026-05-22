# Generation Flow

Use this when creating or redesigning UI.

## Step 1: Determine Target

Classify the request:

- web page
- mobile screen
- web plus mobile
- component only
- design system fragment

If unclear, ask one question.

## Step 2: Pick Surface Family

Choose one:

- dark technical
- warm paper
- cinematic atmosphere
- academic paper
- industrial gray
- mobile kinetic color

The surface must carry meaning. Do not pick a background for decoration only.

## Step 3: Pick Genre

Load one genre file from `genres/`.

The genre defines:

- when to use it
- type roles
- surface rules
- dominant gestures
- interaction stance
- avoid list

## Step 4: Pick Dominant Gesture

Pick one:

- giant wordmark
- object hero
- oversized number
- product screen
- chart or dashboard
- paper or diagram metaphor
- tactile mobile control
- card stack

Do not combine multiple primary gestures in the same first viewport.

## Step 5: Pick Type Role

Choose display, body, and label roles:

- display: editorial serif, giant grotesque, condensed technical sans,
  oversized numeric, engineered wordmark
- body: neutral sans, serif body, compact grotesque
- label: mono annotation, uppercase grotesque, small serif

## Step 6: Pick Accent Footprint

Choose one:

- pin
- signal
- field
- flood

Every accent use must match the selected footprint.

## Step 7: Pick Pattern

For web, load one file from `web-patterns/`.
For mobile, load one file from `mobile-patterns/`.

## Step 8: Pick Interaction Stance

Choose one:

- still and precise
- slow cinematic reveal
- tactile pressed controls
- scroll-synced object
- stateful dashboard
- kinetic number or time

Avoid bounce and hover-scale as default polish.

## Step 9: Run Anti-Slop Gates

Load `references/anti-slop-gates.md` and check the output before shipping.

## Generation Output

Before code, state:

```text
Target:
Genre:
Surface:
Dominant gesture:
Type roles:
Accent footprint:
Pattern:
Interaction stance:
Anti-slop risks:
```

Then implement within the user's existing stack.
