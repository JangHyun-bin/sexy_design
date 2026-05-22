# Reference DNA Schema

Use this schema for `study` and `systemize` outputs.

## Schema

```text
source:
source_type:
source_owner:
study_date:
genre:
genre_confidence:
paper_band:
paper_hue:
accent_hue:
accent_footprint:
type_display_role:
type_body_role:
type_label_role:
dominant_gesture:
object_type:
surface_treatment:
web_pattern:
mobile_pattern:
interaction_stance:
density:
asymmetry:
reusable_components:
anti_patterns:
transferable_rules:
do_not_copy:
```

## Field Guidance

`source`
: File path, URL, screenshot group, or user description.

`source_type`
: `image`, `url`, `folder`, `mixed`, or `description`.

`source_owner`
: `user-owned`, `public-reference`, `unknown`, or `restricted`.

`genre`
: Closest genre from `genres/`, or `new-candidate` only in `systemize` mode.

`accent_footprint`
: `pin`, `signal`, `field`, or `flood`.

`dominant_gesture`
: The one visual move that carries the first impression.

`object_type`
: Product, phone, dashboard, card, chart, number, wordmark, illustration, or
other dominant object.

`surface_treatment`
: Grain, halftone, blur, paper, industrial gray, dot matrix, chart grid, or none.

`interaction_stance`
: Still, slow cinematic reveal, tactile pressed controls, scroll-synced object,
stateful dashboard, or kinetic number/time.

`do_not_copy`
: Any signature artwork, exact layout, exact image, or brand-specific mark that
must remain reference-only.

## Minimum Useful Study

A study is not useful unless it names:

- genre
- dominant gesture
- object type
- accent footprint
- at least one transferable rule
- at least one do-not-copy constraint
