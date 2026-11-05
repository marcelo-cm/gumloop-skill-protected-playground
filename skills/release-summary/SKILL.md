---
name: release-summary
description: Turn a short list of product changes into a clear release summary with checks and open questions.
---

# Release summary

Use this skill when User A asks for a release summary from a list of changes.

1. Read the supplied changes. If none are supplied, use
   `references/sample-changes.md` and state that the input is synthetic.
2. Group related changes. Explain the effect on the user in plain words.
3. Use `templates/summary.md` for the output shape.
4. Separate confirmed checks from checks that still need to run.
5. List missing facts as open questions. Do not invent results or dates.

Keep the summary concise. Do not publish it or contact anyone unless User A
asks for that action.
