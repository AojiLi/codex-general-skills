<a id="english"></a>

# Codex General Skills

Language: English | [中文](#user-content-zh-cn)

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

### [build-html-interface](./skills/build-html-interface/SKILL.md)

Use it to turn concepts, formulas, documents, or software repositories into desktop-first Apple-style visual explanations. It creates one self-contained `index.html` with precise system typography, spacious composition, quiet materials, diagrams, and restrained interaction. Repository tasks map real modules, files, or data flows. It performs one fast desktop browser check and does not default to mobile verification, full app states, broad research, or heavy animation engineering.

```text
Use $build-html-interface to explain this neural-network formula as a polished Apple-style visual HTML page.
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
npx skills@latest add AojiLi/codex-general-skills --skill build-html-interface
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
    |-- build-html-interface/
    `-- algorithmic-art/
```

Each skill keeps its own instructions, metadata, bundled resources, and license files where applicable.

## Licenses

`frontend-design` and `algorithmic-art` retain their bundled `LICENSE.txt` files. Other repository content has no separate repository-wide license unless one is added explicitly.

<a id="zh-cn"></a>

# Codex General Skills

语言版本：[English](#user-content-english) | 中文

这是一组用于 idea 验证、决策、保留个人声音的文字编辑、前端设计、Apple 风格 HTML 讲解和算法艺术的通用 Codex skills。

这个仓库只保存通用创作与生产力工作流。工程专用的项目设置、仓库审核和一手资料调研 skills 继续保留在 [AojiLi/codex-skills](https://github.com/AojiLi/codex-skills)。

## Skills

### [idea-validator](./skills/idea-validator/SKILL.md)

适合在实现之前分析仍不完整的 idea、产品概念、研究方向、项目计划或架构想法。它会一次问一个问题，澄清问题、用户、方案、时机、成功标准、约束和未知项。你确认 brief 后，它会询问使用五个独立 research subagents，还是在主 agent 中顺序执行相同研究路线；随后由主 agent 汇总证据，自动运行最多五轮 skeptic loop，最后给出可行性、价值、差异化、MVP、实现、验证、风险和下一步结论。

```text
使用 $idea-validator 在我开始实现前分析这个 idea：[描述 idea]。
```

### [decision-advisor](./skills/decision-advisor/SKILL.md)

适合重要选择、取舍、选项比较或“要不要做”问题。它会先澄清背景、目的、核心问题、候选选项、司法辖区、约束和决策权重。你确认这个决策框架后，它会询问使用六个独立 lens subagents，还是由主 agent 顺序分析；随后从经济、战略、心理、风险、法律/监管和技术可行性六个角度分析并执行 critique-revision loops。最终结果包括明确推荐、备选方案、行动计划、置信度和复盘信号。

```text
使用 $decision-advisor 帮我决定应该接受这个工作机会，还是继续经营自己的公司。
```

### [voice-preserving-editor](./skills/voice-preserving-editor/SKILL.md)

适合修改粘贴文字、Markdown、README、DOCX 或 Google Docs，同时避免把内容改成通用 AI 腔。它会阅读目标段落周围的上下文，根据请求选择轻度、中度或明确要求的重写，只修改指定位置，并保留作者的立场、语气、节奏、用词和情绪强度；遇到不确定事实时会标记问题，而不是编造修正。

```text
使用 $voice-preserving-editor 修改这段 README，但不要改变我的语气：[粘贴文字]。
```

### [frontend-design](./skills/frontend-design/SKILL.md)

适合需要鲜明视觉身份的新界面或现有界面重设计。它会先把设计落到真实主题、用户和页面任务上，建立紧凑的颜色、字体、布局和 signature element 系统，比较布局思路，在实现前批评通用模板选择，然后完成代码并通过截图检查响应式、可访问性和交互细节。

```text
使用 $frontend-design 根据产品的真实工作流和现有代码重新设计这个 dashboard。
```

### [build-html-interface](./skills/build-html-interface/SKILL.md)

适合把概念、公式、文档或软件项目仓库转换成桌面优先的 Apple 风格可视化讲解。它会生成一个自包含的 `index.html`，使用精确的系统字体、宽松排版、克制材质、清晰图解和必要交互；仓库任务会映射真实模块、文件或数据流。默认只做一次快速桌面浏览器检查，不再自动执行移动端验证、完整应用状态、广泛调研或重型动画工程。

```text
使用 $build-html-interface 把这个神经网络公式做成精致的 Apple 风格 HTML 可视化讲解。
```

### [algorithmic-art](./skills/algorithmic-art/SKILL.md)

适合使用 p5.js 创作原创 generative art 或 computational art。它会先写一份简洁的 algorithmic philosophy，从请求中提取一个含蓄的 conceptual seed，然后在附带的交互 viewer template 中实现可复现的 seeded algorithm。最终输出是一个自包含 HTML artifact，带有参数控制、seed navigation、reset/regenerate 和 PNG 下载功能。

```text
使用 $algorithmic-art 创作一个受轨道共振和潮汐运动启发的交互式生成艺术作品。
```

## 安装

安装全部 skills：

```bash
npx skills@latest add AojiLi/codex-general-skills
```

安装单个 skill：

```bash
npx skills@latest add AojiLi/codex-general-skills --skill idea-validator
npx skills@latest add AojiLi/codex-general-skills --skill decision-advisor
npx skills@latest add AojiLi/codex-general-skills --skill voice-preserving-editor
npx skills@latest add AojiLi/codex-general-skills --skill frontend-design
npx skills@latest add AojiLi/codex-general-skills --skill build-html-interface
npx skills@latest add AojiLi/codex-general-skills --skill algorithmic-art
```

## 目录结构

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
    |-- build-html-interface/
    `-- algorithmic-art/
```

每个 skill 保留自己的说明、metadata、配套资源，以及适用时的许可证文件。

## 许可证

`frontend-design` 和 `algorithmic-art` 保留各自附带的 `LICENSE.txt`。除非之后明确添加统一许可证，仓库中的其他内容不适用单独的仓库级许可证。
