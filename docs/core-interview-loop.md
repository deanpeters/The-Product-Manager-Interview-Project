# Core Interview Loop

## Purpose

A stable, 30-question core bank and a suggested loop structure for running it — the "usable core loop" called for in [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 3. Pairs with [competency-model.md](competency-model.md) (what to assess), [ai-competency-model.md](ai-competency-model.md) (the optional AI-specific layer), [scoring-rubric.md](scoring-rubric.md) (how to score it), [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md) (how to grade the evidence in an answer and, for senior candidates, how to apply pressure responsibly), [interview-scorecard-template.md](interview-scorecard-template.md) (the fillable worksheet an interviewer actually uses during a round), and [structured-interview-guide.md](structured-interview-guide.md) (how to run any interview in the loop). See [question-index.md](question-index.md) for the full catalogue, including legacy material not part of this core set.

The original 14 cards draw on the research synthesis in [`Research/gpt.pm-interview-and-behavioral-questions.md`](../Research/gpt.pm-interview-and-behavioral-questions.md). Six more were added, adapted from decision-review and competitive-intelligence practice used elsewhere in this project owner's tooling. A further ten AI-specific cards were added last, adapted from [`Research/AI Product Management Assessment.md`](../Research/AI%20Product%20Management%20Assessment.md) — see each card's Attributions section for specifics. All thirty were written originally for this project, not copied from any source.

## Do Not Ask All 30 In One Interview

30 questions is the size of the *bank*, not of any one conversation. A single interviewer should ask roughly 3-4 questions in a 45-60 minute slot, chosen from the group they own below, and go deep with follow-up probes rather than rushing through more questions shallowly.

## The Core Bank By Round

### Round 1 — Customer Understanding And Discovery

Owns: does the candidate get curious before getting clever?

- [The Feature That Wasn't the Problem](../Questions/behavioral/Feature-That-Wasnt-The-Problem.md) — Behavioral
- [Designing for a Constraint You Don't Share](../Questions/situational/AlarmClock-Design4Blind.md) — Situational
- [The Loaded Ask](../Questions/situational/The-Loaded-Ask.md) — Situational
- [A Critique You'd Stand Behind](../Questions/judgment/A-Critique-Youd-Stand-Behind.md) — Judgment
- [Assumptions Worth Testing First](../Questions/judgment/Assumptions-Worth-Testing-First.md) — Judgment *(also relevant to Round 2; pick whichever round has room)*

### Round 2 — Product Judgment, Strategy, And Prioritization / Metrics, Outcomes, And Learning

Owns: can the candidate reason about trade-offs, evidence, and what "working" actually means?

- [Vanity Metrics vs. Actionable Analytics](../Questions/judgment/Vanity-Analytics_vs_Action-Metrics.md) — Judgment
- [Deciding Before You're Certain](../Questions/judgment/Deciding-Before-Youre-Certain.md) — Judgment
- [Shipped, But Didn't Work](../Questions/judgment/Shipped-But-Didnt-Work.md) — Judgment
- [Reading Market Signals](../Questions/judgment/Reading-Market-Signals.md) — Judgment
- [Ten Problems, One Focus](../Questions/judgment/Ten-Problems-One-Focus.md) — Judgment
- [Defending a Roadmap Trade-off](../Questions/judgment/Defending-a-Roadmap-Tradeoff.md) — Judgment
- [The Business Case Behind the Ask](../Questions/judgment/The-Business-Case-Behind-The-Ask.md) — Judgment
- [Separating a Funded Move From a Narrated One](../Questions/judgment/Separating-a-Funded-Move-From-a-Narrated-One.md) — Judgment

This round has grown into a deliberately large pool — pick 3-4 per loop based on the role (a strategy-heavy role might favor Reading Market Signals and Separating a Funded Move; a delivery-heavy role might favor Shipped, But Didn't Work and Defending a Roadmap Trade-off). Don't ask all eight in one sitting.

### Round 3 — Influence, Collaboration, And Communication / Delivery, Execution, And Ownership

Owns: can the candidate get things done through people they don't manage, and see it through?

- [Building Trust with New Teams](../Questions/behavioral/Building-Trust-with-New-Teams.md) — Behavioral
- [Influence Without Authority](../Questions/behavioral/Influence-Without-Authority.md) — Behavioral
- [Prepping for a Room You Don't Control](../Questions/behavioral/Prepping-for-a-Room-You-Dont-Control.md) — Behavioral
- [Dealing with Seismic Paradigm Shifts](../Questions/behavioral/Dealing-with-Seismic-Paradigm-Shifts.md) — Behavioral
- [Technical Sizing Sanity Check](../Questions/method/technicalSizing.01.md) — Method *(optional add-on for technical/web-related roles; best run by or with an engineer)*

### Round 4 — Ethics, Self-Awareness, And Responsible Decision-Making

Owns: does the candidate hold themselves accountable, and weigh user trust alongside business metrics?

- [A Decision You Got Wrong](../Questions/behavioral/A-Decision-You-Got-Wrong.md) — Behavioral
- [When Growth Could Harm Customers](../Questions/judgment/When-Growth-Could-Harm-Customers.md) — Judgment

Round 4 is intentionally the shortest — go deep on these two rather than padding the round with unrelated questions borrowed from elsewhere.

### Round 5 — AI Product Judgment (Optional, AI-Heavy Roles Only)

Owns: does the candidate reason well about AI-specific product judgment — see [ai-competency-model.md](ai-competency-model.md) before using this round at all. Skip it entirely for roles where AI isn't a real part of the product surface; running it anyway tests trivia, not job-relevant judgment.

- [Explaining AI Limits to a Skeptic](../Questions/method/Explaining-AI-Limits-to-a-Skeptic.md) — Method (AI Fundamentals)
- [Where AI Actually Helps](../Questions/judgment/Where-AI-Actually-Helps.md) — Judgment (AI Opportunity Discovery)
- [Testing an AI Idea Before It's Real](../Questions/judgment/Testing-an-AI-Idea-Before-Its-Real.md) — Judgment (AI Product Discovery & Validation)
- [What the Model Needs to Know](../Questions/judgment/What-the-Model-Needs-to-Know.md) — Judgment (Data & Context Strategy)
- [How Much Should the AI Decide](../Questions/judgment/How-Much-Should-the-AI-Decide.md) — Judgment (AI Experience & Human Agency)
- [When the Model Is Wrong](../Questions/judgment/When-the-Model-Is-Wrong.md) — Judgment (AI Evaluation & Metrics)
- [The Line You Wouldn't Cross](../Questions/judgment/The-Line-You-Wouldnt-Cross.md) — Judgment (AI Risk, Safety & Responsible Use)
- [Build, Buy, or Wait](../Questions/judgment/Build-Buy-or-Wait.md) — Judgment (AI Economics & Technical Tradeoffs)
- [Turning Usage Into a Better Model](../Questions/judgment/Turning-Usage-Into-a-Better-Model.md) — Judgment (AI Product Operations & Learning)
- [AI as a Moat, or Not](../Questions/judgment/AI-as-a-Moat-or-Not.md) — Judgment (AI Strategy & Competitive Advantage)

Ten cards for one round is deliberately more than any single interview needs — pick 3-4 that match where AI actually shows up in the role (a chat-product PM might prioritize Human Agency and Evaluation & Metrics; a platform PM enabling other teams' AI features might prioritize Data & Context Strategy and Economics & Technical Tradeoffs).

## Assembling A Loop

1. **Weight rounds to the role**, per [structured-interview-guide.md](structured-interview-guide.md) — a growth PM role may want Round 2 to run longer; a platform PM role may want Round 3 to include the technical sizing check for every candidate rather than as optional. Add Round 5 only when AI is a real part of the role.
2. **Assign one interviewer per round.** No single interviewer should try to cover all four (or five) rounds; that's the entire point of splitting by competency ownership.
3. **Every candidate for a given role gets the same rounds and the same selected questions**, so scores are comparable. Don't swap questions in or out per candidate.
4. **Record and score independently per [scoring-rubric.md](scoring-rubric.md)** before any debrief.
5. **For Director/VP-level roles**, several cards carry a Role Or Level Notes section with a senior-specific follow-up or a note to raise pressure per [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md) — check each selected card for one before the interview, rather than improvising pressure on the spot.

## Coverage Note

The original 14-question bank was assembled to close the gap [question-index.md](question-index.md) previously flagged: no card primarily assessed Product Judgment/Strategy/Prioritization. Round 2 now covers that directly, and heavily — it's the largest round by design, since defending a decision under scrutiny is a large part of the job at every level. If future roles surface a competency this bank underserves, add a new card to the relevant type folder and this document, rather than stretching an existing card to cover ground it wasn't designed for.

## What's Still Missing

Per [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 3, item 4: **piloting this loop with experienced interviewers and revising questions that create uneven interpretation** is not something that can be done from a repository alone — it requires running real interviews, comparing interviewer scores, and iterating. That step is still open and needs a human owner.
