# find-unknowns

A Claude Code skill for surfacing what you don't know before, during, and after a task: blind spot pass, brainstorm/prototype, references, implementation notes, pitch/explainer, quiz.

Based on Anthropic's [A field guide to Claude Fable 5: finding your unknowns](https://claude.com/blog/a-field-guide-to-claude-fable-finding-your-unknowns) by Thariq Shihipar, and applying [The new rules of context engineering for Claude 5 generation models](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) to how the skill itself is structured (thin `SKILL.md`, one small file per pattern, loaded only when needed).

## Install

Copy into your global or project skills folder:

```bash
cp -r find-unknowns ~/.claude/skills/
```

## What's inside

- `SKILL.md` — the four-quadrants framework (known/unknown knowns, known/unknown unknowns) and a decision table for which pattern to use when.
- `references/` — one file per pattern, each with ready-to-use example prompts:
  - `blind-spot-pass.md`
  - `brainstorm-prototype.md`
  - `references-as-source.md`
  - `implementation-notes.md`
  - `pitch-explainer.md`
  - `quiz.md`

Two patterns from the article aren't duplicated here on purpose: interviewing you question-by-question about a plan, and brainstorming visual design variants. Both are common enough that you likely already have a skill for them; `SKILL.md` just points at where those would slot in.
