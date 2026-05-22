# Future Visual Board Plan

Status: planned, not implemented in V1.

The visual board is a future companion for reference study and taste systemization.
The markdown rulepack must work without it.

## Purpose

Help compare reference images, extracted DNA, accepted rules, rejected slop
patterns, and genre evolution.

## Panels

- thumbnails
- detected genre
- color footprint
- dominant gesture
- object type
- surface treatment
- web pattern
- mobile pattern
- accepted rules
- rejected slop patterns
- do-not-copy notes

## Board Flow

1. Import a local folder such as `<private-reference-folder>/`.
2. Show image thumbnails.
3. Group references by detected genre.
4. Let the user accept, reject, or revise extracted DNA.
5. Export markdown updates for `reference-dna/`, `genres/`, or pattern files.

## Constraints

- The board must not make design decisions silently.
- It must keep reference images as references, not assets to copy.
- It must identify when a reference is a one-off exception.
- It must preserve the markdown rulepack as source of truth.

## Possible Implementation

- Static local HTML first.
- Later, a small app if editing and export become useful.
- No server dependency unless image ingestion needs it.
