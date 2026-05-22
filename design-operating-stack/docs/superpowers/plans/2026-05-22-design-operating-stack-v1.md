# Design Operating Stack V1 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build the V1 document-based Design Operating Stack as an independent agent skill/rulepack with web, mobile, study, audit, generate, and systemize coverage.

**Architecture:** V1 is markdown-first. `SKILL.md` acts as the routing entrypoint, while focused reference files define genres, web patterns, mobile patterns, reference DNA, anti-slop gates, and future tool boundaries. No executable CLI or web board is implemented in V1.

**Tech Stack:** Markdown skill files, local Git repository at `D:\HB\Rhizome\sexy_design`, remote `https://github.com/JangHyun-bin/sexy_design.git`.

---

## File Structure

- Create `design-operating-stack/SKILL.md`: agent-facing router and operating rules.
- Create `design-operating-stack/README.md`: human-facing overview and usage.
- Create `design-operating-stack/references/taste-principles.md`: global taste laws.
- Create `design-operating-stack/references/reference-study.md`: reference DNA extraction flow.
- Create `design-operating-stack/references/generation-flow.md`: generation workflow.
- Create `design-operating-stack/references/audit-flow.md`: audit workflow.
- Create `design-operating-stack/references/anti-slop-gates.md`: rejection gates.
- Create six files under `design-operating-stack/genres/`: the initial taste families from `<private-reference-folder>/`.
- Create six files under `design-operating-stack/mobile-patterns/`: first-class mobile UI grammar.
- Create five files under `design-operating-stack/web-patterns/`: web/page pattern grammar.
- Create `design-operating-stack/reference-dna/dna-schema.md`: reusable extraction schema.
- Create `design-operating-stack/reference-dna/refs-image-analysis.md`: current 17-image analysis.
- Create `design-operating-stack/future-tools/cli-plan.md`: non-implemented CLI plan.
- Create `design-operating-stack/future-tools/visual-board-plan.md`: non-implemented visual board plan.
- Create root `.gitignore`: exclude nested `hallmark/` repo and local noise.

## Task 1: Initialize Root Repository Boundary

**Files:**
- Create: `.gitignore`

- [ ] **Step 1: Create root ignore rules**

Use this exact content:

```gitignore
# Existing upstream reference checkout; keep out of this repo.
hallmark/

# Local/system noise
.DS_Store
Thumbs.db
desktop.ini

# Package manager / build output
node_modules/
dist/
build/
.vercel/
.next/

# Logs
*.log
```

- [ ] **Step 2: Initialize git repo if missing**

Run: `git init`

Expected: creates `.git/` in `D:\HB\Rhizome\sexy_design`.

- [ ] **Step 3: Add remote**

Run: `git remote add origin https://github.com/JangHyun-bin/sexy_design.git`

If origin already exists, run: `git remote set-url origin https://github.com/JangHyun-bin/sexy_design.git`

- [ ] **Step 4: Verify boundary**

Run: `git status --short`

Expected: `hallmark/` does not appear as a staged or unstaged tracked path.

## Task 2: Create Skill Entrypoint

**Files:**
- Create: `design-operating-stack/SKILL.md`
- Create: `design-operating-stack/README.md`

- [ ] **Step 1: Write `SKILL.md`**

The file must define:

- skill name and description
- four modes: `study`, `audit`, `generate`, `systemize`
- routing rules
- safety rules: no pixel copying, no fake proof, no generic SaaS defaults
- file-loading discipline: load only the needed references
- mobile-first-class rule

- [ ] **Step 2: Write `README.md`**

The file must explain:

- what the stack is
- how it differs from Hallmark
- folder layout
- mode examples
- current V1 status

- [ ] **Step 3: Verify entrypoint links**

Run: `Select-String -Path .\design-operating-stack\SKILL.md -Pattern 'references/|genres/|mobile-patterns/|web-patterns/|reference-dna/'`

Expected: every folder category is referenced at least once.

## Task 3: Create Core Reference Flows

**Files:**
- Create: `design-operating-stack/references/taste-principles.md`
- Create: `design-operating-stack/references/reference-study.md`
- Create: `design-operating-stack/references/generation-flow.md`
- Create: `design-operating-stack/references/audit-flow.md`
- Create: `design-operating-stack/references/anti-slop-gates.md`

- [ ] **Step 1: Write taste principles**

Include the seven principles from the spec:

- Object First
- One Dominant Gesture
- Accent Footprint Discipline
- Material Surface
- Type As Product
- Operational Sexiness
- Mobile Is Not A Shrunk Website

- [ ] **Step 2: Write reference study flow**

Include required output fields:

- source summary
- genre classification
- surface system
- type roles
- dominant gesture
- mobile grammar
- reusable components
- anti-patterns
- candidate build rules

- [ ] **Step 3: Write generation flow**

Include the sequence:

1. choose surface family
2. choose genre
3. choose dominant gesture
4. choose type role
5. choose accent footprint
6. choose web or mobile pattern
7. choose interaction stance
8. run anti-slop gates

- [ ] **Step 4: Write audit flow**

Include scoring axes:

- object presence
- type authority
- surface specificity
- operational evidence
- mobile native grammar
- interaction states
- accent discipline
- proof honesty

- [ ] **Step 5: Write anti-slop gates**

Include explicit failures for:

- generic centered SaaS hero
- purple-blue decorative blobs
- filler rounded cards
- fake browser chrome
- fake metrics/testimonials/logos
- hover-scale-only interactions
- mobile as stacked desktop
- charts without encoded meaning
- controls without states

## Task 4: Create Taste Genre Files

**Files:**
- Create: `design-operating-stack/genres/dark-technical-editorial.md`
- Create: `design-operating-stack/genres/warm-institutional-serif.md`
- Create: `design-operating-stack/genres/atmospheric-product-cinema.md`
- Create: `design-operating-stack/genres/academic-handdrawn-editorial.md`
- Create: `design-operating-stack/genres/industrial-swiss-object.md`
- Create: `design-operating-stack/genres/mobile-kinetic-finance.md`

- [ ] **Step 1: Write one genre file per family**

Each file must include:

- source signal
- when to use
- surface
- typography
- dominant gesture
- interaction stance
- good components
- avoid list

- [ ] **Step 2: Verify six genre files exist**

Run: `Get-ChildItem .\design-operating-stack\genres -File | Measure-Object`

Expected: `Count : 6`.

## Task 5: Create Mobile Pattern Files

**Files:**
- Create: `design-operating-stack/mobile-patterns/oversized-number-screen.md`
- Create: `design-operating-stack/mobile-patterns/tactile-control-surface.md`
- Create: `design-operating-stack/mobile-patterns/card-stack-wallet.md`
- Create: `design-operating-stack/mobile-patterns/alarm-time-picker.md`
- Create: `design-operating-stack/mobile-patterns/transaction-dashboard.md`
- Create: `design-operating-stack/mobile-patterns/bottom-action-system.md`

- [ ] **Step 1: Write one mobile pattern file per pattern**

Each file must include:

- use when
- anatomy
- layout rules
- state rules
- motion rules
- accessibility constraints
- anti-slop checks

- [ ] **Step 2: Verify first-class mobile coverage**

Run: `Select-String -Path .\design-operating-stack\mobile-patterns\*.md -Pattern 'state|motion|thumb|bottom|pressed|disabled|loading|success'`

Expected: matches across multiple files.

## Task 6: Create Web Pattern Files

**Files:**
- Create: `design-operating-stack/web-patterns/object-first-hero.md`
- Create: `design-operating-stack/web-patterns/giant-wordmark-hero.md`
- Create: `design-operating-stack/web-patterns/cinematic-product-fold.md`
- Create: `design-operating-stack/web-patterns/editorial-logo-wall.md`
- Create: `design-operating-stack/web-patterns/operational-dashboard-surface.md`

- [ ] **Step 1: Write one web pattern file per pattern**

Each file must include:

- use when
- anatomy
- layout rules
- typography rules
- surface rules
- responsive behavior
- anti-slop checks

- [ ] **Step 2: Verify web coverage**

Run: `Get-ChildItem .\design-operating-stack\web-patterns -File | Measure-Object`

Expected: `Count : 5`.

## Task 7: Create Reference DNA Files

**Files:**
- Create: `design-operating-stack/reference-dna/dna-schema.md`
- Create: `design-operating-stack/reference-dna/refs-image-analysis.md`

- [ ] **Step 1: Write DNA schema**

Include fields:

- source
- source type
- genre
- paper band
- accent footprint
- type roles
- dominant gesture
- surface treatment
- object type
- web pattern
- mobile pattern
- interaction stance
- anti-patterns
- transferable rules

- [ ] **Step 2: Write current reference analysis**

Document the 17 screenshots as six clusters:

- Dark Technical Editorial
- Warm Institutional Serif
- Atmospheric Product Cinema
- Academic Hand-Drawn Editorial
- Industrial Swiss Object
- Mobile Kinetic Finance

- [ ] **Step 3: Verify all clusters are represented**

Run: `Select-String -Path .\design-operating-stack\reference-dna\refs-image-analysis.md -Pattern 'Dark Technical|Warm Institutional|Atmospheric Product|Academic Hand|Industrial Swiss|Mobile Kinetic'`

Expected: six matches or more.

## Task 8: Create Future Tool Plans

**Files:**
- Create: `design-operating-stack/future-tools/cli-plan.md`
- Create: `design-operating-stack/future-tools/visual-board-plan.md`

- [ ] **Step 1: Write CLI plan**

Document future commands only:

- `dos study <private-reference-folder>/`
- `dos audit <url-or-path>`
- `dos generate --mode mobile --genre industrial-swiss-object`
- `dos board <private-reference-folder>/`

State clearly that CLI is not implemented in V1.

- [ ] **Step 2: Write visual board plan**

Document future board panels:

- thumbnails
- detected genre
- color footprint
- dominant gesture
- extracted patterns
- accepted rules
- rejected slop patterns

State clearly that visual board is not implemented in V1.

## Task 9: Verify, Commit, Push

**Files:**
- All created V1 files

- [ ] **Step 1: Verify markdown file count**

Run: `Get-ChildItem .\design-operating-stack -Recurse -File -Filter *.md | Measure-Object`

Expected: at least 29 markdown files.

- [ ] **Step 2: Verify ignored nested repo**

Run: `git status --short --ignored`

Expected: `hallmark/` appears ignored or absent from normal status.

- [ ] **Step 3: Commit**

Run:

```powershell
git add .gitignore private reference folder design-operating-stack
git commit -m "feat: add design operating stack v1"
```

Expected: commit succeeds.

- [ ] **Step 4: Push**

Run: `git push -u origin main`

If the local branch is `master`, run:

```powershell
git branch -M main
git push -u origin main
```

Expected: branch `main` is pushed to `https://github.com/JangHyun-bin/sexy_design.git`.

## Self-Review

- Spec coverage: all V1 deliverables from the design spec are mapped to tasks.
- Placeholder scan: no task uses `TBD`, `TODO`, or unspecified implementation language.
- Type consistency: folder names match the design spec.
- Execution decision: user asked to push and start, and subagents were not explicitly requested, so execution should proceed inline.

