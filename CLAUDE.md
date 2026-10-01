# Working with Diana

Behavioral guidelines for this project. Follow them exactly.

---

## 1. Think Before Designing

Don't assume. Surface tradeoffs. Ask when confused.

Before generating or editing anything:
- If it's unclear which design system or component set applies, ask rather than guessing.
- If multiple reasonable directions exist (e.g., layout approaches, component patterns), present them, don't pick silently.
- If a simpler version would get the point across, say so before building something more elaborate.
- If something about the request is genuinely ambiguous, name what's confusing rather than quietly interpreting it one way.

Project-specific things to confirm before generating UI:
- Which design system should this reference? There are currently three in use; only the newest is documented in Storybook. If unsure which applies, ask.
- Is this meant to match the existing product closely, or is it an early, rough exploration? These call for different levels of polish.
- If writing to Figma, confirm the target file first. Known file: "TOFU explorations" (key: 4uG2kcXG8PpJELeL7NrfSe).

## 2. Simplicity First

Minimum needed to make the point. Nothing speculative.

- No extra states, settings, or polish beyond what was asked for.
- No building out a "full app" when a single screen or flow was requested.
- If a plain HTML mockup would answer the question, don't reach for a heavier framework.
- If something ends up more complex than it needs to be, simplify it before calling it done.

## 3. Surgical Changes

Touch only what's asked. Don't "fix" things along the way.

When editing an existing file or Figma frame:
- Don't restyle or reorganize elements that weren't part of the request.
- Match whatever structure/style already exists in the file, even if a different approach would be preferred.
- If something unrelated looks broken or outdated, mention it, don't change it unprompted.

## 4. Goal-Driven Execution

Define what "done" looks like before starting. Confirm it before declaring the task finished.

Turn vague asks into checkable outcomes:
- "Mock up this flow" → "Screens exist for each step, navigation between them makes sense, visual style is reasonably close to the brand"
- "Capture this component in Figma" → "Component appears in the target file, structure/spacing roughly matches the live version, layer names are sensible"
- "Build a quick prototype" → "Opens correctly, core interaction works, no placeholder content left unlabeled"

For anything multi-step, state a brief plan before starting:
1. [Step] → check: [what confirms it worked]
2. [Step] → check: [what confirms it worked]
Done when: [final state]

## Figma-specific conventions

- When creating or editing **sections** in Figma, use `#404040` (RGB 0.251, 0.251, 0.251) as the section background fill color.
- Use the `figma-generate-library` or `figma-create-new-file` skills when the goal is capturing existing code components into Figma.
- Use `figma-generate-design` when the goal is producing new design exploration directly in Figma.
- Use `figma-design-to-code` only when going the other direction (Figma → code).

## Writing conventions

- No em dashes in any generated copy, docs, or messages.
- Plain, direct language over jargon. Spell out acronyms on first use.
- Skip step-by-step narration of what's being done (e.g. "first I'll check X, then I'll update Y"). A brief framing sentence is fine, just get to the result without narrating the process.
