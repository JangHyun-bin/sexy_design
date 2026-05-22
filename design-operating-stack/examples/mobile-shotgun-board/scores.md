# Mobile Shotgun Board Scores

Scored with `reference-dna/taste-rubric.md`.

## Ranking

| Rank | Variant | Score | Decision |
| ---: | --- | ---: | --- |
| 1 | A. Night Wallet | 7.8 | Keep and mutate |
| 2 | F. Ops Console | 7.5 | Keep and mutate |
| 3 | C. Swiss Vault | 7.3 | Keep and mutate |
| 4 | B. Acid Alarm | 6.9 | Ingredient, not direction yet |
| 5 | D. Notebook Pay | 6.5 | Ingredient, needs stronger state |
| 6 | E. Care Ledger | 6.3 | Ingredient, too trust-page-like |

## A. Night Wallet

Score: 7.8 / 10

Keep:

- Oversized balance creates immediate mobile object authority.
- Card stack and transaction sheet are recognizably phone-native.
- Dot matrix plus blue card gives material surface.

Weak:

- Transaction rows are still generic.
- Card stack is visually strong but not yet interaction-rich.
- Accent role is split between red markers and blue depth.

Next mutation:

- Make the card stack and balance feel connected by a state: selected card changes available balance and transaction context.
- Add a bottom transfer composer or card detail snap state.

Reject if:

- It drifts into ordinary fintech dashboard rows.

Axis scores:

```text
Object Authority: 4
Surface Quality: 4
Mobile Nativeness: 4
Type Sexiness: 4
Accent Discipline: 3
Operational Evidence: 4
Interaction Promise: 4
Anti-Slop Resistance: 4
Desire: 4
```

## B. Acid Alarm

Score: 6.9 / 10

Keep:

- Yellow flood is memorable.
- Time is clearly the object.
- Ruler control implies tactile interaction.

Weak:

- The product category is narrow unless time/scheduling is central.
- Secondary card feels underdeveloped.
- It needs a clearer before/after state.

Next mutation:

- Turn it into a full scheduling system: drag ruler, next alarm preview, conflict warning, confirm state.

Reject if:

- The yellow field becomes the only idea.

Axis scores:

```text
Object Authority: 4
Surface Quality: 3
Mobile Nativeness: 4
Type Sexiness: 4
Accent Discipline: 5
Operational Evidence: 3
Interaction Promise: 4
Anti-Slop Resistance: 4
Desire: 3
```

## C. Swiss Vault

Score: 7.3 / 10

Keep:

- Industrial object authority is clear.
- Sparse annotations are strong.
- Orange CTA has a precise signal role.

Weak:

- It is more brand object than usable app screen.
- Needs an actual wallet or security state.
- The circular object risks feeling decorative if not tied to function.

Next mutation:

- Convert the object into a custody/security control: locked, armed, confirming, or verified state.
- Add spec rows that respond to the selected asset or vault mode.

Reject if:

- It remains a product poster inside a phone.

Axis scores:

```text
Object Authority: 5
Surface Quality: 4
Mobile Nativeness: 2
Type Sexiness: 4
Accent Discipline: 4
Operational Evidence: 3
Interaction Promise: 3
Anti-Slop Resistance: 5
Desire: 4
```

## D. Notebook Pay

Score: 6.5 / 10

Keep:

- Paper and serif tone are distinct from fintech defaults.
- The assistant/notes direction can be useful for planning.

Weak:

- Mobile state is not strong enough.
- The note panel is too static.
- Object authority is mostly typographic.

Next mutation:

- Make it a spending-plan assistant with a visible decision state: ask, compare, approve, save.

Reject if:

- It becomes only an editorial poster.

Axis scores:

```text
Object Authority: 3
Surface Quality: 4
Mobile Nativeness: 2
Type Sexiness: 4
Accent Discipline: 3
Operational Evidence: 2
Interaction Promise: 2
Anti-Slop Resistance: 4
Desire: 3
```

## E. Care Ledger

Score: 6.3 / 10

Keep:

- Warm institutional tone is a useful trust direction.
- Rust flood and serif type work together.

Weak:

- It reads closer to a landing-page section than a mobile app screen.
- It lacks touchable state.
- Proof language needs real data or placeholders.

Next mutation:

- Make it a care budget approval screen with claims, beneficiaries, and a bottom confirmation system.

Reject if:

- It stays as a miniature trust landing page.

Axis scores:

```text
Object Authority: 3
Surface Quality: 4
Mobile Nativeness: 2
Type Sexiness: 4
Accent Discipline: 4
Operational Evidence: 2
Interaction Promise: 2
Anti-Slop Resistance: 3
Desire: 3
```

## F. Ops Console

Score: 7.5 / 10

Keep:

- Dark operational surface fits the stack well.
- Metrics and bars create state.
- Serif display plus mono labels is a strong contrast.

Weak:

- Metrics are still demo-like.
- Needs a clearer task flow or selected automation state.
- Mobile affordances are weaker than A.

Next mutation:

- Turn it into an active run console: selected workflow, current task, queue, success/failure heat.

Reject if:

- It becomes a static dashboard poster.

Axis scores:

```text
Object Authority: 4
Surface Quality: 4
Mobile Nativeness: 3
Type Sexiness: 4
Accent Discipline: 4
Operational Evidence: 4
Interaction Promise: 3
Anti-Slop Resistance: 5
Desire: 4
```

## V2 Direction

The next board should focus on mutations of A, F, and C:

- A1: Wallet card stack with selected-card state
- A2: Transfer composer with amount and recipient state
- F1: Active workflow run console
- F2: Ops-finance hybrid with task heat and ledger state
- C1: Vault control with lock/verify state
- C2: Industrial wallet with spec-driven asset selection
