---
name: prompt-optimizer
description: Expand short and vague prompts into concrete, executable, high-quality prompts. 把用户简短模糊的提示词改写成具体、可执行、高质量的提示词。
version: 1.2.0
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

## Output Format | 输出格式

Default output should contain 4 parts:
1. Optimized Prompt | 优化后的提示词
2. Short Version | 精简版
3. What Was Added | 补全了哪些内容
4. Optional Follow-up Questions | 可选补充问题

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

## Final Goal | 最终目标

Enable the user to say one short sentence and still receive a concrete, clear, high-quality prompt they can use immediately.

让用户哪怕只说一句话，也能立刻得到一版具体、清晰、可执行的高质量提示词。
