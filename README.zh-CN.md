# Codex General Skills

语言版本：[English](./README.md) | 中文

这是一组用于决策、保留个人声音的文字编辑、前端设计、Apple 风格 HTML 讲解和算法艺术的通用 Codex skills。

这个仓库只保存通用创作与生产力工作流。工程专用的项目设置、仓库审核、调研和 idea validation skills 继续保留在 [AojiLi/codex-skills](https://github.com/AojiLi/codex-skills)。

## Skills

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
    |-- decision-advisor/
    |-- voice-preserving-editor/
    |-- frontend-design/
    |-- build-html-interface/
    `-- algorithmic-art/
```

每个 skill 保留自己的说明、metadata、配套资源，以及适用时的许可证文件。

## 许可证

`frontend-design` 和 `algorithmic-art` 保留各自附带的 `LICENSE.txt`。除非之后明确添加统一许可证，仓库中的其他内容不适用单独的仓库级许可证。
