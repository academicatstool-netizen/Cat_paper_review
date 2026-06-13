# Generic AI vs. Paper Review

Feedback you can't trust is just flattery. The fastest way to see the difference
is to run **the same flawed draft** past a generic chatbot and past this skill.

Below is one draft with a **fatal flaw**, reviewed both ways.

---

## The draft under review

> **Title:** *Screen Time Causes Anxiety in Adolescents*
>
> **Abstract.** We surveyed 500 teenagers (ages 13–17) through an online
> questionnaire. Respondents reported their average daily screen time and
> completed a self-rated anxiety scale. Teens with higher screen time reported
> higher anxiety. **We conclude that screen time causes anxiety in adolescents**
> and that limiting device use will reduce teenage anxiety.
>
> **Methods.** Participants were recruited via social media. All measures
> (screen time, anxiety) were self-reported in a single sitting. No other
> variables were collected.

This is a **cross-sectional online survey** — it measures everything at one
moment, with no comparison condition and no control for anything else going on in
a teenager's life. The headline claim is **causal** ("screen time *causes*
anxiety"). That gap — a correlational design carrying a causal conclusion — is
the methodology-killer. A good reviewer's whole job is to catch it.

---

## Column A — What a generic chatbot often does

> ### ⚠️ ILLUSTRATIVE — the failure mode
> *This is a fabricated example of typical generic-chatbot output, included to
> show the failure mode: flattering, generic, and it misses the
> methodology-killer entirely. It is **not** real Paper Review output.*

> **Great work on this study!** 🎉 This is a clear and well-written paper on a
> really interesting and timely topic — screen time and teen mental health is
> something everyone cares about. Your abstract is easy to follow and your
> conclusion is stated confidently.
>
> A few minor suggestions: tighten up a little grammar in the methods section,
> and maybe add a sentence to the intro about why this matters.
>
> **Overall: 8/10.** Nice job — just polish the writing and you're good to go!

Notice what happened: it praised the topic, rewarded confident phrasing, suggested
**grammar fixes**, and handed out an **8/10** — while the central claim of the
paper is **invalid**. A correlation from a one-shot self-report survey cannot
support "X causes Y." The reader walks away reassured and wrong.

---

## Column B — What Paper Review does

Running the real method (`references/review.md`): the intake editor classifies the
draft as **`observational`**, so the Rigor lens applies **STROBE** — the reporting
standard for observational studies. The five lenses then flag the real problems,
challenge each other in the rebuttal round, and the verdict is calibrated to the
stated draft stage (here: a *working draft*).

> # Verdict
> This is a clearly written study on a relevant question, but as an observational
> design it cannot support its central claim. Appraised against **STROBE**, the
> single fatal issue is causal overreach: a cross-sectional, self-reported survey
> measures *association*, not causation, and the paper concludes "screen time
> **causes** anxiety" and recommends an intervention on that basis. Until the
> claim is rewritten to match the design — or the design is changed — the
> conclusion is invalid no matter how clean the prose is.
>
> # Strengths
> - The research question is timely and clearly motivated.
> - The abstract and methods are easy to follow.
> - The exposure/outcome relationship is stated plainly enough to test.
>
> # Issues to Fix
> **Causal claim from associational data** — the design is cross-sectional, yet
> the paper states screen time *"causes"* anxiety and that limiting devices
> *"will reduce"* it. Rewrite every causal/interventional claim as association
> ("is associated with"), or move to a design that can support causation
> (longitudinal/experimental). *(STROBE: no causal language from observational
> data.)*
> **No confounder control** — "No other variables were collected," so known
> drivers of both screen time and anxiety (sleep, bullying, family stress,
> baseline mental health, socioeconomic status) are uncontrolled. Identify and
> measure plausible confounders and adjust for them; report what could not be
> controlled. *(STROBE: confounders identified and addressed.)*
> **Self-report + single-sitting measurement** — both exposure and outcome are
> self-rated in one session, inviting recall and common-method bias and reverse
> causation (anxious teens may report more screen time). Use validated
> instruments, separate the measurements, and discuss measurement bias.
> **Selection bias from social-media recruitment** — a self-selected online
> sample is not representative of adolescents and over-samples heavy device
> users. State the sampling frame and discuss generalizability limits. *(STROBE:
> selection of participants, generalizability.)*
>
> ## Scorecard
>
> | Significance | Rigor | Evidence | Argument | Clarity | Overall | Verdict |
> |:--:|:--:|:--:|:--:|:--:|:--:|:--:|
> | 6/10 | 2/10 | 3/10 | 4/10 | 7/10 | **4.4/10** | **Major Revision** |
>
> *A relevant question undermined by a correlational design making a causal claim; not ready until the claim matches the design.*
>
> *Appraised as an **observational study** against **STROBE** · 5 lenses (significance · rigor · evidence · argument · clarity), cross-checked against each other — ask to see the full panel.*

---

## The difference

Column A rewards confidence and polish and gives a high number. Column B applies a
**real, published reporting standard** —
[STROBE (Strengthening the Reporting of Observational Studies in Epidemiology)](https://www.equator-network.org/reporting-guidelines/strobe/),
hosted by the EQUATOR Network — plus a rubric calibrated to the draft stage, and
catches the flaw that invalidates the paper.

One gives you vibes. The other gives you a critique you can act on, traceable to a
standard you can look up. That is the point of the trust pack — see
[METHODOLOGY.md](../METHODOLOGY.md) for how the review works and
[LIMITATIONS.md](../LIMITATIONS.md) for what it can and can't do.
