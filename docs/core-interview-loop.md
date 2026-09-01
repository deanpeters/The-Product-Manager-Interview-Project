# Core Interview Loop

## Purpose

A stable, 14-question core bank and a suggested loop structure for running it — the "usable core loop" called for in [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 3. Pairs with [competency-model.md](competency-model.md) (what to assess), [scoring-rubric.md](scoring-rubric.md) (how to score it), and [structured-interview-guide.md](structured-interview-guide.md) (how to run any interview in the loop). See [question-index.md](question-index.md) for the full catalogue, including legacy material not part of this core set.

This bank draws on the research synthesis in [`Research/gpt.pm-interview-and-behavioral-questions.md`](../Research/gpt.pm-interview-and-behavioral-questions.md), which itself derives from hiring-science literature (structured-interview research) and a corpus of Product Management texts. That research file has unresolved AI-generated citation artifacts — see [research-audit.md](research-audit.md) — but the questions it proposes were written originally for this project, not copied from any source, so they're usable here without waiting on that cleanup.

## Do Not Ask All 14 In One Interview

14 questions is the size of the *bank*, not of any one conversation. A single interviewer should ask roughly 3-4 questions in a 45-60 minute slot, chosen from the group they own below, and go deep with follow-up probes rather than rushing through more questions shallowly.

## The Core Bank By Round

### Round 1 — Customer Understanding And Discovery

Owns: does the candidate get curious before getting clever?

- [The Feature That Wasn't the Problem](../Questions/behavioral/Feature-That-Wasnt-The-Problem.md) — Behavioral
- [Designing for a Constraint You Don't Share](../Questions/situational/AlarmClock-Design4Blind.md) — Situational
- [Assumptions Worth Testing First](../Questions/judgment/Assumptions-Worth-Testing-First.md) — Judgment *(also relevant to Round 2; pick whichever round has room)*

### Round 2 — Product Judgment, Strategy, And Prioritization / Metrics, Outcomes, And Learning

Owns: can the candidate reason about trade-offs, evidence, and what "working" actually means?

- [Vanity Metrics vs. Actionable Analytics](../Questions/judgment/Vanity-Analytics_vs_Action-Metrics.md) — Judgment
- [Deciding Before You're Certain](../Questions/judgment/Deciding-Before-Youre-Certain.md) — Judgment
- [Shipped, But Didn't Work](../Questions/judgment/Shipped-But-Didnt-Work.md) — Judgment
- [Reading Market Signals](../Questions/judgment/Reading-Market-Signals.md) — Judgment
- [Ten Problems, One Focus](../Questions/judgment/Ten-Problems-One-Focus.md) — Judgment

Pick 3-4 of these five per loop; don't ask all of them in one sitting even though they share a round.

### Round 3 — Influence, Collaboration, And Communication / Delivery, Execution, And Ownership

Owns: can the candidate get things done through people they don't manage, and see it through?

- [Building Trust with New Teams](../Questions/behavioral/Building-Trust-with-New-Teams.md) — Behavioral
- [Influence Without Authority](../Questions/behavioral/Influence-Without-Authority.md) — Behavioral
- [Dealing with Seismic Paradigm Shifts](../Questions/behavioral/Dealing-with-Seismic-Paradigm-Shifts.md) — Behavioral
- [Technical Sizing Sanity Check](../Questions/method/technicalSizing.01.md) — Method *(optional add-on for technical/web-related roles; best run by or with an engineer)*

### Round 4 — Ethics, Self-Awareness, And Responsible Decision-Making

Owns: does the candidate hold themselves accountable, and weigh user trust alongside business metrics?

- [A Decision You Got Wrong](../Questions/behavioral/A-Decision-You-Got-Wrong.md) — Behavioral
- [When Growth Could Harm Customers](../Questions/judgment/When-Growth-Could-Harm-Customers.md) — Judgment

Round 4 is intentionally the shortest — go deep on these two rather than padding the round with unrelated questions borrowed from elsewhere.

## Assembling A Loop

1. **Weight rounds to the role**, per [structured-interview-guide.md](structured-interview-guide.md) — a growth PM role may want Round 2 to run longer; a platform PM role may want Round 3 to include the technical sizing check for every candidate rather than as optional.
2. **Assign one interviewer per round.** No single interviewer should try to cover all four rounds; that's the entire point of splitting by competency ownership.
3. **Every candidate for a given role gets the same rounds and the same selected questions**, so scores are comparable. Don't swap questions in or out per candidate.
4. **Record and score independently per [scoring-rubric.md](scoring-rubric.md)** before any debrief.

## Coverage Note

This 14-question bank was assembled to close the gap [question-index.md](question-index.md) previously flagged: no card primarily assessed Product Judgment/Strategy/Prioritization. Round 2 now covers that directly. If future roles surface a competency this bank underserves, add a new card to the relevant type folder and this document, rather than stretching an existing card to cover ground it wasn't designed for.

## What's Still Missing

Per [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 3, item 4: **piloting this loop with experienced interviewers and revising questions that create uneven interpretation** is not something that can be done from a repository alone — it requires running real interviews, comparing interviewer scores, and iterating. That step is still open and needs a human owner.
