# Codex General Skills

Language: English | [中文](./README.zh-CN.md)

Reusable Codex skills for decision-making, voice-preserving editing, distinctive frontend design, and algorithmic art.

This repository contains general-purpose creative and productivity workflows. Engineering-specific project setup, repository review, research, and idea-validation skills remain in [AojiLi/codex-skills](https://github.com/AojiLi/codex-skills).

## Skills

- **[decision-advisor](./skills/decision-advisor/SKILL.md)** - Clarify a decision, confirm options and constraints, run research-backed analysis, critique the result, and return a clear recommendation and action plan.
- **[voice-preserving-editor](./skills/voice-preserving-editor/SKILL.md)** - Improve prose while preserving the author's meaning, tone, rhythm, warmth, and recognizable voice.
- **[frontend-design](./skills/frontend-design/SKILL.md)** - Develop distinctive, subject-specific visual direction, typography, layout, motion, and interface copy instead of generic template styling.
- **[algorithmic-art](./skills/algorithmic-art/SKILL.md)** - Create original p5.js generative art through algorithmic philosophies, seeded randomness, interactive parameters, and reusable viewer templates.

## Install

Install all skills:

```bash
npx skills@latest add AojiLi/codex-general-skills
```

Install one skill:

```bash
npx skills@latest add AojiLi/codex-general-skills --skill decision-advisor
npx skills@latest add AojiLi/codex-general-skills --skill voice-preserving-editor
npx skills@latest add AojiLi/codex-general-skills --skill frontend-design
npx skills@latest add AojiLi/codex-general-skills --skill algorithmic-art
```

## Structure

```text
codex-general-skills/
|-- README.md
|-- README.en.md
|-- README.zh-CN.md
`-- skills/
    |-- decision-advisor/
    |-- voice-preserving-editor/
    |-- frontend-design/
    `-- algorithmic-art/
```

Each skill keeps its own instructions, metadata, bundled resources, and license files where applicable.

## Licenses

`frontend-design` and `algorithmic-art` retain their bundled `LICENSE.txt` files. Other repository content has no separate repository-wide license unless one is added explicitly.
