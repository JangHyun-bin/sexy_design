# Taste Rubric

Use this rubric to score generated variants, audits, and reference studies.

The goal is not to make taste mechanical. The goal is to make iteration honest:
when a design feels weak, the stack should name why and suggest the next mutation.

## Scale

Each axis is scored from 1 to 5.

- 1: absent or actively harmful
- 2: present but generic
- 3: workable but not memorable
- 4: strong and directionally useful
- 5: defining strength of the screen

The weighted score is out of 10.

## Axes

| Axis | Weight | What It Measures |
| --- | ---: | --- |
| Object Authority | 1.4 | Does a number, object, wordmark, chart, card, or control own the screen? |
| Surface Quality | 1.1 | Does the background/material system have a reason beyond decoration? |
| Mobile Nativeness | 1.4 | Does the screen feel designed for touch, state, safe areas, and thumb reach? |
| Type Sexiness | 1.1 | Does type behave like product material, not placeholder hierarchy? |
| Accent Discipline | 0.9 | Is accent color assigned a clear footprint and job? |
| Operational Evidence | 1.1 | Does the screen show state, data, work, time, money, tasks, specs, or control? |
| Interaction Promise | 1.0 | Can the viewer infer how the screen moves, presses, snaps, or transitions? |
| Anti-Slop Resistance | 1.0 | Does it avoid common AI/SaaS defaults and fake polish? |
| Desire | 1.0 | Does it create pull: wanting to tap, inspect, hold, or continue? |

Total weight: 10.0.

## Formula

```text
weighted_score =
  sum(axis_score / 5 * axis_weight) / 10 * 10
```

In practice:

```text
score_out_of_10 = sum(axis_score * axis_weight) / 5
```

## Score Bands

- 8.5 to 10.0: keep and deepen
- 7.2 to 8.4: promising, mutate
- 6.0 to 7.1: useful ingredient, not a direction yet
- 4.0 to 5.9: diagnose and salvage one idea
- below 4.0: reject

## Required Scoring Output

Every scored variant should include:

```text
Variant:
Score:
Keep:
Weak:
Next mutation:
Reject if:
Axis scores:
```

## Mutation Rules

When a variant scores below 7.2:

- keep only one strong element
- change either surface, object, or interaction stance
- do not only change palette

When a variant scores 7.2 to 8.4:

- preserve the dominant gesture
- deepen the tactile states
- remove generic UI rows
- make the accent role more explicit

When a variant scores above 8.5:

- build a screen sequence
- add transition states
- test at 390 px and 500 px
- consider making it a reusable pattern

## Red Flags During Scoring

- A design gets high visual score but no interaction promise.
- A mobile screen looks good only because it is inside a phone crop.
- A chart or stat exists but has no encoded meaning.
- A large type treatment can be swapped into another variant without changing the design.
- A variant relies on the source reference too directly.
