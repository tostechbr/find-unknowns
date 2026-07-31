# Brainstorm and prototype

Use when you're in unknown-known territory: you'd recognize the right answer if you saw it, but can't specify it upfront. Finding this out mid-implementation is expensive — small spec changes can force drastically different code, and reverting is harder than it looks.

For visual design brainstorm specifically, use `design-shotgun` instead (it already generates variants + a comparison board). Use this pattern for non-visual scope/approach brainstorming.

**Example prompts:**

- "Before wiring anything up, make a single HTML file mocking [feature] with fake data. I want to react to the shape before you touch the real app."
- "Here's my rough problem: [X]. Search the codebase and brainstorm N places we could intervene, cheapest to most ambitious. I'll tell you which ones resonate."

Start sessions with an explicit brainstorm/exploration phase before committing to scope — it catches both "too narrow" and "too wide" before either costs implementation time.
