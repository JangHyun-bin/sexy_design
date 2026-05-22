# Bottom Action System

## Use When

Use when a mobile screen needs persistent actions, bottom nav, confirmation,
transfer actions, tab actions, or reachable primary controls.

## Anatomy

- bottom safe-area container
- primary action
- secondary action or nav items
- selected state
- pressed state
- optional center action

## Layout Rules

- Respect the home indicator.
- Primary actions should be reachable by thumb.
- Separate navigation from destructive or confirming actions.
- Use stable height to avoid layout jumps.
- Do not crowd more than five actions.

## State Rules

- default: clear hierarchy
- pressed: visible compression, color shift, or surface change
- selected: persistent selected indicator
- disabled: visible but unavailable
- loading: keep bar stable and show progress
- error: show recovery near the action
- success: confirm without hiding the next action

## Motion Rules

- Bar can appear after scroll or stay fixed.
- State changes should be fast and tactile.
- Avoid large vertical jumps.

## Accessibility

- Minimum tap targets: 44 by 44 px.
- Icon-only actions need labels.
- Selected state must be announced.
- Do not rely on color alone.

## Anti-Slop Checks

- Fails if the bar floats decoratively with no state.
- Fails if buttons wrap or shift under loading text.
- Fails if destructive and primary actions look identical.
