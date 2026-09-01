# Evidence And Pressure Standard

## Purpose

A shared vocabulary for what counts as evidence in an answer, and a lightweight way to record a specific concern about that evidence — so "strong evidence" and "warning signs" mean the same thing across every card, not just whatever each card's author happened to write. Pairs with [scoring-rubric.md](scoring-rubric.md) (how to turn evidence into a score) and [structured-interview-guide.md](structured-interview-guide.md) (how to run the conversation that surfaces it).

This is adapted from the evidence-grading and pressure-testing approach used in adversarial product-review practice (the kind of rigor applied to a roadmap or business case before it goes in front of an executive), translated here for interview evidence rather than document review.

## The Evidence Ladder

When a candidate makes a claim, place it on this ladder. Higher rungs are stronger evidence; a strong answer moves up the ladder as you probe, a weak one stays at the bottom no matter how confidently it's delivered.

1. **Aspiration** — a stated goal or hope with nothing behind it yet ("we wanted it to reduce churn").
2. **Assumption** — an unstated belief the candidate is relying on, often revealed only by asking "what were you assuming?"
3. **Hypothesis** — an assumption the candidate has explicitly named as something to test, rather than treated as given.
4. **Estimate** — a number derived from reasoning or partial data, not directly measured.
5. **Forecast** — a stated prediction of a future result, distinct from a report of what already happened.
6. **Reported statement** — something the candidate was told by someone else (a stakeholder, a customer, a dashboard someone else built) but didn't verify directly.
7. **Interpretation** — the candidate's own reading of directly observed information, where a different reasonable person might read it differently.
8. **Observed fact** — something the candidate directly saw, measured, or did, with little room for a different reading.
9. **Commitment** — a decision or action the candidate actually took, not merely considered.

A candidate who says "the metric improved" (a claim) versus "I pulled the dashboard myself and it moved from 12% to 18% over three weeks after the change shipped" (observed fact, with the reasoning to interpretation shown) are giving you very different evidence, even if both sound confident.

## Using The Ladder While Interviewing

- **Ask which rung a claim is on.** "How do you know that?" and "Did you see that yourself, or did someone tell you?" are the two questions that do most of the work.
- **Don't penalize a candidate for starting low on the ladder.** An assumption or hypothesis, named as such, is honest and often correct at that stage of a project. What matters is whether the candidate *knows* which rung they're on and moved up it when the situation called for it.
- **Watch for claims presented at a higher rung than they actually earned** — an assumption stated with the confidence of an observed fact is a warning sign in its own right, independent of whether the underlying claim turns out to be true.

## Recording A Concern

When something in an answer doesn't add up — a claim that seems too strong for its evidence, a gap in the story, a contradiction — record it in this shape rather than a vague note:

- **What the concern is.** One sentence.
- **Why it matters.** What decision or claim it would undermine if true.
- **What evidence exists for and against it,** and where each piece sits on the Evidence Ladder.
- **What would resolve it.** A specific follow-up question or piece of evidence that would let you close the concern one way or the other.

Ask the resolving question in the interview if there's time. If a candidate's later answer genuinely resolves the concern, close it — don't keep scoring against a concern that's been addressed. If it isn't resolved, it becomes part of the evidence record you carry into the scoring and debrief steps in [scoring-rubric.md](scoring-rubric.md).

## Pressure As A Dial, Not A Switch

Some cards benefit from turning up pressure for a senior or Director-level candidate — more skeptical follow-ups, less patience with restating the question instead of answering it, more "but what if that assumption is wrong?" Some don't need it at all. Treat pressure as something you can dial per candidate and per round, not something baked into a question's wording:

- **Baseline:** ask the question and the card's neutral probes as written. This is the default for every candidate.
- **Elevated:** add skeptical follow-ups that press on the weakest-looking claim — "how do you know that was actually the cause?" — reserved for cards whose card explicitly notes it (see Role Or Level Notes on relevant cards), or for a senior candidate where the interviewer wants to see how they hold up under real scrutiny.
- **Never:** invented facts, impossible standards, interrupting to prevent an answer, or refusing to be persuaded by good evidence. Pressure tests the candidate's reasoning, not their patience for abuse. If a candidate produces genuinely strong evidence, the interviewer's job is to recognize it, not keep moving the bar.

## When To Use This

Not every card needs the full ladder and concern-record treatment — for most behavioral cards, the existing Strong Evidence / Warning Signs sections are enough. Reach for this standard specifically for judgment-type cards where a candidate is defending a decision (a roadmap trade-off, a business case, a claim about a competitor) and the quality of their evidence, not just the decision itself, is the thing being assessed.
