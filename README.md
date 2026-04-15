# Skills

Better prompts. Better handoff. Better results.

A public bilingual skill repository for turning vague prompts into concrete, executable instructions — starting with `prompt-optimizer`.

This repository publishes bilingual AI skills that help users turn rough requests into clear, executable instructions — starting with `prompt-optimizer`.

更好的 prompt，更好的交接，更好的结果。

这是一个公开的双语 skill 仓库，专门用来把模糊提示词变成具体、可执行的指令，其中首个技能是 `prompt-optimizer`。

这个仓库发布双语 AI skills，帮助用户把粗糙需求转化为清晰、可执行的指令，其中首个技能是 `prompt-optimizer`。

## What this repository is | 这是什么仓库

This is a public repository of reusable AI agent skills.

这是一个公开的、可复用的 AI Agent Skills 仓库。

The main skill in this repository is:

当前仓库的核心 skill 是：

- `prompt-optimizer` — a bilingual skill that transforms short, vague prompts into concrete, structured, high-quality prompts
- `prompt-optimizer` —— 一个双语 skill，用于把简短、模糊的提示词改写成具体、结构化、高质量的 prompt

It is especially useful for:
- writing
- coding
- analysis
- design / image prompting
- marketing
- study / teaching
- general task clarification

它尤其适合：
- 写作
- 代码生成
- 分析总结
- 设计 / 图像生成
- 营销文案
- 学习 / 教学
- 通用任务澄清

---

## Available Skills | 可用技能

### prompt-optimizer

Turn short, vague prompts into concrete, executable, high-quality prompts.

把简短、模糊的提示词扩写成具体、可执行、高质量的提示词。

What it helps add | 它会自动补全：
- goal clarity | 目标明确
- target audience | 面向对象
- context and assumptions | 背景与合理假设
- output requirements | 输出要求
- style and tone | 风格语气
- constraints and boundaries | 约束条件
- quality criteria | 质量标准

---

## Installation | 安装方式

Install with `npx skills`:

使用 `npx skills` 安装：

```bash
npx skills add arfbt/skills@prompt-optimizer -g -y
```

If you use Hermes, you can also add this repository as a skill source:

如果你使用 Hermes，也可以把这个仓库作为 skill 源添加：

```bash
hermes skills tap add arfbt/skills
```

Then install or use the skill through Hermes.

然后通过 Hermes 安装或使用该 skill。

---

## Why this skill exists | 为什么做这个 skill

Many users know what they want, but do not know how to phrase it as a strong prompt.

很多用户知道自己想要什么，但不知道怎么把它写成一个强 prompt。

They often write things like:
- “写个招聘文案”
- “做个 logo”
- “帮我分析这个产品”
- “写一个 Python 脚本”
- “Optimize this prompt”
- “Make this more specific”

These requests are directionally useful, but too vague for consistent high-quality output.

这些请求方向是对的，但通常过于模糊，难以稳定得到高质量结果。

`prompt-optimizer` solves that by turning rough requests into prompts that are:
- specific
- structured
- constrained
- directly usable

`prompt-optimizer` 的作用，就是把这类粗糙需求转化为：
- 更具体
- 更结构化
- 更有约束
- 可直接使用

---

## Usage Examples | 使用示例

After installing `prompt-optimizer`, you can use it with requests like:

安装 `prompt-optimizer` 后，你可以这样使用：

- 帮我优化这个提示词：写个招聘文案
- 把这句话改成更具体的 prompt：做一个 AI 首页
- 用 prompt-optimizer 改写：写个 Python 脚本清理 Excel
- Optimize this prompt: write a product launch email
- Rewrite this into a better prompt: build a landing page for an AI app

### Example input | 示例输入

```text
写个 Python 脚本清理 Excel
```

### What `prompt-optimizer` will do | `prompt-optimizer` 会做什么

It will typically expand the request by adding:
- Python + pandas as a likely stack
- common Excel cleaning tasks
- input/output expectations
- comments and usage instructions
- basic quality constraints

它通常会自动补全：
- Python + pandas 作为合理技术栈
- 常见 Excel 清洗动作
- 输入输出要求
- 注释与运行说明
- 基本质量约束

So the result becomes a directly usable prompt instead of a vague sentence.

这样，结果就会从一句模糊的话，变成一个可直接复制使用的 prompt。

---

## What the output usually looks like | 输出通常长什么样

A typical `prompt-optimizer` response includes 4 parts:

一个典型的 `prompt-optimizer` 输出通常包含 4 部分：

1. Optimized Prompt | 优化后的提示词
2. Short Version | 精简版
3. What Was Added | 补全了哪些内容
4. Optional Follow-up Questions | 可选补充问题

Example structure:

示例结构：

```text
优化后的提示词 / Optimized Prompt:
[full prompt]

精简版 / Short Version:
[short prompt]

我补全了这些关键细节 / What I added:
- ...
- ...
- ...

如果你愿意，我还可以继续细化这些点 / Optional follow-up:
- ...
- ...
- ...
```

---

## Main Use Cases | 主要使用场景

### 1. Writing | 写作类
Examples:
- recruitment copy
- product intros
- emails
- article outlines
- short video scripts

示例：
- 招聘文案
- 产品介绍
- 邮件
- 提纲
- 短视频脚本

### 2. Coding | 代码类
Examples:
- scripts
- web pages
- demos
- dashboards
- small tools

示例：
- 脚本
- 网页
- demo
- 管理后台
- 小工具

### 3. Analysis | 分析类
Examples:
- product analysis
- competitor analysis
- strategy review
- problem breakdown

示例：
- 产品分析
- 竞品分析
- 策略分析
- 问题拆解

### 4. Image / Design | 图像 / 设计类
Examples:
- logo prompts
- poster prompts
- illustration prompts
- cover image prompts

示例：
- logo prompt
- 海报 prompt
- 插画 prompt
- 封面 prompt

### 5. Marketing / Growth | 营销 / 增长类
Examples:
- ad copy
- campaign planning
- growth ideas
- landing page copy

示例：
- 广告文案
- 活动方案
- 增长思路
- 落地页文案

### 6. Learning / Teaching | 学习 / 教学类
Examples:
- study plans
- tutoring prompts
- concept explanation prompts
- quiz generation prompts

示例：
- 学习计划
- 辅导 prompt
- 概念讲解 prompt
- 出题 prompt

---

## Repository Structure | 仓库结构

```text
.
├── README.md
├── LICENSE
├── CHANGELOG.md
└── prompt-optimizer/
    ├── SKILL.md
    └── references/
        ├── examples.md
        ├── use-cases.md
        └── output-patterns.md
```

### File Guide | 文件说明

- `README.md`
  - repository overview and installation instructions
  - 仓库介绍与安装说明

- `prompt-optimizer/SKILL.md`
  - the main skill definition
  - skill 主文件

- `prompt-optimizer/references/examples.md`
  - bilingual examples of prompt transformation
  - 双语示例文件

- `prompt-optimizer/references/use-cases.md`
  - common usage scenarios
  - 典型使用场景

- `prompt-optimizer/references/output-patterns.md`
  - recommended response/output patterns
  - 推荐输出模式

- `LICENSE`
  - open-source license
  - 开源许可证

- `CHANGELOG.md`
  - version history
  - 版本记录

---

## Design Principles | 设计原则

`prompt-optimizer` follows these principles:

`prompt-optimizer` 遵循以下原则：

### 1. Produce first, ask later | 先产出，再补问
If the user gives very little information, produce a strong default version first.

如果用户信息很少，先基于常见场景产出一个强可用版本。

### 2. Preserve intent | 保留原意
Do not silently change the user's request into a different task.

不要擅自把用户原始需求改造成另一个任务。

### 3. Make prompts concrete | 从模糊到具体
Add structure, constraints, audience, deliverables, and quality criteria.

补充结构、约束、对象、交付物和质量标准。

### 4. Favor usability | 实用优先
The output should be directly usable, not just theoretically “better”.

输出应是“能直接用”的，而不是只是“看起来更专业”。

---

## Who this is for | 适合谁用

This repository is useful for:
- AI tool builders
- prompt engineers
- agent developers
- content creators
- product managers
- educators
- anyone who writes rough prompts and wants better results

这个仓库适合：
- AI 工具开发者
- Prompt 工程实践者
- Agent 开发者
- 内容创作者
- 产品经理
- 教育工作者
- 任何经常写“粗糙 prompt”但希望结果更好的人

---

## Roadmap | 规划方向

Possible future improvements:
- more examples
- more domain-specific prompt patterns
- more skills in the repository
- richer bilingual prompt templates
- stronger support for coding / design / analysis subtypes

后续可能继续增强：
- 更多 examples
- 更多垂直领域 prompt 模式
- 更多可安装 skills
- 更丰富的双语模板
- 更强的代码 / 设计 / 分析子场景支持

---

## Contributing | 贡献方式

Issues and pull requests are welcome.

欢迎提交 issue 和 pull request。

Good contributions include:
- better bilingual examples
- clearer use cases
- improved metadata
- new reference docs
- additional reusable skills

欢迎的贡献包括：
- 更好的中英双语示例
- 更清晰的 use cases
- 更完善的元信息
- 新的参考文档
- 更多可复用 skills

---

## Changelog | 更新记录

See:

请查看：

- `CHANGELOG.md`

---

## License

MIT
