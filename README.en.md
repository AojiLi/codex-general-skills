# Codex General Skills

Language: English | [中文](./README.zh-CN.md)

Reusable Codex skills for idea validation, decision-making, voice-preserving editing, distinctive frontend design, Apple-style HTML explainers, and algorithmic art.

This repository contains general-purpose creative and productivity workflows. Engineering-specific project setup, repository review, and primary-source research remain in [AojiLi/codex-skills](https://github.com/AojiLi/codex-skills).

## Skills

### [idea-validator](./skills/idea-validator/SKILL.md)

Use it before implementation when an idea, product concept, research direction, project plan, or architecture thought is still incomplete. It clarifies the problem, user, solution, timing, success criteria, constraints, and unknowns one question at a time. After you confirm the brief, it asks whether to use five independent research subagents or run the same lanes sequentially, synthesizes the evidence, automatically runs up to five skeptic rounds, and returns feasibility, value, differentiation, MVP, implementation, validation, risk, and next-step conclusions.

```text
Use $idea-validator to evaluate this idea before I build it: [describe the idea].
```

### [decision-advisor](./skills/decision-advisor/SKILL.md)

Use it for a meaningful choice, tradeoff, option comparison, or whether-to-do-something question. It clarifies the background, purpose, decision question, candidate options, jurisdiction, constraints, and decision weights before analysis. After you confirm that frame, it asks whether to use six independent lens subagents or a sequential single-agent mode, then analyzes economics, strategy, psychology, risk, legal/regulatory issues, and technical feasibility with critique-revision loops. The result includes a recommendation, alternatives, action plan, confidence, and review signals.

```text
Use $decision-advisor to help me decide whether to take this job offer or keep building my company.
```

### [voice-preserving-editor](./skills/voice-preserving-editor/SKILL.md)

Use it to polish pasted prose, Markdown, README files, DOCX documents, or Google Docs without turning the writing into generic AI prose. It reads the surrounding context, chooses light, medium, or explicitly requested heavy editing, changes only the requested passage, preserves viewpoint, tone, rhythm, vocabulary, and emotional intensity, and flags uncertain facts rather than inventing corrections.

```text
Use $voice-preserving-editor to polish this README section without changing my tone: [paste text].
```

### [frontend-design](./skills/frontend-design/SKILL.md)

Use it when building a new interface or redesigning an existing one that needs a distinctive visual identity. It grounds the design in the real subject and audience, develops a compact color/type/layout/signature system, compares layout ideas, critiques generic choices before implementation, then builds and visually reviews the result with responsive, accessible interaction details.

```text
Use $frontend-design to redesign this dashboard around the product's actual workflow and existing codebase.
```

### [apple-html-explainer](./skills/apple-html-explainer/SKILL.md)

Use it to turn concepts, formulas, documents, or software repositories into desktop-first Apple-style visual explanations. It creates one self-contained `index.html` with precise system typography, spacious composition, quiet materials, diagrams, and restrained interaction. Repository tasks map real modules, files, or data flows. It performs one fast desktop browser check and does not default to mobile verification, full app states, broad research, or heavy animation engineering.

```text
Use $apple-html-explainer to explain this neural-network formula as a polished Apple-style visual HTML page.
```

### [algorithmic-art](./skills/algorithmic-art/SKILL.md)

Use it to create original generative or computational art with p5.js. It first writes a concise algorithmic philosophy, extracts a subtle conceptual seed from the request, then builds a seeded and reproducible algorithm in the bundled interactive viewer template. The output is a self-contained HTML artifact with working parameters, seed navigation, reset/regenerate controls, and PNG download.

```text
Use $algorithmic-art to create an interactive generative artwork inspired by orbital resonance and tidal motion.
```

## Install

Install all skills:

```bash
npx skills@latest add AojiLi/codex-general-skills
```

Install one skill:

```bash
npx skills@latest add AojiLi/codex-general-skills --skill idea-validator
npx skills@latest add AojiLi/codex-general-skills --skill decision-advisor
npx skills@latest add AojiLi/codex-general-skills --skill voice-preserving-editor
npx skills@latest add AojiLi/codex-general-skills --skill frontend-design
npx skills@latest add AojiLi/codex-general-skills --skill apple-html-explainer
npx skills@latest add AojiLi/codex-general-skills --skill algorithmic-art
```

## Structure

```text
codex-general-skills/
|-- README.md
|-- README.en.md
|-- README.zh-CN.md
`-- skills/
    |-- idea-validator/
    |-- decision-advisor/
    |-- voice-preserving-editor/
    |-- frontend-design/
    |-- apple-html-explainer/
    `-- algorithmic-art/
```

Each skill keeps its own instructions, metadata, bundled resources, and license files where applicable.

## Licenses

`frontend-design` and `algorithmic-art` retain their bundled `LICENSE.txt` files. Other repository content has no separate repository-wide license unless one is added explicitly.
