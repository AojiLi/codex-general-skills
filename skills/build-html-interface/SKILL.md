---
name: build-html-interface
description: "Create fast, desktop-first, Apple-style HTML visual explainers from user-provided concepts, formulas, documents, or software repositories. Use when the user wants a polished standalone HTML explanation, interactive teaching page, architecture walkthrough, codebase map, process or data-flow visualization, or explicitly invokes build-html-interface. Default to one self-contained index.html, strong Apple-inspired typography and composition, focused diagrams, restrained interaction, and one quick desktop browser check. Do not default to mobile verification, full web-app states, multi-agent work, broad research, or gesture-physics engineering."
---

# Apple-Style HTML Explainer

## Objective

Turn information into a visually compelling explanation that feels like a polished Apple product story: clear hierarchy, generous space, precise typography, quiet materials, crisp diagrams, and restrained motion.

Optimize for explanation quality and execution speed. This is not a general web-app builder. Default to the user's language and a desktop presentation around `1440x900`.

## Default Deliverable

- Create one self-contained `index.html` with embedded CSS and JavaScript.
- Open with the actual topic, question, system, or repository story, not a generic marketing page.
- Build one primary explanatory visual and at most one supporting visual system.
- Add interaction only when it improves understanding: reveal, compare, filter, step through, inspect, or adjust a meaningful variable.
- Include a basic narrow-width CSS fallback when inexpensive, but do not design for or verify mobile unless the user explicitly asks.

## Apple Visual Language

Treat Apple style as a mandatory visual direction, not a vague reference.

- Use the system font stack so Apple platforms resolve to San Francisco. Use confident weight, clear scale, comfortable leading, and `letter-spacing: 0`.
- Build on a neutral white, soft gray, or near-black foundation with one or two functional accent colors. Use accent colors to map meaning consistently across diagrams, labels, and formulas.
- Prefer a few large compositional planes, broad whitespace, hairline separators, exact alignment, and quiet hierarchy over dense card grids.
- Use translucent material only for genuinely floating or sticky chrome. Keep content surfaces mostly solid and readable.
- Use subtle, diffuse shadows and restrained borders. Avoid loud glow, decorative gradients, bokeh, floating orbs, and generic glass cards.
- Keep corner radii and spacing systematic. Do not mix unrelated shape languages.
- Use large editorial headings only for the page's main thesis. Keep panel and diagram labels compact.
- Make the central diagram or visualization crisp and inspectable. It must encode real relationships, quantities, sequence, or hierarchy.
- Use short opacity, transform, or reveal transitions to guide attention. Avoid bounce, excessive parallax, perpetual motion, and gesture physics unless the user explicitly requests them.
- Respect `prefers-reduced-motion` with a simple fallback, but do not run a separate reduced-motion test by default.
- Do not copy Apple logos, product names, screenshots, or exact page layouts. Recreate the visual discipline, not the brand assets.

## Explanation Model

Build one coherent narrative:

1. Thesis: state the question and shortest correct answer.
2. Model: show the entities and relationships visually.
3. Breakdown: walk through the mechanism, formula, flow, or architecture.
4. Evidence: include one concrete example, trace, calculation, or repository path.
5. Takeaway: show what to remember, what is excluded, or where to inspect next.

Do not fill the page with repeated feature cards or generic prose. Every section must advance the explanation.

## Workflow

### 1. Read The Source Quickly

For a concept, formula, document, or pasted explanation, extract:

- the exact question
- the shortest correct conclusion
- important entities and relationships
- sequence, hierarchy, or causal flow
- one worked example
- likely misunderstanding or boundary case

For a repository-based explanation, read [references/repo-explainer.md](references/repo-explainer.md) and inspect only enough files to support an accurate visual story.

Do not perform web research, image search, or multi-agent analysis unless the user asks or the explanation depends on external facts not present in the source.

### 2. Choose One Visual Story

Select the clearest primary pattern:

- equation decomposition for formulas and parameter counts
- node-link or layered diagram for architectures and dependencies
- sequence or swimlane for request lifecycles
- pipeline for data and build flows
- timeline for historical or ordered processes
- before/after comparison for transformations
- small simulator for variables with meaningful effects

Use no more than one primary pattern and one supporting pattern. Keep the main diagram to a readable number of labeled elements; group secondary detail instead of shrinking everything.

Silently form the design direction and proceed. Do not make the user approve a design plan unless the visual interpretation is genuinely ambiguous.

### 3. Build The Page

- Use semantic HTML and real content from the request or repository.
- Prefer CSS and inline SVG for diagrams, formulas, connectors, callouts, and architecture maps. Use canvas only when the visual is genuinely dynamic or dense.
- Use actual repository file paths, module names, data shapes, and functions when explaining code. Do not invent components for visual neatness.
- Keep formulas visually linked to the corresponding diagram colors and labels.
- Use progressive JavaScript without a framework for standalone explainers.
- Do not add a build system, external UI framework, animation library, or CDN dependency unless the task clearly benefits from it.
- Do not implement loading, empty, error, authentication, persistence, or other app states unless they are part of the explanation.
- Keep every visible control functional and keyboard reachable, but do not run a full accessibility audit by default.

### 4. Run Fast Desktop Verification

Perform one quick browser pass when browser tooling is available:

1. Render at approximately `1440x900`.
2. Capture one screenshot and inspect the actual composition.
3. Check the browser console.
4. Exercise the single primary interaction, if one exists.
5. Check for overlap, clipping, accidental horizontal overflow, unreadable text, blank diagrams, broken assets, and factual or formula mismatches.

If a defect appears, fix it and repeat only the affected check. Do not run mobile, tablet, orientation, 200% zoom, full keyboard traversal, multiple browser sessions, full-page screenshot suites, or exhaustive state testing unless the user explicitly asks.

If a temporary local server is needed only for browser tooling, stop it after verification. A standalone file should remain directly openable.

### 5. Hand Off

Return:

- a clickable path to `index.html`
- one sentence describing the visual story
- the desktop viewport and primary interaction checked
- any real limitation

Keep the response brief. Do not paste the full HTML or narrate the design process unless requested.

## Speed Guardrails

- Do not spawn subagents.
- Do not generate multiple visual concepts unless asked.
- Do not browse for inspiration by default.
- Do not add decorative assets when a precise diagram communicates better.
- Do not over-engineer animation or interaction.
- Do not perform mobile verification unless explicitly requested.
- Stop after the first clean desktop check.
