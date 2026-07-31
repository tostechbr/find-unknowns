# Quiz

Use post-implementation, before merging a long session. Reading the diff only gives a light understanding of what happened — a lot of the actual behavior depends on existing code paths you didn't touch but that now interact differently.

Have Claude quiz you on the change after briefing you on context. Only merge after passing the quiz.

**Example prompt:**

- "I want to make sure I understand everything that happened in this change. Give me a report with context, intuition, and what was done, then a quiz at the bottom I must pass before I merge."

If you can't pass your own quiz, that's a signal you don't understand the change well enough to be the one approving it — go back and ask, don't just merge anyway.
