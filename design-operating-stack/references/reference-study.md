# Reference Study Flow

Use this when the user gives screenshots, URLs, local images, or a folder of
references.

The goal is to extract DNA, not copy pixels.

## Inputs

Accepted:

- local image folder
- attached screenshots
- public URL
- mixed web and mobile captures
- user-described references

Ask before studying if the source looks like:

- paid template marketplace
- private dashboard
- auth-walled product
- a designer's signature work being treated as a template

## Study Order

1. Source summary
2. Genre classification
3. Surface system
4. Type roles
5. Dominant gesture
6. Object model
7. Mobile grammar if present
8. Web pattern if present
9. Interaction stance
10. Anti-patterns to avoid
11. Transferable build rules

## Required Output

Return a compact diagnosis with these fields:

```text
Source:
Closest genre:
Surface:
Type roles:
Dominant gesture:
Object:
Accent footprint:
Web pattern:
Mobile pattern:
Interaction stance:
Reusable components:
Anti-patterns:
Transferable rules:
```

## Genre Classification

Start with the six existing families:

- Dark Technical Editorial
- Warm Institutional Serif
- Atmospheric Product Cinema
- Academic Hand-Drawn Editorial
- Industrial Swiss Object
- Mobile Kinetic Finance

If the reference does not fit, name the nearest family and describe the delta.
Only create a new genre in `systemize` mode.

## Study Rules

- Do not name exact typefaces from screenshots unless the source provides them.
- Describe roles instead: editorial serif, giant grotesque, mono annotation,
  oversized numeric.
- Treat screenshots as evidence of rhythm, density, hierarchy, and surface.
- Treat URLs as useful for exact CSS values, but weaker for visual rhythm unless
  the rendered page is visible.
- If a reference contains copyrighted artwork, extract layout and surface logic
  only. Do not reproduce the artwork.

## Transfer Rule

A good study output should let a different product use the same structural DNA
without looking like a clone.
