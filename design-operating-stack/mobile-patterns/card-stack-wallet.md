# Card Stack Wallet

## Use When

Use for wallets, payment methods, subscriptions, passes, identity cards, account
selection, or object collections where the card itself is a stateful object.

## Anatomy

- stacked cards
- selected card
- amount or status
- card metadata
- paging indicator
- action sheet or bottom bar

## Layout Rules

- Selected card should overlap or rise above the stack.
- Metadata belongs close to the selected card.
- Use depth sparingly: shadow, blur, or scale, not all at once.
- Keep the card ratio stable across states.

## State Rules

- default: one card selected
- pressed: selected card responds
- dragging: cards track motion and expose next item
- disabled: unavailable card is visibly muted
- loading: avoid replacing cards with empty skeletons
- error: preserve selected card and explain the problem
- success: show confirmation near the selected card

## Motion Rules

- Drag should have snap points.
- Stack depth can change during drag.
- Page indicators must follow state.

## Accessibility

- Cards need accessible names.
- Swipe actions need button alternatives.
- Selected state must not rely on scale alone.

## Anti-Slop Checks

- Fails if cards are just decorative rectangles.
- Fails if selected state is unclear.
- Fails if card actions are outside thumb reach.
