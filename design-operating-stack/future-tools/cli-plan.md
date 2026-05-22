# Future CLI Plan

Status: planned, not implemented in V1.

The CLI should be a convenience layer over the markdown rulepack. It must not
become a second source of truth.

## Candidate Name

`dos`

## Commands

```powershell
dos study <private-reference-folder>/
dos audit <url-or-path>
dos generate --mode mobile --genre industrial-swiss-object
dos board <private-reference-folder>/
```

## Command Responsibilities

### `dos study`

- Reads local screenshots or URLs.
- Produces DNA using `reference-dna/dna-schema.md`.
- Suggests whether the result maps to an existing genre or a new candidate.

### `dos audit`

- Reads a local path, screenshot, or URL.
- Runs `references/audit-flow.md`.
- Outputs ranked findings and score axes.

### `dos generate`

- Loads the requested genre and pattern files.
- Produces a design brief or scaffold.
- Runs anti-slop gates before writing code.

### `dos board`

- Opens or generates a visual board from references.
- Uses the same DNA fields as `study`.

## Non-Goals

- No CLI in V1.
- No duplicate rules in code.
- No remote fetching beyond explicit user input.
- No automatic copying from reference sites.

## Implementation Notes For Later

- Prefer a small Node or Python CLI only after the markdown workflow proves
  useful.
- Keep outputs human-readable.
- Store generated analysis as markdown unless a real need for JSON appears.
