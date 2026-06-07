<div align="center">

[English](README.md) · **中文**

<img src="assets/cover-zh.png" alt="AcademiCats · Paper Review" width="100%">

<br>

# 🐱 模拟同行评审

**让你自己的草稿走完六阶段模拟同行评审，得到一封评审意见信 + 一份评分裁决 —— 并按你的稿件实际完成度精准校准。**

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-FF7A45.svg)](LICENSE)
&nbsp;[![Claude](https://img.shields.io/badge/Claude-FF7A45.svg)](https://claude.com/claude-code)
&nbsp;[![ChatGPT](https://img.shields.io/badge/ChatGPT-FF7A45.svg)](https://chatgpt.com)
&nbsp;[![DeepSeek](https://img.shields.io/badge/DeepSeek-FF7A45.svg)](https://chat.deepseek.com)
&nbsp;[![Full product](https://img.shields.io/badge/完整产品-academicats.com-FF7A45.svg)](https://academicats.com)

</div>

---

> ### 🪶 这是 [**AcademiCats**](https://academicats.com) 的**开源轻量版**（正式版现处公测，免费试用）
> 完整产品在 **[academicats.com](https://academicats.com)** —— 一个 AI 研究工作台，带你从*找文献*一路走到*读、写、自审*。本 skill 把其中的评审部分免费开源，自包含、可直接在你自己的 AI 上运行——Claude、ChatGPT 或 DeepSeek 皆可。

---

## ✨ 它能做什么

🧪 **一整个评审团的审视，由单个模型完成** —— 它用五种独立的评审视角（重要性、严谨性、证据、论证、清晰度）逐一审你的草稿，再在**反驳轮**里让这些视角**相互质询**，最后由仲裁统合。正是这种交叉质询，筛掉"看似有理、实则站不住"的意见，让真正重要的问题更突出。

🔬 **用对的标准来评** —— 方法学评审会**按你实际写的论文类型**切换尺子：观察性研究对照 **STROBE**、系统综述对照 **PRISMA + AMSTAR-2**、随机对照试验对照 **CONSORT**、质性研究对照 **COREQ**、研究计划对照 **NIH** 准则、论说文对照 **Toulmin** 论证模型 —— 而不是一把通用清单量到底。

📊 **带数字的裁决** —— 你会拿到一封评审信（裁决、优点、待修问题、可选改进）*以及*一份评分卡：每个维度 0–10 分、一个总分、一条建议 —— **接受 / 小修 / 大修 / 拒稿**。

🎚️ **按阶段校准** —— 告诉它这是*终稿、在写稿、草图*还是*学生作业*，它就不会拿期刊投稿的标准去苛求一篇课程论文。

<br>

## 🎬 演示

> *"帮我审一下这份草稿 —— 是一份在写的短研究计划。能投了吗？"*

你说了是"在写的草稿"——它就**直接开审**（不用填表，只标一下采用的稿件阶段，方便你纠正）。返回的成品**永远是同一种结构**——评审信、评分卡、一句话总结——换任何大模型跑都一样：

> # 裁决
> 这是一份针对真实且有价值问题的短计划——背景音乐是否影响编程效率——有正确的两组对照设计直觉、文笔清晰。但作为在写稿，它还只是个有潜力的骨架而非可行方案；最关键的一处是结果度量：研究依赖*每小时代码行数*，这是一个早已被学界否定的生产力衡量指标，无论实验怎么跑，结论都站不住。
>
> # 优点
> - 两组对照设计的方向是对的。
> - 文笔清晰易读。
>
> # 待修问题
> **替换唯一的指标** —— "每小时写多少行代码"奖励冗长、忽视正确性；改用有效指标（任务完成度、测试通过数、用时）。
> **补上既有研究** —— 全文无任何引用；加一段相关工作。

| 重要性 | 严谨性 | 证据 | 论证 | 清晰度 | 总分 | 裁决 |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 6 | 3 | 3 | 6 | 6 | **4.8/10** | **大修** |

> *一个有价值的问题，却被"只想证实"的设计拖累；在修好指标与对照之前还不能投。*
> *按研究计划对照 NIH 准则评审（重要性 · 创新性 · 方案）· 五视角交叉核对。*

<br>

## 🚀 开始使用 —— 按你的平台选一种

按你常用的 AI 选一种，每种不到一分钟：

**🖥️ Claude Code** —— 本地运行、自动触发
```bash
mkdir -p ~/.claude/skills
git clone https://github.com/jy1529098645-gif/Cat_paper_review.git ~/.claude/skills/paper-review
```
重启 Claude Code，然后直接说 —— *"帮我审这份草稿，是一份在写的研究计划…"*

**🌐 Claude 网页 / 桌面版** —— 下载 **[`paper-review.skill`](paper-review.skill)**，在 **Settings → Capabilities → Skills** 里上传，然后任意对话直接问。

**🤖 ChatGPT** —— 打开 **[`PORTABLE_PROMPT.md`](PORTABLE_PROMPT.md)**，贴进**自定义 GPT** 的 *Instructions*（或作为第一条消息发送），然后把草稿贴给它。

**💬 DeepSeek / 任意其他模型** —— 把 **[`PORTABLE_PROMPT.md`](PORTABLE_PROMPT.md)** 作为**系统提示**（或第一条消息）粘贴，然后把草稿贴给它。

> ✅ **无需联网** —— 模拟同行评审是纯推理，任何模型上都能完整运行（在线离线都行）。它只评审你粘贴的草稿，不需要联网查任何东西。

<br>

## 💙 内部构造

六个阶段 —— **接收 → 5 个评审视角 → 反驳轮 → 仲裁 → 主编信 → 评分卡** —— 与正式版背后是同一套评审方法。

|  | 模拟同行评审（本 skill） | [AcademiCats 完整产品 →](https://academicats.com) |
|---|:---:|:---:|
| ⚡ **速度** | 几分钟（单个模型一遍生成） | 更快 —— 流式 + 并行评审团 |
| 六阶段评审团 + 评分裁决 | ✅ | ✅ |
| 按论文类型挂标准（STROBE / PRISMA / CONSORT / COREQ / Toulmin） | ✅ | ✅ |
| 按稿件阶段校准 | ✅ | ✅ |
| 自动找并读它需要的文献 | 自备文献 | ✅ 端到端 |
| 草稿保存与修订历史 | — | ✅ |
| 精致的网页与移动端 | — | ✅ |

## 🐱 AcademiCats 技能家族

三个开源 skill，串起一条完整的研究工作流——按需安装其一或全部：

- 🔍 [论文检索](https://github.com/jy1529098645-gif/Cat_paper_search) —— 找文献、读文献
- ✍️ [文献写作台](https://github.com/jy1529098645-gif/Cat_synthesis_lab) —— 用你的文献写出有据可查的成稿
- 🧪 **模拟同行评审** *（你在这里）* —— 对你自己的草稿做同行评审

**一次装齐三个** —— clone 任意一个仓库后运行 `bash install.sh`。

## 🙋 常见问题

- **这些文件都是干嘛的？** 上面几种方式用其一即可——git clone（Claude Code）、`.skill` 文件（Claude 网页/桌面）、或 `PORTABLE_PROMPT.md`（ChatGPT/DeepSeek）。`SKILL.md`、`references/` 是助手自动加载的内部文件，无需手动打开。
- **没触发？** 安装后重启 Claude Code，并把话说成一个任务 —— *"帮我审这份草稿…"*。
- **记得说明稿件阶段。** 告诉它是*"在写稿"、"终稿"、"草图"*还是*"学生作业"*，它才会公平打分——课程作业不该用期刊投稿的标准来评。
- **用哪个模型？** 任何够强的模型都行——Claude Sonnet/Opus、GPT‑4o/o 系列、DeepSeek‑V3/R1 效果最好。
- **隐私 & 免费？** 全程跑在你自己的 AI 上——无需账号、不向我们回传任何东西。

<div align="center">
<br>

### 想要完整的研究工作流？
**→ [academicats.com](https://academicats.com) ←**

*🚀 正式版现处**公测阶段** —— 现在免费试用。*

<br>

由 [AcademiCats](https://academicats.com) 团队用 💙 打造 · [MIT 许可证](LICENSE)

</div>
