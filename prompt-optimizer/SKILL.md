---
name: prompt-optimizer
description: Expand short and vague prompts into concrete, executable, high-quality prompts. 把用户简短模糊的提示词改写成具体、可执行、高质量的提示词。
version: 1.3.0
author: arfbt
license: MIT
metadata:
  hermes:
    tags: [prompt, prompting, rewrite, optimization, bilingual, chinese, english, specificity]
    category: creative
    requires_toolsets: []
---

# Prompt Optimizer

Expand short, vague, casual user input into concrete, structured, executable prompts.

把“很短、很泛、很口语”的用户输入，扩写成“目标明确、上下文完整、交付清晰、可直接执行”的高质量提示词。

## Purpose | 核心目标

This skill is not for cosmetic rewriting.
It is for turning an under-specified request into a usable prompt with clear goals, context, constraints, and deliverables.

这个 skill 不是做表面润色，
而是把“不够具体的需求”变成“可直接使用的高质量 prompt”。

The optimized prompt should:
1. clarify the task
2. clarify the target audience or object
3. add useful context and reasonable assumptions
4. define output format
5. define style, constraints, and boundaries
6. define quality standards
7. avoid asking too many questions too early

优化后的提示词应做到：
1. 明确任务目标
2. 明确对象/受众
3. 补充背景信息和合理假设
4. 明确输出格式
5. 明确风格、约束与边界
6. 明确质量标准
7. 避免一开始就追问太多问题

## When to Use | 何时使用

Use this skill when the user says things like:
- “帮我优化这个提示词”
- “把这句话改成更具体的 prompt”
- “我只有一个大概想法，帮我写成完整提示词”
- “Optimize this prompt”
- “Rewrite this into a better prompt”
- “Make this prompt more specific”

Also use it when the user gives only a short vague request, such as:
- “写个招聘文案”
- “做个 logo”
- “帮我分析这个产品”
- “写一个 Python 脚本”
- “做个短视频脚本”
- “write a landing page”
- “build a small app”
- “analyze this product idea”

## Core Principles | 工作原则

### 1. Produce first, ask later | 先产出，再补问
If the user gives very little information, produce a solid default version first.
Do not stop immediately for clarification unless missing information would meaningfully change the result.

如果用户信息很少，先基于常见场景补全一个可用版本。
不要因为缺少少量细节就立刻停下来追问，除非这些信息会实质改变结果。

### 2. Preserve intent | 保留原意
Stay faithful to the user's original intention.
Do not silently change the task into a broader or different one.

优化时必须忠于用户原始需求。
不要擅自换题、扩题或偏题。

### 3. Make it concrete | 从模糊到具体
Prefer adding:
- what the task is
- who it is for
- what success looks like
- what the output should contain
- what style to use
- what constraints apply
- what to avoid

优先补全：
- 任务是什么
- 为谁而做
- 想达到什么效果
- 输出包含哪些内容
- 风格是什么
- 有哪些约束
- 需要避免什么

### 4. Favor usability | 默认实用主义
Unless specified otherwise, the result should be:
- directly copyable
- clear and structured
- constrained enough to guide execution
- practical instead of fluffy

如果用户没有特别要求，默认输出应：
- 可直接复制使用
- 结构清晰
- 约束充分
- 重实用，少空话

## Task Type Recognition | 任务类型识别

First identify the task category.

先识别原始提示词的任务类型。

Common categories:
- writing
- analysis
- coding
- image/design
- learning/coaching
- marketing/operations
- general execution

常见类型：
- 写作类
- 分析类
- 代码类
- 图像/设计类
- 学习/辅导类
- 运营/营销类
- 通用执行类

## Key Dimensions to Fill | 关键补全维度

Always try to fill these dimensions when helpful:

优先补全以下维度：
- background | 背景
- goal | 目标
- target audience/object | 面向对象
- deliverables/output | 输出内容
- style/tone | 风格语气
- constraints | 约束条件
- success criteria | 质量标准

## Category-Specific Guidance | 分类型补全建议

### A. Writing | 写作类
Add:
- audience
- platform/channel
- tone
- length range
- whether title, hook, CTA, sections are needed

补充：
- 受众是谁
- 发布平台
- 文风语气
- 字数范围
- 是否需要标题、开头钩子、结尾 CTA

### B. Analysis | 分析类
Add:
- what is being analyzed
- analysis dimensions or framework
- summary vs deep dive
- whether conclusion, table, recommendations, priorities are needed

补充：
- 分析对象
- 分析框架
- 概览还是深入
- 是否需要结论、表格、建议、优先级

### C. Coding | 代码类
Add:
- language/framework
- input/output
- runtime environment
- comments/tests/error handling
- whether the user wants MVP simplicity or more engineering rigor

补充：
- 编程语言/框架
- 输入输出
- 运行环境
- 注释/测试/错误处理
- 优先最小可用还是工程化

Recommended line:
```text
Please prioritize a minimum viable implementation that is runnable, readable, and well-structured, with necessary comments and handling for common edge cases.
```

推荐附加句：
```text
请优先提供最小可用版本，并确保代码可运行、结构清晰、包含必要注释；如果有潜在边界条件，请一并处理。
```

### D. Image / Design | 图像/设计类
Add:
- subject
- scene
- style
- lighting
- camera/composition
- color palette
- materials/textures
- aspect ratio
- negative prompt elements

补充：
- 主体
- 场景
- 风格
- 光线
- 镜头/构图
- 配色
- 材质
- 比例
- 负面提示

Recommended line:
```text
Please specify the subject, composition, style, lighting, color palette, camera language, and elements to avoid so the output is more controllable and consistent.
```

推荐附加句：
```text
请把画面主体、构图、风格、光线、色彩、镜头语言和需要避免的元素都写清楚，确保生成结果稳定且可控。
```

## Output Format | 输出格式

Default output should contain 4 parts:

默认输出分为 4 段：

### 1. Optimized Prompt | 优化后的提示词
A fully usable prompt the user can copy directly.

给出一版可以直接复制使用的完整版 prompt。

### 2. Short Version | 精简版
A shorter but still concrete version.

给出一版更短但仍然具体的 prompt。

### 3. What Was Added | 补全了哪些内容
List the key details you added.

用项目符号简要说明补全了哪些关键信息。

### 4. Optional Follow-up Questions | 可选补充问题
Ask only 3-5 high-value follow-up questions if useful.
If the current version is already enough, say so.

只给 3-5 个真正高价值的问题用于下一轮优化。
如果当前信息已足够，也可以直接说明“当前已可直接使用”。

## Response Template | 推荐回复模板

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

## Prompt Skeleton | Prompt 骨架

Use this structure whenever suitable:

```text
You are [role/expert identity].
Please help me complete [specific task].

Background:
[user-provided info + reasonable assumptions]

Goal:
[desired result]

Target audience/object:
[who it is for]

Output requirements:
1. ...
2. ...
3. ...

Style requirements:
[tone/style]

Constraints:
- ...
- ...

Quality standard:
- ...
- ...

If information is missing, make reasonable assumptions based on common business, creative, or development scenarios, and prioritize giving a directly usable version first.
```

对应中文骨架：

```text
你是[角色/专家身份]。
请帮我完成[具体任务]。

背景信息：
[用户已提供的信息 + 合理补全的假设]

目标：
[想要达成的结果]

面向对象：
[受众/用户/读者/客户]

输出要求：
1. ...
2. ...
3. ...

风格要求：
[语气、风格、调性]

约束条件：
- ...
- ...

质量标准：
- ...
- ...

如果信息不足，请基于常见商业/创作/开发场景做合理假设，并优先给出可直接使用的版本。
```

## Example Scenarios | 示例场景

### Example 1 | 示例 1
Original:
“帮我写个招聘文案”

Optimization direction:
- define the role
- define company stage
- define target candidate
- define structure and tone

优化方向：
- 明确岗位
- 明确公司阶段
- 明确目标候选人
- 明确结构与语气

### Example 2 | 示例 2
Original:
“写个 Python 脚本清理 Excel”

Optimization direction:
- specify Python + pandas
- define common cleaning tasks
- define input/output
- require comments and running instructions

优化方向：
- 明确 Python + pandas
- 明确常见清洗动作
- 明确输入输出
- 要求注释和运行说明

## Quality Checklist | 质量检查清单

Before finalizing, check:
- Is it substantially more specific than the original?
- Did it add real constraints rather than empty wording?
- Is it directly usable as a prompt?
- Did it preserve the user's original intent?
- Did it include a shorter version?
- Did it avoid useless verbosity?

输出前检查：
- 是否比原始提示词显著更具体？
- 是否增加了有效约束，而不是空泛变长？
- 是否可直接复制使用？
- 是否保留了用户原意？
- 是否提供了精简版？
- 是否避免了无意义的废话？

## Common Mistakes to Avoid | 常见错误

Do not:
- just paraphrase the original sentence
- over-assume and drift away from intent
- ask too many clarification questions too early
- output theory without a ready-to-use prompt
- make it fancy but not actionable

不要这样做：
- 只是改写原句，没有新增有效信息
- 过度脑补，偏离原意
- 一上来追问太多问题
- 只讲方法，不给成品 prompt
- 看起来华丽，实际上不可执行

## Default Behavior | 默认行为

If information is incomplete:
- infer from the most common scenario
- make assumptions explicit when useful
- give a usable version first
- then offer a few high-value refinements

当信息不足时：
- 基于最常见场景补全
- 必要时明确哪些是合理假设
- 先给一个能用的版本
- 再提供少量高价值追问

## Final Goal | 最终目标

Enable the user to say one short sentence and still receive a concrete, clear, high-quality prompt they can use immediately.

让用户哪怕只说一句话，也能立刻得到一版具体、清晰、可执行的高质量提示词。
