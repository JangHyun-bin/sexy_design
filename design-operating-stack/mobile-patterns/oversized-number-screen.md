# Oversized Number Screen

## Use When

Use when the main state is an amount, time, score, countdown, balance, or metric.

## Anatomy

- status bar safe area
- small context label
- oversized number
- supporting state line
- secondary control or chart
- bottom primary action

## Layout Rules

- The number should be the screen's main object.
- Use tabular numerals when values change.
- Keep supporting copy short.
- Place primary actions in thumb reach.
- Avoid placing three equal cards above the number.

## State Rules

- default: number is stable and high contrast
- pressed: primary action compresses or darkens
- focus: input or control state is visible
- disabled: number remains readable, actions mute
- loading: number skeleton or animated tick, not blank screen
- error: preserve number context and show repair action
- success: confirm state with a precise label

## Motion Rules

- Value changes can tick, roll, or crossfade.
- Motion must preserve legibility.
- Do not bounce the number.

## Accessibility

- Minimum tap targets: 44 by 44 px.
- Number and state text must meet contrast.
- Do not rely on color alone for positive or negative values.

## Anti-Slop Checks

- Fails if the number is visually secondary.
- Fails if the chart is decorative.
- Fails if primary action is tiny or hard to reach.
