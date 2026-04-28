# 高三突围 Skill 集

> 《高三突围》全书蒸馏 · 16 个可即时调用的 RIA++ 可执行技能

[![GitHub](https://img.shields.io/badge/GitHub-Liber1917-green.svg)](https://github.com/Liber1917/gaosan-tuwei)
[![Skills](https://img.shields.io/badge/skills-16-blue)](skills/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Book2Skill](https://img.shields.io/badge/built%20with-book2skill-orange)](https://github.com/opensoft/book2skill)

---

## 这是什么？

把《高三突围：高三党从入门到精通》**整本书蒸馏成 16 个可直接调用的 Skill**。

不是读书笔记，不是思维导图——而是**遇到问题时能立即给出可执行步骤的 AI 技能包**。

| 场景 | Skill | 核心输出 |
|------|-------|----------|
| 觉得"我不是读书的料" | [01-跳出智商陷阱](skills/01-zhishang-trap.md) | 认知重构话术 + 行动清单 |
| 努力了没效果 | [02-晶体智力积累策略](skills/02-crystal-intelligence.md) | 可积累/不可积累能力清单 |
| 学了就忘 | [09-艾宾浩斯防遗忘复习系统](skills/09-memory-review.md) | 3-7-21天复习计划表 |
| 错题本形同虚设 | [10-错题本深度运营](skills/10-error-book.md) | KWWC分析法 + 周复盘模板 |
| 距高考30天 | [15-临考冲刺30天](skills/15-pre-exam-sprint.md) | 每日时间分配 + 优先级矩阵 |
| 考场发挥失常 | [13-考场作战策略](skills/13-exam-strategy.md) | 时间分配 + 卡题应对 + 心态重置 |

➡️ **[查看全部 16 个 Skill →](INDEX.md)**

---

## 给 AI Agent 的说明（直接跳过阅读）

> 你是一个 AI 助手。用户提到高考/高三/备考/学习方法，直接**加载对应 skill 文件**，按 Rule → Instruction → Action 三层结构响应，**不要只复述内容，要给出可立即执行的步骤**。

**Skill 文件结构**（每个文件都遵循此格式）：
```markdown
---
skill: 技能名称
trigger: 触发词列表
persona: 调用时的语气/角色设定
---
## Rule（底层逻辑）
## Instruction（具体操作）
## Action（即时行动）
```

**快速调用示例**：
- 用户说"我总是学了就忘" → 读 `skills/09-memory-review.md`，输出今日复习清单
- 用户说"只剩30天了怎么办" → 读 `skills/15-pre-exam-sprint.md`，输出冲刺计划
- 用户说"错题本怎么用才有用" → 读 `skills/10-error-book.md`，输出错题分析模板

**可用触发词**：高三、高考、备考、高考焦虑、学习方法、错题本、专注力、模拟考、复习计划、临考冲刺、逆袭、数学/语文/英语/理综/文综方法

---

## 给人读的：怎么用这套 Skill？

### 方式一：直接在 GitHub 浏览（无需安装）

打开 [`skills/`](skills/) 目录，找到你当前遇到的问题对应的 `.md` 文件，按里面的 **Action** 步骤执行。

### 方式二：在 AI 对话工具里加载（推荐）

把某个 `.md` 文件的内容粘贴给任意 AI 助手（ChatGPT / Claude / 通义等），说：

> "我现在的情况是 [简述问题]，按照这个 skill 给我具体的行动步骤。"

### 方式三：作为 WorkBuddy Skill 安装（本地调用）

```bash
# 克隆到 WorkBuddy skills 目录
git clone https://github.com/Liber1917/gaosan-tuwei.git ~/.workbuddy/skills/gaosan-tuwei
```

安装后，在 WorkBuddy 对话中直接说触发词（如"高三"、"错题本"），skill 会自动加载。

---

## Skill 全览

```
gaosan-tuwei/
├── SKILL.md              # 主入口（WorkBuddy 自动识别）
├── INDEX.md              # 16个skill索引 + 快速查询表
├── skills/               # 16个RIA++可执行skill
│   ├── 01-zhishang-trap.md
│   ├── 02-crystal-intelligence.md
│   ├── ...
│   └── 16-time-planning.md
└── books/gaosan-tuwei/  # 蒸馏过程产物（可忽略）
    ├── BOOK_OVERVIEW.md
    └── candidates/
```

**16 个 Skill 按篇章分类**：

| 篇章 | Skill | 解决的核心问题 |
|------|-------|--------------|
| **认知重构** | 01 跳出智商陷阱 | 把成绩差归咎于天赋 |
| | 02 晶体智力积累策略 | 不知道在哪里下功夫 |
| | 03 灯泡-电线学习模型 | 理解学习的神经科学本质 |
| | 04 长期思维 | 情绪随考试成绩波动 |
| | 05 只有高考 | 精力被排名/比较占用 |
| | 06 概率思维 | 对高考过度焦虑 |
| **方法论** | 07 30天方法训练术 | 找不到适合自己的方法 |
| | 08 内容鄙视链 | 刷了大量内容没有收获 |
| | 09 防遗忘复习系统 | 学了就忘 |
| | 10 错题本深度运营 | 错题本形同虚设 |
| | 11 三轮复习全攻略 | 不知道每轮复习该做什么 |
| | 12 专注力管理 | 无法集中、手机成瘾 |
| | 16 时间规划自律系统 | 计划落空、拖延 |
| **学科** | 14 各学科方法速查 | 某科不知道怎么学 |
| **临考** | 13 考场作战策略 | 考场时间不够、难题卡壳 |
| | 15 临考冲刺30天 | 最后30天怎么安排 |

---

## 为什么是"AI 原生"的？

传统的学习方法书：你读 → 理解 → 自己转化成行动

这套 Skill 集：**你描述问题 → AI 读 skill → 直接给你执行步骤**

每个 skill 都按 **Rule / Instruction / Action** 三层结构编写：
- **Rule**：理解底层逻辑（为什么要这样做）
- **Instruction**：掌握操作流程（具体怎么做）
- **Action**：现在就做（5分钟内能完成的行动）

---

## 数据声明

本仓库声明如下量化内容，基于书籍原文提炼：
- 全书约 32 万字 / 364 页
- 16 个可执行 skill
- 核心方法论 7 个、学科专项 6 个

> ⚠️ **注意**：以上数据由 AI 从 PDF 中自动提取并蒸馏，未与纸质书逐页核对。引用时建议以原书为准。

---

## 基于什么书？

- 书名：《高三突围：高三党从入门到精通》
- 蒸馏方法：[book2skill](https://github.com/opensoft/book2skill) 工作流
- 蒸馏时间：2026-04-28

---

## 贡献

发现问题？有更好的方法？欢迎提 Issue 或 PR：

1. Fork 本仓库
2. 创建你的分支：`git checkout -b skill/xxx-improvement`
3. 提交改动：`git commit -m '改进：xxx skill 的 Action 步骤'`
4. 推送分支：`git push origin skill/xxx-improvement`
5. 提交 Pull Request

---

## License

[MIT License](LICENSE) — 自由使用、修改、分发。

---

> 💡 **Quote**："高考不是看谁更聪明，而是看谁能把自己训练成一个更可靠的学习系统。" —— 《高三突围》
