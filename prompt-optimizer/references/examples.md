# Prompt Optimizer Examples

This file contains bilingual examples showing how `prompt-optimizer` transforms short, vague prompts into concrete, executable prompts.

这个文件提供中英双语示例，展示 `prompt-optimizer` 如何把简短、模糊的提示词改写成具体、可执行的高质量提示词。

---

## Example 1 — Recruitment Copy | 招聘文案

### Original | 原始输入
帮我写个招聘文案

### Optimized Direction | 优化方向
- define the role
- define the company stage
- define the target candidate
- define the output structure
- define tone and length

- 明确岗位
- 明确公司阶段
- 明确目标候选人
- 明确输出结构
- 明确语气和长度

### Optimized Prompt | 优化后的提示词
你是一名资深招聘文案策划，请帮我写一篇用于招聘平台发布的岗位招聘文案，岗位为“AI 产品经理”。

背景信息：
这是一家早期成长型 AI 创业公司，团队规模 20~50 人，产品方向为企业级 AI 应用。

目标：
吸引有 3~5 年经验、具备 AI 产品设计和跨团队协作能力的候选人投递。

面向对象：
对 AI 行业有热情、希望参与 0 到 1 或 1 到 10 产品建设的中高级产品经理。

输出要求：
1. 产出一个有吸引力的职位标题
2. 写清岗位职责、任职要求、加分项
3. 突出团队机会、业务前景和成长空间
4. 语言专业但不要死板
5. 结尾加入明确的投递引导

风格要求：
真诚、专业、有吸引力，避免空泛和套话。

约束条件：
控制在 400~600 字，适合直接发布到 Boss 直聘或拉勾。

质量标准：
让候选人快速理解岗位价值、团队亮点和能力要求。

---

## Example 2 — Excel Cleaning Script | Excel 清洗脚本

### Original | 原始输入
写个 Python 脚本清理 Excel

### Optimized Direction | 优化方向
- specify Python + pandas
- define common cleaning tasks
- define input/output
- require comments and running instructions

- 明确 Python + pandas
- 明确常见清洗动作
- 明确输入输出
- 要求注释和运行方式

### Optimized Prompt | 优化后的提示词
你是一名经验丰富的 Python 数据处理工程师，请帮我编写一个用于清洗 Excel 数据的 Python 脚本。

背景信息：
我有一份业务数据 Excel，里面可能存在空值、重复项、格式不统一、日期格式混乱、手机号/邮箱字段脏数据等问题。

目标：
生成一个可复用的清洗脚本，读取原始 Excel 后输出一份清洗完成的新文件。

输出要求：
1. 使用 Python 实现
2. 优先使用 pandas
3. 包含读取文件、数据清洗、保存结果的完整流程
4. 对常见问题做处理：去重、空值处理、去除首尾空格、统一日期格式、统一字段命名
5. 关键步骤加注释
6. 给出运行方法和依赖安装方式

约束条件：
代码应尽量简单、可直接运行；如果某些字段名未知，请把可配置项集中放在脚本顶部。

质量标准：
脚本结构清晰、便于修改、对新手友好。

---

## Example 3 — Landing Page Copy | 落地页文案

### Original | 原始输入
写个产品介绍

### Optimized Direction | 优化方向
- identify product type
- identify audience
- define usage scenario
- define structure
- define CTA

- 明确产品类型
- 明确目标用户
- 明确使用场景
- 明确结构
- 明确行动引导

### Optimized Prompt | 优化后的提示词
你是一名专业的产品营销文案策划，请帮我写一版 AI SaaS 产品的官网产品介绍文案。

背景信息：
该产品面向中小企业，核心能力是通过 AI 自动整理客户沟通记录、生成销售跟进建议，并提升团队协作效率。

目标：
让首次访问官网的潜在客户在短时间内理解产品价值，并愿意预约演示或注册试用。

面向对象：
销售团队负责人、运营负责人、中小企业管理者。

输出要求：
1. 写一个清晰有吸引力的主标题
2. 写一个简洁有力的副标题
3. 提炼 3~5 个核心卖点
4. 加入典型使用场景说明
5. 结尾加入明确 CTA，如“预约演示”或“立即试用”

风格要求：
专业、清晰、可信，不要夸张，不要空泛套话。

约束条件：
适合官网首页首屏到卖点区块使用，整体简洁有力。

质量标准：
读者能迅速理解产品是什么、适合谁、为什么值得使用。

---

## Example 4 — Logo Prompt | Logo 生成提示词

### Original | 原始输入
做个 logo

### Optimized Direction | 优化方向
- define brand type
- define visual style
- define color direction
- define application scenario
- define elements to avoid

- 明确品牌类型
- 明确视觉风格
- 明确色彩方向
- 明确使用场景
- 明确避免元素

### Optimized Prompt | 优化后的提示词
你是一名资深品牌设计师，请为一个 AI 教育产品设计 logo 生成提示词。

背景信息：
该品牌面向学生和年轻职场人，主打“高效学习、智能辅导、清晰成长路径”的产品体验，品牌气质偏科技感、可信赖、年轻化。

目标：
生成适合用于 AI 绘图模型或设计方向探索的高质量 logo prompt。

输出要求：
1. 明确 logo 的主体概念
2. 描述整体风格，如极简、现代、科技感、扁平化
3. 指定推荐配色方向
4. 说明适合的构图形式，如图形+文字或纯图形
5. 加入适用场景，如官网、App 图标、宣传物料
6. 提供需要避免的设计元素

风格要求：
简洁、现代、识别度高，不要复杂堆叠。

约束条件：
避免过度通用的 AI 脑回路图标、过时渐变、过于卡通的风格。

质量标准：
logo 概念清晰、易识别、具备品牌感和实际落地性。

---

## Example 5 — Video Script | 短视频脚本

### Original | 原始输入
做个短视频脚本

### Optimized Direction | 优化方向
- define platform
- define audience
- define duration
- define structure
- define hook and CTA

- 明确平台
- 明确受众
- 明确时长
- 明确结构
- 明确开头钩子和结尾 CTA

### Optimized Prompt | 优化后的提示词
你是一名短视频内容策划，请帮我写一个适合抖音发布的 30~60 秒短视频脚本。

背景信息：
视频内容是介绍一个 AI 写作工具，目标用户是需要高频写文案、做内容运营、写邮件或写报告的职场人。

目标：
通过短视频快速传达工具价值，提升用户对产品的兴趣，并引导点击主页了解更多。

输出要求：
1. 给出一个强吸引力的开头钩子
2. 用口语化方式介绍用户痛点
3. 展示产品的核心功能和使用效果
4. 脚本分镜头写出，每段说明画面和台词
5. 结尾加入明确 CTA

风格要求：
节奏快、口语化、信息密度高，适合短视频传播。

约束条件：
时长控制在 30~60 秒内，语言自然，不要像广告硬广。

质量标准：
前 3 秒能抓人，整体节奏流畅，卖点表达清楚。

---

## Example 6 — Product Analysis | 产品分析

### Original | 原始输入
帮我分析这个产品

### Optimized Direction | 优化方向
- define analysis object
- define framework
- define output depth
- define whether recommendations are needed

- 明确分析对象
- 明确分析框架
- 明确输出深度
- 明确是否需要建议

### Optimized Prompt | 优化后的提示词
你是一名资深产品分析师，请帮我对一个 AI 笔记产品进行结构化分析。

背景信息：
该产品主打会议记录整理、知识归档、智能总结和团队协作，目标用户是知识工作者和中小团队。

目标：
从产品定位、核心功能、用户价值、竞争优势和潜在问题几个角度进行分析，并输出可执行建议。

输出要求：
1. 先用一段话总结产品定位
2. 分析核心用户群和核心场景
3. 拆解主要功能模块及价值
4. 分析产品优势与短板
5. 给出 3~5 条可执行优化建议
6. 最后做一个简短结论总结

风格要求：
专业、清晰、结构化。

约束条件：
不要只给泛泛而谈的评价，要有明确分析维度。

质量标准：
分析逻辑清楚，结论有依据，建议具备可执行性。

---

## Example 7 — English Copywriting Prompt

### Original
write a launch email

### Optimized Direction
- define product type
- define audience
- define email goal
- define structure
- define tone and CTA

### Optimized Prompt
You are an experienced SaaS email copywriter. Please write a product launch email for a new AI note-taking assistant.

Background:
The product helps teams automatically summarize meetings, extract action items, and organize follow-ups. The audience is busy professionals, founders, and team managers.

Goal:
Announce the launch, explain the value clearly, and drive readers to start a free trial.

Target audience:
Professionals who attend many meetings and want to reduce manual note-taking and follow-up work.

Output requirements:
1. Write 3 subject line options
2. Write 1 preview text option
3. Write the full email body
4. Clearly explain the problem and the product's value
5. Include a strong CTA for starting a free trial

Style requirements:
Clear, concise, professional, and persuasive without sounding overly promotional.

Constraints:
Keep it suitable for a SaaS launch email and avoid buzzword-heavy language.

Quality standard:
The email should be easy to scan, easy to understand, and strong enough to increase trial conversions.

---

## Example 8 — English Landing Page Prompt

### Original
build a landing page for an ai app

### Optimized Direction
- define app category
- define target audience
- define page sections
- define tone
- define implementation expectations

### Optimized Prompt
You are a senior frontend engineer and conversion-focused product designer. Please create a landing page for an AI study assistant web app.

Background:
The app helps students summarize notes, generate quizzes, and build personalized study plans. The main audience is university students and exam-focused learners.

Goal:
Create a landing page that clearly communicates the product value and increases sign-ups for a free trial.

Output requirements:
1. Include a hero section with headline, subheadline, and CTA
2. Include a benefits section with 3-5 core value propositions
3. Include a product features section
4. Include a simple social proof or trust section
5. Include a final CTA section
6. If generating code, provide a complete single-file implementation or clearly structured component output

Style requirements:
Modern, clean, student-friendly, and trustworthy.

Constraints:
Avoid generic AI buzzwords and make the messaging concrete and benefit-driven.

Quality standard:
The page should make users understand what the app does, why it matters, and why they should sign up.

---

## Example 9 — Exam Generator Web App | 试卷生成网页

### Original | 原始输入
生成一个导入excel题库生成试卷的网页

### Optimized Direction | 优化方向
- define user scenario
- define feature modules
- define supported question types
- define export requirements
- define technical constraints

- 明确使用场景
- 明确功能模块
- 明确题型支持
- 明确导出要求
- 明确技术约束

### Optimized Prompt | 优化后的提示词
你是一名资深前端工程师兼轻量级 Web 工具开发专家，请帮我开发一个“基于 Excel 题库导入并生成 Word 试卷”的单页网页应用。

背景信息：
这是一个面向教师、教培机构或出题人员使用的网页工具，主要用于从 Excel 题库中读取题目数据，按题型管理题目，并生成可下载的 Word 格式试卷。

目标：
支持题库导入、网页新增题目、题目管理、试卷生成和试题导出，形成完整闭环。

输出要求：
1. 支持导入 Excel 题库
2. 支持新增单选题、多选题、判断题、填空题
3. 支持生成试卷
4. 支持导出 Word 格式试卷
5. 支持导出试题数据
6. 允许通过 CDN 引入外部库
7. 直接输出完整可运行的单文件 HTML

风格要求：
结构清晰、实用优先、便于后续扩展。

约束条件：
尽量纯前端实现，不依赖复杂后端。

质量标准：
页面可直接运行，功能闭环完整，题型支持真实可用。

---

## Example 10 — Minimal Follow-up Questions | 高价值追问示例

When information is missing, do not ask too many questions. Ask only high-value follow-ups such as:

当信息不足时，不要一次问很多问题。只追问真正高价值的问题，例如：

### For writing | 写作类
- 这篇内容主要发布在哪个平台？
- 目标读者是谁？
- 你更想要“专业可信”还是“更有销售感”的语气？

### For coding | 代码类
- 你希望用什么语言或框架？
- 这是一个最小可用版本，还是希望更工程化一些？
- 需要我直接输出完整代码，还是先给方案？

### For analysis | 分析类
- 你更想看概览结论，还是深入拆解？
- 需要我输出表格、优先级和建议吗？

### For image generation | 图像类
- 你更偏好哪种风格：极简、写实、科技感还是插画感？
- 这张图主要用在什么场景？
- 有没有必须避免的元素或颜色？
