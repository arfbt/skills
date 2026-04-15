# Skills

From one vague sentence to a usable prompt.

This repository publishes bilingual AI skills that help users turn rough requests into clear, executable instructions — starting with `prompt-optimizer`.

从一句模糊的话，到一个能直接用的 prompt。

这个仓库发布双语 AI skills，帮助用户把粗糙需求转化为清晰、可执行的指令，其中首个技能是 `prompt-optimizer`。

## What this repository is | 这是什么仓库

This is a public repository of reusable AI agent skills.

这是一个公开的、可复用的 AI Agent Skills 仓库。

The main skill in this repository is:

当前仓库的核心 skill 是：

- `prompt-optimizer` — a bilingual skill that transforms short, vague prompts into concrete, structured, high-quality prompts
- `prompt-optimizer` —— 一个双语 skill，用于把简短、模糊的提示词改写成具体、结构化、高质量的 prompt

## Installation | 安装方式

Install with `npx skills`:

```bash
npx skills add arfbt/skills@prompt-optimizer -g -y
```

If you use Hermes, you can also add this repository as a skill source:

```bash
hermes skills tap add arfbt/skills
```

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

## License

MIT
