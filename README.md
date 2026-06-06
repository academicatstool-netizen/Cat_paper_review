<div align="center">

**English** · [中文](README.zh-CN.md)

<img src="assets/cover.png" alt="AcademiCats · Paper Review" width="100%">

<br>

# 🐱 Paper Review

**Run your own draft through a six-phase simulated peer-review panel and get back a referee letter plus a scored verdict — calibrated to how finished your draft really is.**

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-FF7A45.svg)](LICENSE)
&nbsp;[![Runs on Claude](https://img.shields.io/badge/runs%20on-Claude-FF7A45.svg)](https://claude.com/claude-code)
&nbsp;[![Full product](https://img.shields.io/badge/full%20product-academicats.com-FF7A45.svg)](https://academicats.com)

</div>

---

> ### 🪶 This is the **lite, open-source edition** of [**AcademiCats**](https://academicats.com) — now in free open beta
> The full product at **[academicats.com](https://academicats.com)** is an AI research workbench that takes you from *finding* papers through *reading, writing, and self-review*. This skill is a free, self-contained slice of the review workflow you can run on your own Claude.

---

## ✨ What it does

🧪 **A whole panel's scrutiny, from one model** — your draft is examined through five independent review lenses (structure, argument, evidence, language, originality) that then **challenge each other** in a rebuttal round before a moderator reconciles them. That cross-examination is what kills plausible-but-wrong feedback and sharpens what's real.

📊 **A verdict with a number** — you get a referee letter (verdict, strengths, issues to fix, optional improvements) *and* a scorecard: each dimension scored 0–10, an overall, and a recommendation — **Accept / Minor / Major Revision / Reject**.

🎚️ **Calibrated to your stage** — tell it whether it's a *final*, *working*, *sketch*, or *student* draft, and it won't judge a class essay like a journal submission.

<br>

## 🎬 Demo

> *"Peer-review my draft — it's a working draft of a short research proposal. Is it ready?"*

You said it's a working draft — so it reviews straight away (no forms; it notes the stage it used so you can correct it). The result is **always the same shape** — a referee letter, a scorecard, then a one-line summary — no matter which model runs the skill:

> # Verdict
> A clear, relevant proposal — but as a working draft it's a promising skeleton, not yet a viable plan. The key fix: it rests on *lines of code per hour*, a discredited productivity proxy that would invalidate the result no matter how the experiment runs.
>
> # Strengths
> - The two-group design is the right shape for the question.
> - Clear, readable prose.
>
> # Issues to Fix
> **Replace the sole metric** — lines-of-code rewards verbosity and ignores correctness; add a validated outcome (task completion, tests passed, time-on-task).
> **Ground it in prior work** — there are no citations anywhere; add a short related-work paragraph.

| Structure | Argument | Evidence | Language | Originality | Overall | Verdict |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 6 | 4 | 3 | 6 | 5 | **4.8/10** | **Major Revision** |

> *A relevant question undermined by a confirmation-seeking design; not ready until the metric and controls are fixed.*

<br>

## 🚀 Get started in 60 seconds

```bash
# install into Claude Code's skills folder — no dependencies, no setup
mkdir -p ~/.claude/skills
git clone https://github.com/jy1529098645-gif/Cat_paper_review.git ~/.claude/skills/paper-review
```

Restart Claude Code, then just talk to it — *"review my draft, it's a working draft of a research proposal …"* or *"peer-review this essay as a final submission — is it ready?"* The skill triggers itself and runs entirely on your own Claude.

**On Claude web or desktop instead?** Download **[`paper-review.skill`](paper-review.skill)** and upload it under **Settings → Capabilities → Skills** — then just ask in any chat.

<br>

## 💙 What's inside

Six phases — **intake → 5 lenses → rebuttal round → moderator → editor letter → scorecard** — distilled from the same review method behind the full product.

|  | Paper Review (this skill) | [AcademiCats full product →](https://academicats.com) |
|---|:---:|:---:|
| ⚡ **Speed** | minutes (one Claude pass) | faster — streamed, parallel panel |
| Six-phase panel + scored verdict | ✅ | ✅ |
| Stage-aware calibration | ✅ | ✅ |
| Find & read the literature it asks for | bring your own | ✅ end-to-end |
| Saved drafts & revision history | — | ✅ |
| Polished web & mobile app | — | ✅ |

## 🐱 The AcademiCats skill family

Three open skills that chain into one research workflow — install any or all:

- 🔍 [Paper Search](https://github.com/jy1529098645-gif/Cat_paper_search) — find & read papers
- ✍️ [Synthesis Lab](https://github.com/jy1529098645-gif/Cat_synthesis_lab) — write grounded papers from your sources
- 🧪 **Paper Review** *(you are here)* — peer-review your own draft

**Install all three at once** — clone any one repo, then run `bash install.sh`.

## 🙋 FAQ

- **It didn't trigger?** Restart Claude Code after installing, and phrase your message as a task — *"review my draft …"*.
- **Tell it the draft stage.** Say it's a *"working draft"*, *"final"*, *"rough sketch"*, or *"student essay"* so it grades you fairly — a class essay shouldn't be judged like a journal submission.
- **Which model?** Any model works; quality is best on Claude Sonnet or above.
- **Private & free?** It runs on your own Claude — no account, nothing sent to us.

<div align="center">
<br>

### Want the whole research workflow?
**→ [academicats.com](https://academicats.com) ←**

*🚀 The full product is in **open beta** — free to try right now.*

<br>

Made with 💙 by the [AcademiCats](https://academicats.com) team · [MIT License](LICENSE)

</div>
