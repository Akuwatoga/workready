# WorkReady

> 面向数据分析新人和职场新人的 AI Skill Stack：先帮 23 岁数据分析应届生把模糊业务需求变成清晰分析计划、进度汇报和试用期证据，再逐步扩展为完整职场新人操作系统。

[English](README.en.md) | [技能索引](docs/skills.md) | [使用说明](docs/usage.md) | [方法论](docs/methodology.md)

## 为什么需要 WorkReady

很多职场新人不是不会努力，而是不知道工作应该如何被组织、表达和交付：

- 老板说“你研究一下”，但不知道要交付什么、做到什么程度。
- 刚入职信息很多，却不知道该问谁、先学什么、如何建立可信度。
- 会议开完只有一堆散乱记录，没有决策、负责人和截止时间。
- 项目推进时责任边界不清，协作对象、决策人、知会对象混在一起。
- 周报和汇报写成“我做了很多事”，但没有结果、风险、决策和下一步。
- 任务散落在聊天、文档、表格和脑子里，无法形成稳定的个人工作系统。

WorkReady 的第一个 wedge 是 **WorkReady Analyst**：当数据分析新人收到“你看一下这个数据为什么不对”这类模糊需求时，先帮他确认业务问题、指标口径、数据源、交付物、时间线和风险，而不是直接埋头取数。

长期目标是把这些模糊职场场景变成可执行的工作流程。用户输入原始信息，AI 按对应 skill 输出可以直接使用的计划、表格、消息、汇报或复盘。

## WorkReady Analyst

第一版优先服务这个具体用户：

> 23 岁大厂数据分析应届生，正在完成 3-6 个月试用期。

核心链路：

```text
/analyst-intake -> /datamap -> /update -> /retro -> /promotion-pack
```

当前主入口是 `/analyst-intake`：

| 输入 | 输出 |
|---|---|
| 模糊业务/数据分析需求 | 需求复述、澄清问题、指标口径风险、数据源风险、启动计划、确认消息 |

## 它能帮你做什么

WorkReady 不只是提示词集合，而是一套面向真实职场场景的工作操作系统：

| 场景 | 你可以调用 | WorkReady 输出 |
|---|---|---|
| 数据分析新人收到模糊需求 | `/analyst-intake` | 需求确认清单、指标口径问题、数据源风险、启动计划、确认消息 |
| 刚入职，不知道怎么上手 | `/onboard` | 第一周计划、角色地图、人员地图、问题清单、给老板的确认消息 |
| 需要通过试用期或实习期 | `/first90` | 30/60/90 天计划、学习议程、早期胜利、风险清单 |
| 老板给了一个模糊任务 | `/plan` | 任务理解、假设、执行步骤、风险依赖、确认消息 |
| 需要向老板汇报进展 | `/update` | 一句话总结、结构化汇报、风险、决策请求、下一步 |
| 开完会需要推进事情 | `/meeting` | 会议摘要、决策、行动项、负责人、截止时间、跟进消息 |
| 项目责任不清 | `/raci` | RACI 责任矩阵、所有权风险、澄清问题 |
| 需要搞清楚关键人和协作关系 | `/stakeholder` | Stakeholder Map、沟通计划、下一轮访谈问题 |
| 项目要做状态汇报 | `/status` | Green/Yellow/Red 状态报告、风险、阻塞、决策建议 |
| 想搭建个人任务系统 | `/tasks` | 任务板、项目清单、日记、决策日志、周复盘循环 |
| 每周复盘或准备 1:1 | `/retro` | 成果证据、经验教训、问题修正、下周前三优先级 |
| 想梳理业务流程和数据源 | `/datamap` | 流程图、数据源表、报表依赖、AI 自动化机会 |
| 不知道消息怎么写得专业 | `/message` | 简洁版、协作版、正式版、推荐发送版本 |

## 为什么选择 WorkReady

### 1. 它关注“职场可信度”，不是泛泛的效率

新人最重要的不是看起来很忙，而是让团队相信你能理解任务、管理风险、及时沟通、稳定交付。WorkReady 的每个 skill 都围绕可信度设计：明确目标、负责人、截止时间、依赖、风险和下一步。

### 2. 它把成熟方法论内置到每次调用里

WorkReady 沉淀了几类经典工作方法：

- **The First 90 Days**：帮助新人理解组织、建立可信度、加速学习、创造早期胜利。
- **Manager Tools / New Job Plan**：帮助用户理解老板、对齐预期、建立沟通节奏。
- **RACI / Stakeholder Mapping / Status Report**：帮助团队协作时明确责任、关键人和项目状态。
- **Obsidian Tasks + Dataview 思路**：把任务、会议、项目、决策和周报沉淀为可查询的个人工作系统。

方法论文件在 [methodologies/](methodologies/)，每个 skill 都会引用对应方法，而不是每次从零开始想。

### 3. 它产出真实工作物，而不是建议

WorkReady 的输出必须是可以继续使用的 artifact：

- 行动计划
- 经理汇报
- 会议纪要和行动项
- RACI 责任矩阵
- Stakeholder Map
- 状态报告
- 任务系统
- 决策日志
- 30/60/90 天计划
- 职场消息草稿
- 业务流程和数据地图

### 4. 它像 gstack 一样按场景调用

gstack 面向软件开发全过程，把 review、QA、ship、retro 等工程场景做成 `/` skill。WorkReady 借鉴这种结构，把新人真实工作中的高频场景做成 `/onboard`、`/plan`、`/update`、`/meeting`、`/raci` 等技能。

### 5. 它有本地记忆，越用越贴合你的工作

WorkReady 不会默认把所有聊天都当成永久记忆。只有写进本地 `memory/` 的结构化内容才是长期记忆，例如：

- 用户岗位和试用期阶段
- 老板偏好的汇报方式
- 常用数据源和指标口径
- 历次分析需求
- 每周复盘和试用期证据

见 [docs/memory.md](docs/memory.md)。

你不需要从空白聊天开始，只要告诉 AI：

```text
/plan

老板让我研究一下为什么周报数据不一致。
我是新入职的数据分析实习生。
数据来自 CRM 导出和一个人工维护的表格。
周五前需要给出初步结论。
```

WorkReady 会输出：

- 对任务的工作解释
- 当前假设和范围外内容
- 分步骤执行计划
- 风险和依赖
- 需要澄清的问题
- 给老板确认范围的消息

## 推荐工作流

### 新人第一周

```text
/onboard -> /stakeholder -> /tasks -> /update -> /retro
```

先建立角色地图和问题清单，再识别关键人，搭建任务系统，每周形成可汇报的证据。

### 模糊任务变成可执行计划

```text
/plan -> /message -> /tasks -> /update
```

先把任务澄清成计划，再写确认消息，落到任务系统，最后持续汇报进展。

### 跨团队项目协作

```text
/stakeholder -> /raci -> /meeting -> /status
```

先知道谁重要，再明确责任边界，把会议变成行动项，并持续更新项目状态。

### 业务流程和 AI 自动化探索

```text
/datamap -> /plan -> /status
```

先画出业务流程、数据源和报表依赖，再把自动化机会拆成可执行计划。

### 数据分析新人接需求

```text
/analyst-intake -> /datamap -> /update -> /retro
```

先确认业务问题、指标口径和数据源，再推进分析、汇报风险，并把完成结果沉淀成试用期证据。

## 项目结构

```text
workready/
  README.md          # 中文默认首页
  README.en.md       # English README
  SKILL.md           # 顶层 WorkReady skill
  WORKREADY.md       # 场景路由器
  commands/          # 简短 slash-command 入口
  skills/            # 可被 Agent 加载的 SKILL.md
  role-packs/        # 面向具体岗位的 skill pack
  methodologies/     # 可复用职场方法论
  templates/         # 任务、会议、周报、RACI、状态报告模板
  memory/            # 本地、显式、可检查的长期记忆
  docs/              # 使用说明和技能索引
  examples/          # 示例工作流
```

## 快速开始

1. 打开 [WORKREADY.md](WORKREADY.md)，根据你的场景选择一个 `/` command。
2. 或直接打开 [skills/](skills/) 中对应的 `SKILL.md`。
3. 把你的原始工作信息粘贴给 AI，并要求它按该 skill 执行。
4. 把输出沉淀到 [templates/](templates/) 对应的工作模板中。

示例：

```text
请使用 /update。

我的原始记录：
- 完成了 CRM 客户字段清理
- 发现 137 条重复记录
- Sales Ops 还没确认合并规则
- 如果今天不确认，周五的 dashboard 可能延迟
```

## 适合谁

- 正在准备入职的学生和应届生
- 刚开始实习的新手
- 刚换团队、换老板、换岗位的人
- 想提高职场沟通和汇报质量的人
- 想把工作流沉淀到 Obsidian/Notion/Markdown 的人
- 想用 AI Agent 辅助日常工作计划和团队协作的人

## 建议 GitHub Topics

为了让更多用户搜索到这个项目，建议给仓库添加这些 topics：

```text
ai-skills
ai-agent
slash-commands
workplace
career
new-grad
internship
onboarding
first-90-days
manager-tools
raci
stakeholder-mapping
status-report
productivity
obsidian
markdown
knowledge-management
workflows
```

仓库 description 建议：

```text
Scenario-driven AI skills for workplace onboarding, planning, collaboration, reporting, and personal work systems.
```

## License

MIT
