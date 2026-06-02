<div align="center">

<img src="assets/cover.png" alt="AcademiCats · Paper Review" width="100%">

<br>

# 🐱 Paper Review · 模拟同行评审

**Run your own draft through a six-phase simulated peer-review panel and get back a referee letter plus a scored verdict — calibrated to how finished your draft really is.**

让你的草稿走完六阶段模拟同行评审，得到一封评审意见信 + 评分裁决。**按你的稿件阶段精准校准。**

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-FF7A45.svg)](LICENSE)
&nbsp;[![Runs on Claude](https://img.shields.io/badge/runs%20on-Claude-FF7A45.svg)](https://claude.com/claude-code)
&nbsp;[![Full product](https://img.shields.io/badge/full%20product-academicats.com-FF7A45.svg)](https://academicats.com)

</div>

---

> ### 🪶 This is the **lite, open-source edition** of [**AcademiCats**](https://academicats.com)
> The full product at **[academicats.com](https://academicats.com)** is an AI research workbench that takes you from *finding* papers through *reading, writing, and self-review*. This skill is a free, self-contained slice of the review workflow you can run on your own Claude.
>
> 这是 [**AcademiCats**](https://academicats.com) 的**开源轻量版**。完整产品在 **academicats.com**——一个从找文献到读、写、自审的 AI 研究工作台。

---

## ✨ What it does

🧪 **A whole panel, not one opinion** — five specialist reviewers (structure, argument, evidence, language, originality) each critique from their own lens, then **argue with each other** in a rebuttal round before a moderator reconciles them. That cross-examination is what kills plausible-but-wrong feedback and sharpens what's real.

📊 **A verdict with a number** — you get a referee letter (verdict, strengths, issues to fix, optional improvements) *and* a scorecard: each dimension scored 0–10, an overall, and a recommendation — **Accept / Minor / Major Revision / Reject**.

🎚️ **Calibrated to your stage** — tell it whether it's a *final*, *working*, *sketch*, or *student* draft, and it won't judge a class essay like a journal submission.

<br>

## 🎬 Demo

> *"Peer-review my draft — it's a working draft of a short research proposal. Is it ready?"*

A real excerpt of the letter it returns:

> **# Verdict**
> This is a short proposal asking a real and relevant question — does background music affect coding productivity — with the correct two-group design instinct and clean prose. As a working draft it is a promising skeleton rather than a viable plan, and the single most important thing to fix is the outcome measure: the study currently rests on *lines of code per hour*, a discredited productivity proxy that would invalidate the result no matter how the experiment runs.
>
> **# Issues to Fix**
> **Replace the sole productivity metric.** "How many lines of code they write in one hour" rewards verbosity and ignores correctness… add a validated outcome (task completion, tests passed, time-on-task).
> **Ground the proposal in prior work.** There are no citations anywhere… add a short related-work paragraph with 3–5 references.

…followed by a scorecard:

| Structure | Argument | Evidence | Language | Originality | **Overall** | **Verdict** |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 6 | 4 | 3 | 6 | 5 | **4.8 / 10** | **Major Revision** |

<br>

## 🚀 Get started in 60 seconds

```bash
# drop this skill where Claude Code can find it — no dependencies, no setup
cp -r Cat_paper_review ~/.claude/skills/paper-review
```

Then just talk to Claude: *"review my draft, it's a working draft of a research proposal …"* or *"peer-review this essay as a final submission — is it ready?"* The skill triggers itself and runs entirely on your own Claude.

<br>

## 💙 What's inside

Six phases — **intake → 5 specialists → rebuttal round → moderator → editor letter → scorecard** — distilled from the same panel that powers the full product.

|  | Paper Review (this skill) | [AcademiCats full product →](https://academicats.com) |
|---|:---:|:---:|
| Six-phase panel + scored verdict | ✅ | ✅ |
| Stage-aware calibration | ✅ | ✅ |
| Find & read the literature it asks for | bring your own | ✅ end-to-end |
| Saved drafts & revision history | — | ✅ |
| Polished web & mobile app | — | ✅ |

<div align="center">
<br>

### Want the whole research workflow?
**→ [academicats.com](https://academicats.com) ←**

<br>

Made with 💙 by the [AcademiCats](https://academicats.com) team · [MIT License](LICENSE)

</div>
