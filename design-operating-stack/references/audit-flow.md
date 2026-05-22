# Audit Flow

Use this when evaluating an existing UI.

Lead with findings. Do not bury risks under praise.

## Audit Axes

Score each axis from 1 to 5.

| Axis | 1 | 5 |
| --- | --- | --- |
| Object presence | No dominant object | Clear object carries the screen |
| Type authority | Generic hierarchy | Type has product-level presence |
| Surface specificity | Flat or decorative | Surface supports concept |
| Operational evidence | Claims only | State, data, controls, or specs visible |
| Mobile native grammar | Stacked desktop | Phone-native state and controls |
| Interaction states | Static | States are designed and legible |
| Accent discipline | Many casual accents | One controlled footprint |
| Proof honesty | Fake or vague proof | Real, labeled, or omitted proof |

## Findings Format

```text
Findings
1. [Severity] Issue - file/screen/area
   Why it fails:
   Repair direction:
   Relevant principle:

Scores
Object presence:
Type authority:
Surface specificity:
Operational evidence:
Mobile native grammar:
Interaction states:
Accent discipline:
Proof honesty:

Best-fit direction:
Next repair:
```

## Severity

- Critical: makes the UI generic, dishonest, unusable, or off-taste.
- High: weakens first impression or mobile usability.
- Medium: undermines craft but does not break the concept.
- Low: polish issue.

## Repair Direction

Name one concrete repair:

- switch to object-first hero
- replace filler cards with spec sheet
- convert mobile screen to oversized number pattern
- reduce accents to signal footprint
- remove fake proof
- add pressed/loading/success states
- replace decorative blob with material surface

## Audit Rules

- Do not edit unless asked.
- Do not invent missing context.
- If proof is missing, recommend placeholders or removal, not fabricated content.
- If mobile is absent, state the residual risk.
