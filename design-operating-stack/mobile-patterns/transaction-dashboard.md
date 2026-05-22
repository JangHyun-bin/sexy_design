# Transaction Dashboard

## Use When

Use for banking, crypto, expense, marketplace, ledger, and operational mobile
screens where lists and balances coexist.

## Anatomy

- account selector or search
- balance or primary metric
- quick actions
- transaction list
- filters or tabs
- bottom nav or bottom action

## Layout Rules

- The balance or primary metric should be visually dominant.
- Quick actions must be thumb-sized.
- Transaction rows should prioritize merchant, type, amount, and status.
- Use sheet depth to separate overview from details.

## State Rules

- default: current balance and recent transactions
- pressed: quick actions and rows respond
- loading: preserve layout and show row skeletons
- error: show retry without hiding balance context
- success: show completed transaction state
- empty: explain next action
- disabled: unavailable action is visible but muted

## Motion Rules

- Lists can slide or fade, not bounce.
- Balance changes can tick or crossfade.
- Sheet transitions should be short and directional.

## Accessibility

- Amounts need explicit currency labels.
- Positive and negative values need text or sign, not only color.
- Rows need accessible grouping.

## Anti-Slop Checks

- Fails if transaction list is generic lorem rows.
- Fails if chart or card data is fake.
- Fails if actions are tiny icon-only buttons without labels.
