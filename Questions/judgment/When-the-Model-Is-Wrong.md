# When the Model Is Wrong

> Tell me about a time an AI feature you shipped produced a wrong, weird, or harmful output. How did you find out, and what did you measure to know if it was actually a systemic problem versus a one-off?

> **Follow-up** What would you evaluate before shipping the next version that you didn't evaluate before this one?

## Type

Judgment

## Competencies Assessed

- Metrics, Outcomes, And Learning

## AI Competency

[AI Evaluation & Metrics](../../docs/ai-competency-model.md#ai-evaluation--metrics)

## Why This Matters

Only use this card for roles where AI is a real part of the product surface — see [ai-competency-model.md](../../docs/ai-competency-model.md). AI systems will produce bad outputs; the real differentiator is whether a PM has a real way of distinguishing an isolated bad output from a systemic quality problem, and a real evaluation practice rather than "we'll know it when we see it."

## Neutral Follow-Up Probes

- How did you actually find out — a user report, monitoring, an internal eval?
- What did "systemic" versus "one-off" actually look like in the data?
- Who decided what to do about it, and what did you do?

## Strong Evidence

1. Describes a specific real bad output and how it was discovered — ideally through some form of monitoring or evaluation, not purely luck or a user complaint.
2. Describes a real method for distinguishing a systemic issue from an isolated one — a rate, a pattern across inputs, a category of failure — not just gut feel.
3. Describes what was actually done in response — a fix, a guardrail, a scope reduction — with a real outcome.
4. In the follow-up, names a specific evaluation added for future versions, showing the incident changed practice.

## Warning Signs

1. No real method for distinguishing systemic from one-off — treats every bad output the same way.
2. Discovery was purely accidental with no monitoring or evaluation practice in place at all.
3. No real change to future evaluation practice as a result.

## Scoring Anchors

- **5:** Specific real incident, a genuine systemic-vs-one-off method, a concrete response, and a real change to evaluation practice going forward.
- **3:** A real incident exists but the systemic/one-off distinction or the practice change is thin.
- **1:** No real incident, or no evaluation practice of any kind.

## Attributions

* Adapted from [`Research/AI Product Management Assessment.md`](../../Research/AI%20Product%20Management%20Assessment.md), an internal framework contributed to this project — see [ai-competency-model.md](../../docs/ai-competency-model.md) for how it maps to this card.

## Additional Reading

* (None yet — contributions welcome.)
