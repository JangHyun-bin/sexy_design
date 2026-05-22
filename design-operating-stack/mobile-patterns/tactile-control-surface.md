# Tactile Control Surface

## Use When

Use for sliders, toggles, scrubbers, alarm controls, transfer controls, filters,
and any screen where touch manipulation is the product.

## Anatomy

- control field
- selected state
- handle, knob, or thumb
- scale, ticks, or grid
- immediate feedback label
- confirm or cancel action

## Layout Rules

- Controls need enough physical area for a thumb.
- Use visual affordance: rails, ticks, holes, raised cards, or shadow.
- Keep secondary text away from the manipulation zone.
- Bottom actions should not collide with the system home indicator.

## State Rules

- default: clear resting position
- pressed: surface visibly depresses or grips
- dragging: value follows touch without lag
- disabled: control communicates non-interactive state
- loading: lock control and explain why
- success: show final selected value
- error: preserve previous value and show repair path

## Motion Rules

- Use snap, drag, or inertial movement.
- Movement should feel physical, not decorative.
- Avoid spring bounce unless the product is playful.

## Accessibility

- Provide textual value output.
- Support keyboard or stepper fallback when applicable.
- Do not require precision dragging for critical actions.

## Anti-Slop Checks

- Fails if it looks like a static illustration.
- Fails if pressed and disabled states are missing.
- Fails if feedback text updates after the motion rather than during it.
