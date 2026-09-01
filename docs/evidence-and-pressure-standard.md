# Evidence And Pressure Standard

## Purpose

A shared vocabulary for what counts as evidence in an answer, and a lightweight way to record a specific concern about that evidence — so "strong evidence" and "warning signs" mean the same thing across every card, not just whatever each card's author happened to write. Pairs with [scoring-rubric.md](scoring-rubric.md) (how to turn evidence into a score), [structured-interview-guide.md](structured-interview-guide.md) (how to run the conversation that surfaces it), and [interviewer-voices.md](interviewer-voices.md) (named personas built on the pressure levels below).

The evidence ladder is adapted from the evidence-grading approach used in adversarial product-review practice (the kind of rigor applied to a roadmap or business case before it goes in front of an executive), translated here for interview evidence rather than document review. The pressure levels below are adapted more directly from a private adversarial product-decision-review tool's pressure-level and stakeholder-persona mechanics (`product-manager-antagonist-skills/shared/pressure-levels.md` and `dialogue-mode.md`) — see the Candidate Safety Cap for the important way that adaptation had to change for a real hiring interview rather than a consenting rehearsal.

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

## Pressure Levels

Pressure changes how much resistance an interviewer gives a candidate's claims and how quickly they follow up on a weak one — not whether the interviewer is respectful. This four-level taxonomy is adapted from adversarial product-decision-review practice, where a user rehearses a pitch against a colleague who has agreed to play a skeptical or hostile stakeholder. **That consent structure does not exist in a real hiring interview** — a candidate has not opted into adversarial treatment the way a colleague rehearsing a pitch has. The levels below are capped accordingly; see Candidate Safety Cap below before using anything past `skeptical` on a real candidate.

| Level | Burden of proof | Interviewer behavior | Appropriate use |
|---|---|---|---|
| `constructive` | Reasonable, provisional evidence is accepted | Patient clarification, generous time to think, collaborative tone | Early-career candidates, first-round screens, Round 1 (Customer Understanding) |
| `skeptical` | Load-bearing claims need explicit support | Faster follow-up, tests assumptions and the weakest-looking claim, limited acceptance of vague answers | The default for most rounds and most candidates — this is what the neutral follow-up probes on every card already assume |
| `resistant` | The claim starts at "not yet proven" until the candidate earns it | Pursues the gap directly, tests what the candidate would do if their key assumption were wrong, expects decision-relevant evidence rather than a plausible story | Director/VP-level rounds, or a card whose Role Or Level Notes explicitly call for it |
| `hostile-room` | Multiple unresolved objections at once, little patience for a good-sounding but unsupported answer | Interrupts a wandering answer, returns to what's still unresolved, offers real resistance | **Not for real candidate interviews** — see Candidate Safety Cap |

## Candidate Safety Cap

- **`hostile-room` is reserved for internal use only** — staff rehearsing with each other before running a high-stakes loop, or interviewer-training exercises where everyone involved has agreed to the exercise. Never run it against an actual candidate. A real candidate hasn't consented to adversarial rehearsal the way a colleague preparing a pitch has, and uneven "hostility" across candidates is also a fairness problem, not just a tone problem — it risks scoring candidates on how they handle an interviewer's mood rather than on comparable evidence.
- **`resistant` is the practical ceiling for real candidates**, and only for senior/Director/VP rounds or a card that explicitly calls for it (see [role-loop-presets.md](role-loop-presets.md)'s Director/VP preset). It should never involve interrupting to prevent an answer, inventing facts, or refusing to be persuaded by genuinely strong evidence.
- **Invariants at every level, including `resistant`:** challenge the claim, not the candidate. Accept evidence that actually resolves a concern — don't keep moving the bar once a candidate produces it. Never invent facts or impossible standards. Never confuse rudeness with rigor.
- **Increase pressure one level at a time**, and only when the interview plan called for it in advance (see the [scorecard template](interview-scorecard-template.md)'s header) — never as an improvised reaction to a candidate you've decided you don't like.

See [interviewer-voices.md](interviewer-voices.md) for named interviewer personas built on these levels, each capped the same way.

## When To Use This

Not every card needs the full ladder and concern-record treatment — for most behavioral cards, the existing Strong Evidence / Warning Signs sections are enough. Reach for this standard specifically for judgment-type cards where a candidate is defending a decision (a roadmap trade-off, a business case, a claim about a competitor) and the quality of their evidence, not just the decision itself, is the thing being assessed.
