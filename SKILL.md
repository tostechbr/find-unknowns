---
name: find-unknowns
description: Surface your unknowns before, during, and after a task (blind spot pass, references, implementation notes, pitch/explainer, quiz). Use when starting unfamiliar work, when scope feels fuzzy, mid-implementation after hitting an edge case the plan didn't cover, or before merging/shipping a long session. For interviewing you about a plan question-by-question, use grill-me instead. For visual design brainstorm, use design-shotgun instead.
---

Core idea: the prompt is the map, the codebase/reality is the territory. The gap between them is your unknowns. Quality of output is bottlenecked by how well you surface those unknowns, not just by model capability.

## The four quadrants

Before picking a pattern, name which quadrant you're in:

- **Known known** — already in the prompt. Just say it.
- **Known unknown** — aware you haven't figured it out. Ask directly, or interview (→ `grill-me`).
- **Unknown known** — obvious once you see it, can't verbalize it upfront (taste, "I'll know it when I see it"). → brainstorm/prototype.
- **Unknown unknown** — don't even know what you don't know. → blind spot pass.

## When to use which

| Moment | Situation | Pattern | File |
|---|---|---|---|
| Pre-implementation | New/unfamiliar area of the codebase or domain | Blind spot pass | `references/blind-spot-pass.md` |
| Pre-implementation | You'd recognize "good" but can't describe it upfront | Brainstorm/prototype (visual → `design-shotgun`) | `references/brainstorm-prototype.md` |
| Pre-implementation | Ambiguity you're aware of, need it resolved one branch at a time | Interview | use `grill-me` |
| Pre-implementation | Hard to describe in words, easy to point at | References | `references/references-as-source.md` |
| During implementation | Agent may hit edge cases that force a deviation from plan | Implementation notes | `references/implementation-notes.md` |
| Post-implementation | Need buy-in / approval from reviewers | Pitch and explainer | `references/pitch-explainer.md` |
| Post-implementation | Need to actually understand what a long session changed before merging | Quiz | `references/quiz.md` |

Don't run every pattern on every task. Pick the one that matches where the unknown actually is. A five-minute fix doesn't need a blind spot pass; a new domain rarely needs a quiz.
