<a id="english"></a>

# Codex General Skills

Language: English | [中文](#user-content-zh-cn)

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

<a id="zh-cn"></a>

# Codex General Skills

语言版本：[English](#user-content-english) | 中文

这是一组用于决策、保留个人声音的文字编辑、前端设计和算法艺术的通用 Codex skills。

这个仓库只保存通用创作与生产力工作流。工程专用的项目设置、仓库审核、调研和 idea validation skills 继续保留在 [AojiLi/codex-skills](https://github.com/AojiLi/codex-skills)。

## Skills

- **[decision-advisor](./skills/decision-advisor/SKILL.md)** - 澄清决策背景、选项和约束，通过有来源的多视角分析与 critique，给出明确推荐和行动计划。
- **[voice-preserving-editor](./skills/voice-preserving-editor/SKILL.md)** - 在保留作者原意、语气、节奏、温度和个人声音的前提下修改文字。
- **[frontend-design](./skills/frontend-design/SKILL.md)** - 建立与具体主题匹配的视觉方向、字体、布局、动效和界面文案，避免通用模板风格。
- **[algorithmic-art](./skills/algorithmic-art/SKILL.md)** - 通过 algorithmic philosophy、seeded randomness、交互参数和 viewer templates 创作原创 p5.js generative art。

## 安装

安装全部 skills：

```bash
npx skills@latest add AojiLi/codex-general-skills
```

安装单个 skill：

```bash
npx skills@latest add AojiLi/codex-general-skills --skill decision-advisor
npx skills@latest add AojiLi/codex-general-skills --skill voice-preserving-editor
npx skills@latest add AojiLi/codex-general-skills --skill frontend-design
npx skills@latest add AojiLi/codex-general-skills --skill algorithmic-art
```

## 目录结构

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

每个 skill 保留自己的说明、metadata、配套资源，以及适用时的许可证文件。

## 许可证

`frontend-design` 和 `algorithmic-art` 保留各自附带的 `LICENSE.txt`。除非之后明确添加统一许可证，仓库中的其他内容不适用单独的仓库级许可证。
