<div align="center">

[English](README.md) · **中文**

<img src="assets/cover.png" alt="AcademiCats · Paper Review" width="100%">

<br>

# 🐱 Paper Review · 模拟同行评审

**让你自己的草稿走完六阶段模拟同行评审，得到一封评审意见信 + 一份评分裁决 —— 并按你的稿件实际完成度精准校准。**

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-FF7A45.svg)](LICENSE)
&nbsp;[![Runs on Claude](https://img.shields.io/badge/运行于-Claude-FF7A45.svg)](https://claude.com/claude-code)
&nbsp;[![Full product](https://img.shields.io/badge/完整产品-academicats.com-FF7A45.svg)](https://academicats.com)

</div>

---

> ### 🪶 这是 [**AcademiCats**](https://academicats.com) 的**开源轻量版**
> 完整产品在 **[academicats.com](https://academicats.com)** —— 一个 AI 研究工作台，带你从*找文献*一路走到*读、写、自审*。本 skill 是其中评审工作流的一块免费、自包含、可在你自己的 Claude 上运行的切片。

---

## ✨ 它能做什么

🧪 **一整个评审团，而非一家之言** —— 五位专家评审（结构、论证、证据、语言、原创性）各从自己的视角批评，再在**反驳轮**里互相辩论，最后由仲裁者统合。正是这种交叉质询，淘汰掉"看似有理实则错误"的意见，并把真正的问题打磨锋利。

📊 **带数字的裁决** —— 你会拿到一封评审信（裁决、优点、待修问题、可选改进）*以及*一份评分卡：每个维度 0–10 分、一个总分、一条建议 —— **接受 / 小修 / 大修 / 拒稿**。

🎚️ **按阶段校准** —— 告诉它这是*终稿、在写稿、草图*还是*学生作业*，它就不会拿期刊投稿的标准去苛求一篇课程论文。

<br>

## 🎬 演示

> *"帮我审一下这份草稿 —— 是一份在写的短研究计划。能投了吗？"*

它返回的评审信真实节选：

> **# Verdict（裁决）**
> This is a short proposal asking a real and relevant question — does background music affect coding productivity — with the correct two-group design instinct and clean prose. As a working draft it is a promising skeleton rather than a viable plan, and the single most important thing to fix is the outcome measure: the study currently rests on *lines of code per hour*, a discredited productivity proxy that would invalidate the result no matter how the experiment runs.
>
> **# Issues to Fix（待修问题）**
> **Replace the sole productivity metric.** "每小时写多少行代码"奖励冗长、忽视正确性…… 增加一个有效指标（任务完成度、测试通过数、用时）。
> **Ground the proposal in prior work.** 全文没有任何引用…… 增加一段 3–5 篇参考文献的相关工作。

……随后附上一份评分卡：

| 结构 | 论证 | 证据 | 语言 | 原创性 | **总分** | **裁决** |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 6 | 4 | 3 | 6 | 5 | **4.8 / 10** | **大修（Major Revision）** |

<br>

## 🚀 60 秒上手

```bash
# 把 skill 放到 Claude Code 能发现的位置 —— 无依赖、零配置
cp -r Cat_paper_review ~/.claude/skills/paper-review
```

然后直接跟 Claude 说：*"帮我审这份草稿，是一份在写的研究计划…"* 或 *"把这篇 essay 当最终稿来同行评审 —— 能投了吗？"* skill 会**自动触发**，全程跑在你自己的 Claude 上。

<br>

## 💙 内部构造

六个阶段 —— **接收 → 5 位专家 → 反驳轮 → 仲裁 → 主编信 → 评分卡** —— 提炼自驱动完整产品的同一套评审团。

|  | Paper Review（本 skill） | [AcademiCats 完整产品 →](https://academicats.com) |
|---|:---:|:---:|
| 六阶段评审团 + 评分裁决 | ✅ | ✅ |
| 按稿件阶段校准 | ✅ | ✅ |
| 自动找并读它需要的文献 | 自备文献 | ✅ 端到端 |
| 草稿保存与修订历史 | — | ✅ |
| 精致的网页与移动端 | — | ✅ |

<div align="center">
<br>

### 想要完整的研究工作流？
**→ [academicats.com](https://academicats.com) ←**

<br>

由 [AcademiCats](https://academicats.com) 团队用 💙 打造 · [MIT 许可证](LICENSE)

</div>
