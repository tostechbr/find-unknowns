# Implementation notes

Use during implementation, after a plan exists. No matter how much you planned, unknown unknowns surface mid-work — an edge case forces a deviation from the plan.

Have Claude keep a temporary `implementation-notes.md` (or `.html`) logging those deviations as they happen, so the next attempt (or the next reviewer) learns from them instead of rediscovering them.

**Example prompt:**

- "Keep an implementation-notes.md file. If you hit an edge case that forces you to deviate from the plan, pick the conservative option, log it under 'Deviations', and keep going."

The file is temporary scaffolding for the session, not documentation to ship — delete it once the change is understood and merged, unless it's worth folding into a real doc.
