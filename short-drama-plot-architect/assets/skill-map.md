# short-drama-plot-architect 技能包导航图

这个文件用于快速说明整个 skill 包的结构、各文件用途、推荐调用顺序，以及不同任务场景下该优先读取哪些文件。

适合用途：
- 新加载这个 skill 时快速理解全貌
- 判断当前任务该读哪一个 references / templates 文件
- 避免只读 SKILL.md 而忽略更具体的模板与模式库
- 作为后续继续扩展本 skill 的总导航

---

## 一、技能包总目标

`short-drama-plot-architect` 的目标是：

把用户简短、模糊的一句话创意，升级成可落地、强冲突、强反转、强悬念、可拆集、适配中文商业短剧语境的成熟剧情方案。

它不是单一 prompt，而是一个完整的小型“短剧开发工具包”，包含：
- 主规则文件
- 示例参考
- 反转库
- 女性向模式库
- 输出模板
- 分集拆解模板

---

## 二、目录结构

```text
short-drama-plot-architect/
├── SKILL.md
├── references/
│   ├── example.md
│   ├── reversal-library.md
│   └── female-oriented-patterns.md
├── templates/
│   ├── output-template.md
│   └── episode-breakdown-template.md
└── assets/
    └── skill-map.md
```

---

## 三、每个文件的用途

### 1. SKILL.md

作用：
- 定义这个 skill 的总目标、适用范围、工作流程、默认风格、质量标准
- 说明从“模糊点子”到“剧情方案”的核心方法论
- 作为整个技能包的主入口

什么时候读：
- 每次加载本 skill 时都应该先读
- 当需要理解整体规则、默认行为、输出要求时优先读

它回答的问题：
- 这个 skill 到底是干什么的？
- 生成剧情时应遵守哪些原则？
- 什么样的结果才算合格？

---

### 2. references/example.md

作用：
- 提供一条“从一句创意到完整剧情方案”的成品示例
- 用于校准输出风格、完整度、成熟度、密度

什么时候读：
- 当你不确定结果该写到多细时
- 当你想模仿一版高完成度成品时
- 当你想检查自己的输出是否过于抽象、过于平铺时

它回答的问题：
- 一版合格输出长什么样？
- 剧情定位、人物、冲突、反转、拆集建议应该写到什么程度？

---

### 3. references/reversal-library.md

作用：
- 提供反转类型库、组合公式、阶段配置建议、强度分级、检查清单
- 用于专门加强“跌宕感”“局中局感”“反转密度”

什么时候读：
- 用户强调“反转多”“跌宕”“吸睛”“反杀”“局中局”时
- 初版剧情已经有框架，但不够刺激、不够起伏时
- 你发现剧情只有设定，没有足够反转层次时

它回答的问题：
- 反转该怎么设计才不生硬？
- 哪些反转适合开场、中段、高潮？
- 怎么组合身份反转、关系反转、证据反转、命运反转？

---

### 4. references/female-oriented-patterns.md

作用：
- 提供中文女性向短剧常见题材模式、情绪链、主角模板、关系模式、爽点痛点库
- 用于强化女性向情绪抓力和关系拉扯

什么时候读：
- 用户需求偏女性向
- 题材涉及婚恋、复仇、豪门、认亲、误认恩人、家庭伦理、情感博弈时
- 需要让主角成长弧线更成熟，不只是“打脸爽文”时

它回答的问题：
- 女性向短剧真正抓人的地方是什么？
- 女主成长应该怎么写，才不是单纯黑化？
- 爱情线、亲情线、复仇线怎么一起工作？

---

### 5. templates/output-template.md

作用：
- 提供标准剧情方案输出格式
- 规范剧情定位、高概念、人物、冲突、骨架、反转、爆点、拆集建议的呈现方式

什么时候读：
- 默认都建议读
- 当需要稳定产出结构清晰、可直接复用的结果时必须读

它回答的问题：
- 结果应该怎么组织？
- 每个部分应该写哪些字段？
- 如何避免输出混乱、缺项、层次不清？

---

### 6. templates/episode-breakdown-template.md

作用：
- 把剧情总纲继续拆成 10 集、20 集、30 集分集大纲
- 保证每一集都有目标、冲突、反转、爆点、钩子

什么时候读：
- 用户要“分集大纲”“拆成连续短剧”“每集节奏表”时必须读
- 用户已经有总纲，下一步要开发成连载型短剧时必须读

它回答的问题：
- 一部短剧该怎么拆成每集内容？
- 每集如何避免注水？
- 每集结尾怎么做钩子最有效？

---

### 7. assets/skill-map.md

作用：
- 也就是本文件
- 用于给整个技能包提供总导航与调用建议

什么时候读：
- 当你第一次接触这个 skill 包时
- 当你不确定该先看哪个文件时
- 当未来继续扩展新文件时

---

## 四、推荐调用顺序

### 场景 A：用户只给一句创意，要生成成熟剧情方案
推荐读取顺序：
1. `SKILL.md`
2. `templates/output-template.md`
3. `references/example.md`（可选，用于校准完成度）

### 场景 B：用户强调“跌宕、反转、局中局、吸睛”
推荐读取顺序：
1. `SKILL.md`
2. `templates/output-template.md`
3. `references/reversal-library.md`
4. `references/example.md`（可选）

### 场景 C：用户需求明显偏女性向
推荐读取顺序：
1. `SKILL.md`
2. `templates/output-template.md`
3. `references/female-oriented-patterns.md`
4. `references/reversal-library.md`（若还强调强反转）
5. `references/example.md`（可选）

### 场景 D：用户已经有剧情骨架，要拆成分集
推荐读取顺序：
1. `SKILL.md`
2. `templates/episode-breakdown-template.md`
3. `references/reversal-library.md`（若需要给每集加钩子）
4. `references/female-oriented-patterns.md`（若是女性向）

### 场景 E：用户要“女性向 + 强反转 + 分集拆解”完整版
推荐读取顺序：
1. `SKILL.md`
2. `templates/output-template.md`
3. `references/female-oriented-patterns.md`
4. `references/reversal-library.md`
5. `templates/episode-breakdown-template.md`
6. `references/example.md`

---

## 五、按任务类型选择文件

### 任务：只想把一句话扩成剧情方案
优先文件：
- `SKILL.md`
- `templates/output-template.md`

### 任务：剧情已有框架，但太平
优先文件：
- `references/reversal-library.md`

### 任务：想做更强女性向情绪抓力
优先文件：
- `references/female-oriented-patterns.md`

### 任务：要出分集大纲
优先文件：
- `templates/episode-breakdown-template.md`

### 任务：想参考一版成品长什么样
优先文件：
- `references/example.md`

---

## 六、执行时的简易决策树

可以按下面的判断走：

```text
用户给了一个模糊创意
  ↓
先读 SKILL.md
  ↓
是否要标准剧情输出？
  ├─ 是 → 读 templates/output-template.md
  └─ 否 → 继续判断
  ↓
是否强调女性向、婚恋、豪门、复仇、认亲？
  ├─ 是 → 读 references/female-oriented-patterns.md
  └─ 否 → 跳过
  ↓
是否强调跌宕、反转、局中局？
  ├─ 是 → 读 references/reversal-library.md
  └─ 否 → 跳过
  ↓
是否要求分集大纲？
  ├─ 是 → 读 templates/episode-breakdown-template.md
  └─ 否 → 跳过
  ↓
如需对齐成品质感 → 读 references/example.md
```

---

## 七、当前技能包覆盖能力

目前这套 skill 已能覆盖：

- 一句话创意扩写
- 高概念提炼
- 人物关系补全
- 冲突与秘密设计
- 反转链条强化
- 女性向模式强化
- 情绪爆点设计
- 标准格式输出
- 10/20/30 集分集拆解
- 追更钩子设计

也就是说，它已经从“单个提示词”升级成了一套小型短剧开发框架。

---

## 八、后续可继续扩展的方向

如果未来继续增强，可以优先考虑增加这些文件：

### references/title-hook-formulas.md
用途：
- 爆款标题公式
- 一句话卖点公式
- 宣发钩子语句

### references/male-oriented-patterns.md
用途：
- 男频逆袭、权力、复仇、事业流短剧模式库

### templates/character-sheet-template.md
用途：
- 统一输出角色卡
- 用于后续人物设定延展

### templates/scene-beat-template.md
用途：
- 把分集继续拆成场次节拍
- 适合进入更细的编剧开发阶段

---

## 九、最终说明

这个技能包的正确使用方式，不是只读主文件然后自由发挥。

更高质量的用法是：
- 用 `SKILL.md` 管总规则
- 用 `templates/` 管输出结构
- 用 `references/` 管风格强化与模式补充
- 用本文件 `assets/skill-map.md` 管导航与调度

最终目标只有一个：

让“用户一句模糊想法”可以稳定变成“成熟、吸睛、跌宕、可落地、可拆集的中文 AI 短剧剧情方案”。