# My Interview Answer

> **会做事的人，值得一个会说话的答案。**

**一道题 → 一个有结论、有细节、能直接开口练的回答。**

一个面向中文面试的 Agent Skill。给它一道题，它会按「接题 → 结论 → 分点展开 → 收束」组织成口语逐字稿：有观点、有例子、有具体做法，也给人留出真实说话的呼吸感。

**适合谁：**想练习面试表达、打磨回答结构，或者需要快速准备多道面试题的人。

## 它能帮你做什么

- **先把答案立起来。** 开头接住问题，先说结论，再逐点展开，最后回到岗位或具体行动。
- **把空话压下去。** 每个判断尽量跟上例子、操作步骤、工具选择或影响因素。
- **让稿子说得出口。** 保留自然的中文口语节奏，避免把一段书面报告塞进面试现场。
- **按题型换结构。** 自我介绍、流程题、解决问题题、观点题、数字成本题、开放方案题、事实题、个人情况题和反问，都有对应的回答思路。
- **守住真实边界。** 个人经历、作品、数据和薪资只取自你本次提供的材料；缺少必要信息时，用 `【待补：需要什么】` 标记。

它是一套**回答方法**，也是一份**可直接开口练习的初稿**。你负责提供真实经历，AI 负责帮你把话组织清楚。

## 一眼看懂它的变化

问：「你怎么用 AI 提效工作？」

> **松散回答：**“我会用 AI 写文案、查资料，也会用它提高工作效率。”

> **结构化回答片段：**“我会把 AI 放进完整的工作流程里，主要分三步。第一步是整理信息，先把资料和待确认的问题梳理清楚；第二步是做初稿，但事实和判断要由我来核对；第三步是复盘，把有效的做法整理成下次还能用的流程。”

这里展示的是表达方式的差别；真正涉及你的项目、工具和结果时，请补充自己的材料，让答案有你的证据。

## 30 秒上手

在支持 Agent Skills 的工具里安装后，直接提问：

```text
使用 my-interview-answer，帮我回答：你是如何使用 AI 提效整个工作流程的？
```

如果题目涉及你的亲身经历，建议一起给出可验证的材料：

```text
使用 my-interview-answer，帮我回答：你做过最有挑战的一次项目是什么？
材料：项目目标是……；我负责……；遇到的困难是……；最后结果是……。
控制在 1 分钟左右，只用我给出的事实。
```

你也可以一次给多道题。Skill 会为每道题分别写出可练习的回答。

## 安装

### 共用目录：Codex、Cursor、Copilot CLI、Kimi Code、Gemini CLI

这些工具支持从用户级 `~/.agents/skills/` 发现 Skill。macOS / Linux 可以执行：

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/realruian/my-interview-answer.git ~/.agents/skills/my-interview-answer
```

如果不使用 Git，也可以下载本仓库的 ZIP，解压后将文件夹放到 `~/.agents/skills/my-interview-answer/`。确认里面直接包含 `SKILL.md`。

### Claude Code

Claude Code 的个人 Skill 目录是 `~/.claude/skills/`。已经按上一步安装的，可以链接同一份文件：

```bash
mkdir -p ~/.claude/skills
ln -s ~/.agents/skills/my-interview-answer ~/.claude/skills/my-interview-answer
```

也可以直接把仓库克隆或解压到 `~/.claude/skills/my-interview-answer/`。

其他支持 `SKILL.md` 的工具，可将整个 `my-interview-answer` 文件夹放到该工具的个人 Skill 目录。网页端和云端产品通常不会自动读取你电脑上的文件，需要在对应产品内单独导入。

目录结构应为：

```text
my-interview-answer/
├── SKILL.md      # Skill 本体
└── README.md     # 你正在读的使用说明
```

> 不同产品的发现路径和刷新方式可能随版本变化。安装后，先在产品的 Skill 列表里确认 `my-interview-answer` 已出现；已有会话看不到时，刷新 Skill 列表或开启新会话。

## 这份 Skill 的回答风格

它偏向**有结论、能举例、讲得具体、听起来像真人**的表达。开放题通常会写成约 1～2 分钟的逐字稿；事实题会短答；自我介绍会控制在约 1 分钟。回答可以直接练，但最好再按自己的语速、经历和目标岗位调整一遍。

**使用前请留意：**Skill 不会替你验证个人事实，也不能凭空补齐经历。看到 `【待补：……】`，请用自己的真实信息替换。面试时涉及外部数据、平台规则或行业动态，也请核对其时效性。

## 设计思路

这个 Skill 把一套面试表达习惯压缩进一个文件：

1. **总分总**：让面试官先听到判断，再听到支撑。
2. **判断后接例子**：让观点落到动作、工具、原因和结果。
3. **按题型组织**：流程题讲步骤，观点题讲依据，个人情况题简短直接。
4. **口语化收尾**：收回结论，落到“我能做什么”。

它的目标很简单：**把“我知道怎么做”变成“我能清楚地说出来”。**

## 官方路径参考

- [Cursor Skills](https://prod.cursor.com/help/customization/skills)
- [GitHub Copilot CLI Skills](https://docs.github.com/en/copilot/how-tos/copilot-cli/customize-copilot/add-skills)
- [Kimi Code Agent Skills](https://www.kimi.com/code/docs/kimi-code-cli/customization/skills.html)
- [Gemini CLI Agent Skills](https://geminicli.com/docs/cli/using-agent-skills/)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)

---

**作者：田睿安** · 欢迎下载试用，也欢迎带着真实面试题反馈使用体验。
