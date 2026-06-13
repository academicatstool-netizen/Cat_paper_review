# Known limitations

Honest boundaries build trust. Paper Review is a useful first-pass appraisal, but
it is not magic and it is not a journal. Here is what it is **not**, written down,
so you know exactly what you're getting.

## It is one model role-playing a panel — not a real panel

The "five lenses," "rebuttal round," "moderator," and "chief editor" are **one
model adopting each role in sequence within a single pass**. There are no separate
reviewers, no independent experts, no real deliberation between distinct minds.
The cross-examination is a technique to force more rigorous, self-challenging
output — it genuinely sharpens the result — but it is **not** the independent
multi-reviewer scrutiny of real peer review, and it does not have the diversity of
perspective that several human experts bring.

## It does not replace journal peer review

This skill **assists** your own pre-submission review; it does not substitute for
it. It cannot accept or reject your paper, cannot speak for a journal's specific
scope or house standards, and a single-model pass cannot match a domain expert's
judgement on highly technical methods, niche statistics, or field-specific
conventions. Treat the verdict as a serious reader's opinion, not a gatekeeping
decision.

## The score is heuristic, not a measurement

The 0–10 lens scores and the overall mean are **calibrated heuristics**, not
objective metrics. There is no instrument behind the numbers — they are a
structured judgement expressed numerically to make the verdict legible. Two runs,
or two models, can land a point or two apart. Read the numbers as a band ("this is
a mid-range working draft"), not a precise grade, and weight the **letter** over
the digits.

## It can only assess what you paste in

The review sees **only the text of your draft**. It cannot:

- check whether your citations are real, current, or accurately summarized;
- read the papers you cite or search the literature for work you missed;
- verify your data, re-run your analysis, or confirm your numbers;
- see figures, tables, supplements, or appendices you didn't paste.

So it can flag *"this claim has no citation"* or *"this design can't support a
causal conclusion,"* but it cannot tell you *"a 2023 study already refuted this"*
unless that's in the text. (For literature discovery and reading, that's a
different tool — see [Paper Search](https://github.com/academicatstool-netizen/Cat_paper_search).)

## Stage mis-detection changes the verdict

The verdict thresholds depend on the **draft stage** (final / working / sketch /
student). If the skill guesses the wrong stage — judging a rough sketch as a final
submission, say — the same draft gets a harsher verdict than it deserves, and
vice versa. **State your stage explicitly** ("this is a working draft," "this is a
student essay") so it grades you on the right curve. This is the single most common
way the output goes wrong.

## Type mis-classification mis-applies the standard

The right reporting standard is chosen from the paper type the intake step infers.
If the type is ambiguous or mis-read, the wrong checklist may be applied (e.g.
STROBE criteria pressed onto a paper that's really a theory piece). If your draft
sits between types, say what it is up front.

## Quality varies by model

The skill is pure reasoning, so the quality of the critique tracks the strength of
the model running it. Strong frontier models (Claude Opus/Sonnet, GPT-4-class,
DeepSeek-V3/R1) give the most reliable results; weaker models may miss issues,
mis-calibrate scores, or apply a standard loosely.

---

**Bottom line:** use it as a rigorous, standards-grounded second reader to catch
problems before a human sees them — not as a substitute for the human, the
literature, or your own judgement. For how the method works, see
[METHODOLOGY.md](METHODOLOGY.md); for a worked example, see
[examples/](examples/).
