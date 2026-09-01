# Core Interview Loop

## Purpose

A stable, 58-question core bank and a suggested loop structure for running it — the "usable core loop" called for in [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 3. Pairs with [competency-model.md](competency-model.md) (what to assess), [ai-competency-model.md](ai-competency-model.md) (the optional AI-specific layer), [people-management-competency.md](people-management-competency.md) (the optional manager-track layer), [scoring-rubric.md](scoring-rubric.md) (how to score it), [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md) (how to grade the evidence in an answer and, for senior candidates, how to apply pressure responsibly), [interviewer-voices.md](interviewer-voices.md) (optional named personas for a consistent round style), [negotiation-signals.md](negotiation-signals.md) (techniques to listen for on stakeholder-pressure cards), [interview-scorecard-template.md](interview-scorecard-template.md) (the fillable worksheet an interviewer actually uses during a round), and [structured-interview-guide.md](structured-interview-guide.md) (how to run any interview in the loop). See [question-index.md](question-index.md) for the full catalogue, including legacy material not part of this core set.

The original 14 cards draw on the research synthesis in [`Research/gpt.pm-interview-and-behavioral-questions.md`](../Research/gpt.pm-interview-and-behavioral-questions.md). Six more were added, adapted from decision-review and competitive-intelligence practice used elsewhere in this project owner's tooling. Ten AI-specific cards were added next, adapted from [`Research/AI Product Management Assessment.md`](../Research/AI%20Product%20Management%20Assessment.md). Four more cards followed — a defensible market-sizing method, a premortem risk exercise, and two more AI cards (agentic-system governance, external risk scanning). Six more were added from *The Dangerous Animals of Product Management* (Productboard, in partnership with Dean Peters, 2022) and its companion 2021 ProductCamp talk — real, publicly published stakeholder-pressure archetypes (HiPPO, RHiNO, ZEbRA, WoLF, Seagull Manager, CoBRA), each grounded in a real named case study. Six more closed two more gaps: two general situational cards (market expansion reasoning, a new role's first 90 days) and four people-management cards for manager-track roles, adapted from the same internal leveling worksheet behind the core scorecard. A final three cards test the judgment underneath engineering sizing frameworks — not sizing mechanics, which [Technical Sizing Sanity Check](../Questions/method/technicalSizing.01.md) already covers, but what a sizing estimate is actually measuring, adapted from two internal sizing rubrics (`Research/epic-sizing-considerations.png`, `Research/story-sizing-considerations.png`); see each card's Attributions section for specifics. A further three cards closed narrower gaps surfaced by auditing a 70-question generic compendium (`Research/gemini.pm-questions-compendium.md`) against the active bank: peer-vs-peer decision-rights ambiguity, live diagnostic reasoning when two metrics disagree, and whether a candidate's solution space extends past "build a feature." A final six cards extended the AI-competency layer, mined from Dean Peters's own public Substack essays: verifying AI-synthesized research against source quotes, telling a proven AI bet from a zombie one, translating AI value into a finance-legible lever, context engineering as a team practice rather than an individual one, bolt-on-AI vs. redesigning a workflow around it, and internal (as opposed to external/regulatory) AI-project risk. All fifty-eight were written originally for this project, not copied from any source.

## Do Not Ask All 58 In One Interview

58 questions is the size of the *bank*, not of any one conversation. A single interviewer should ask roughly 3-4 questions in a 45-60 minute slot, chosen from the group they own below, and go deep with follow-up probes rather than rushing through more questions shallowly.

## The Core Bank By Round

### Round 1 — Customer Understanding And Discovery

Owns: does the candidate get curious before getting clever?

- [The Feature That Wasn't the Problem](../Questions/behavioral/Feature-That-Wasnt-The-Problem.md) — Behavioral
- [Designing for a Constraint You Don't Share](../Questions/situational/AlarmClock-Design4Blind.md) — Situational
- [The Loaded Ask](../Questions/situational/The-Loaded-Ask.md) — Situational
- [A Critique You'd Stand Behind](../Questions/judgment/A-Critique-Youd-Stand-Behind.md) — Judgment
- [The One Deal That Needs One Feature](../Questions/situational/The-One-Deal-That-Needs-One-Feature.md) — Situational
- [The First 90 Days](../Questions/situational/The-First-90-Days.md) — Situational
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
- [The Premortem](../Questions/situational/The-Premortem.md) — Situational
- [Should We Expand Into That Market?](../Questions/situational/Should-We-Expand-Into-That-Market.md) — Situational
- [What Your Estimate Is Actually Measuring](../Questions/judgment/What-Your-Estimate-Is-Actually-Measuring.md) — Judgment
- [Weeks for Leadership, Points for the Team](../Questions/judgment/Weeks-for-Leadership-Points-for-the-Team.md) — Judgment
- [The 21-Point Story](../Questions/judgment/The-21-Point-Story.md) — Judgment
- [Sizing a Market You Can Defend](../Questions/method/Sizing-a-Market-You-Can-Defend.md) — Method *(optional add-on where market sizing is a real skill for the role)*
- [One Signal Up, Another Down](../Questions/judgment/One-Signal-Up-Another-Down.md) — Judgment
- [Not Every Fix Is a Feature](../Questions/behavioral/Not-Every-Fix-Is-a-Feature.md) — Behavioral

This round has grown into a deliberately large pool — pick 3-4 per loop based on the role (a strategy-heavy role might favor Reading Market Signals and Separating a Funded Move; a delivery-heavy role might favor Shipped, But Didn't Work and Defending a Roadmap Trade-off; a role with real estimation/planning ownership might favor the three sizing-judgment cards together). Don't ask all fifteen in one sitting.

### Round 3 — Influence, Collaboration, And Communication / Delivery, Execution, And Ownership

Owns: can the candidate get things done through people they don't manage, and see it through?

- [Building Trust with New Teams](../Questions/behavioral/Building-Trust-with-New-Teams.md) — Behavioral
- [Influence Without Authority](../Questions/behavioral/Influence-Without-Authority.md) — Behavioral
- [Prepping for a Room You Don't Control](../Questions/behavioral/Prepping-for-a-Room-You-Dont-Control.md) — Behavioral
- [Dealing with Seismic Paradigm Shifts](../Questions/behavioral/Dealing-with-Seismic-Paradigm-Shifts.md) — Behavioral
- [Overruling the HiPPO](../Questions/situational/Overruling-the-HiPPO.md) — Situational
- [A Confident Opinion With No Evidence](../Questions/situational/A-Confident-Opinion-With-No-Evidence.md) — Situational
- [Negotiating the Technical-Debt Fire](../Questions/situational/Negotiating-the-Technical-Debt-Fire.md) — Situational
- [The Weekend Code Drop](../Questions/behavioral/The-Weekend-Code-Drop.md) — Behavioral
- [Who Actually Owns This Decision](../Questions/judgment/Who-Actually-Owns-This-Decision.md) — Judgment
- [Technical Sizing Sanity Check](../Questions/method/technicalSizing.01.md) — Method *(optional add-on for technical/web-related roles; best run by or with an engineer)*

This round has also grown into a large pool — pick 3-4 based on the role and the kind of stakeholder pressure it involves (a sales-heavy org might favor The One Deal That Needs One Feature in Round 1 and Overruling the HiPPO here; a platform role might favor Negotiating the Technical-Debt Fire and the technical sizing check).

### Round 4 — Ethics, Self-Awareness, And Responsible Decision-Making

Owns: does the candidate hold themselves accountable, and weigh user trust alongside business metrics?

- [A Decision You Got Wrong](../Questions/behavioral/A-Decision-You-Got-Wrong.md) — Behavioral
- [When Growth Could Harm Customers](../Questions/judgment/When-Growth-Could-Harm-Customers.md) — Judgment
- [Catching Your Own Bias](../Questions/behavioral/Catching-Your-Own-Bias.md) — Behavioral

Round 4 is intentionally short — go deep on 2-3 of these rather than padding the round with unrelated questions borrowed from elsewhere.

### Round 5 — AI Product Judgment (Optional, AI-Heavy Roles Only)

Owns: does the candidate reason well about AI-specific product judgment — see [ai-competency-model.md](ai-competency-model.md) before using this round at all. Skip it entirely for roles where AI isn't a real part of the product surface; running it anyway tests trivia, not job-relevant judgment.

- [Explaining AI Limits to a Skeptic](../Questions/ai/Explaining-AI-Limits-to-a-Skeptic.md) — Method (AI Fundamentals)
- [Where AI Actually Helps](../Questions/ai/Where-AI-Actually-Helps.md) — Judgment (AI Opportunity Discovery)
- [Testing an AI Idea Before It's Real](../Questions/ai/Testing-an-AI-Idea-Before-Its-Real.md) — Judgment (AI Product Discovery & Validation)
- [What the Model Needs to Know](../Questions/ai/What-the-Model-Needs-to-Know.md) — Judgment (Data & Context Strategy)
- [How Much Should the AI Decide](../Questions/ai/How-Much-Should-the-AI-Decide.md) — Judgment (AI Experience & Human Agency)
- [When the Model Is Wrong](../Questions/ai/When-the-Model-Is-Wrong.md) — Judgment (AI Evaluation & Metrics)
- [The Line You Wouldn't Cross](../Questions/ai/The-Line-You-Wouldnt-Cross.md) — Judgment (AI Risk, Safety & Responsible Use)
- [Build, Buy, or Wait](../Questions/ai/Build-Buy-or-Wait.md) — Judgment (AI Economics & Technical Tradeoffs)
- [Turning Usage Into a Better Model](../Questions/ai/Turning-Usage-Into-a-Better-Model.md) — Judgment (AI Product Operations & Learning)
- [AI as a Moat, or Not](../Questions/ai/AI-as-a-Moat-or-Not.md) — Judgment (AI Strategy & Competitive Advantage)
- [Governing an Agent That Acts on Its Own](../Questions/ai/Governing-an-Agent-That-Acts-on-Its-Own.md) — Judgment (AI Experience & Human Agency)
- [Scanning External Forces Before You Bet on AI](../Questions/ai/Scanning-External-Forces-Before-You-Bet-on-AI.md) — Judgment (AI Risk, Safety & Responsible Use)
- [Which Customer Said This?](../Questions/ai/Which-Customer-Said-This.md) — Method (AI Fundamentals)
- [Kill the Zombie Pilot](../Questions/ai/Kill-the-Zombie-Pilot.md) — Judgment (AI Product Operations & Learning)
- [The Lever the CFO Can See](../Questions/ai/The-Lever-the-CFO-Can-See.md) — Judgment (AI Economics & Technical Tradeoffs)
- [Twelve Tabs, Twelve Truths](../Questions/ai/Twelve-Tabs-Twelve-Truths.md) — Judgment (Data & Context Strategy)
- [Frankensoft or AI-First](../Questions/ai/Frankensoft-or-AI-First.md) — Judgment (AI Strategy & Competitive Advantage)
- [The Storm You Could See in Week One](../Questions/ai/The-Storm-You-Could-See-in-Week-One.md) — Behavioral (AI Risk, Safety & Responsible Use)

Eighteen cards for one round is deliberately more than any single interview needs — pick 3-4 that match where AI actually shows up in the role (a chat-product PM might prioritize Human Agency and Evaluation & Metrics; a platform PM enabling other teams' AI features might prioritize Data & Context Strategy and Economics & Technical Tradeoffs; a PM leading a portfolio of AI bets might prioritize Kill the Zombie Pilot and The Lever the CFO Can See).

### Round 6 — People Management (Optional, Manager-Track Roles Only)

Owns: can the candidate actually grow, structure, and lead a team of PMs — see [people-management-competency.md](people-management-competency.md) before using this round at all. Skip it entirely for individual-contributor and Senior PM roles; running it on a candidate who won't manage anyone tests a skill the role doesn't need.

- [Growing a PM You Manage](../Questions/people-management/Growing-a-PM-You-Manage.md) — Behavioral (Coaching & Development)
- [Building the Team You Need](../Questions/people-management/Building-the-Team-You-Need.md) — Behavioral (Hiring & Team Composition)
- [Getting a Room Full of Strangers to Care](../Questions/people-management/Getting-a-Room-Full-of-Strangers-to-Care.md) — Behavioral (Evangelism)
- [Leading Through a Bad Quarter](../Questions/people-management/Leading-Through-a-Bad-Quarter.md) — Behavioral (Leadership & Motivation)

All four are worth asking for a Director/VP loop — this round is intentionally smaller than Round 5, and unlike Round 5's AI cards, these aren't a large pool to filter down from.

## Assembling A Loop

1. **Weight rounds to the role**, per [structured-interview-guide.md](structured-interview-guide.md) — a growth PM role may want Round 2 to run longer; a platform PM role may want Round 3 to include the technical sizing check for every candidate rather than as optional. Add Round 5 only when AI is a real part of the role, and Round 6 only for manager-track roles. See [role-loop-presets.md](role-loop-presets.md) for four fully worked examples rather than deriving this from scratch each time.
2. **Assign one interviewer per round.** No single interviewer should try to cover all four (or more) rounds; that's the entire point of splitting by competency ownership.
3. **Every candidate for a given role gets the same rounds and the same selected questions**, so scores are comparable. Don't swap questions in or out per candidate.
4. **Record and score independently per [scoring-rubric.md](scoring-rubric.md)** before any debrief.
5. **For Director/VP-level roles**, several cards carry a Role Or Level Notes section with a senior-specific follow-up or a note to raise pressure per [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md) — check each selected card for one before the interview, rather than improvising pressure on the spot.

## Coverage Note

The original 14-question bank was assembled to close the gap [question-index.md](question-index.md) previously flagged: no card primarily assessed Product Judgment/Strategy/Prioritization. Round 2 now covers that directly, and heavily — it's the largest round by design, since defending a decision under scrutiny is a large part of the job at every level. Four more cards closed two specific gaps: a genuinely defensible market-sizing method (distinct from the legacy estimation puzzle in `Questions/legacy/`) and agentic-system governance and external risk-scanning within the AI layer. Six cards added named, real-world stakeholder-pressure scenarios to Rounds 1, 3, and 4 — a candidate's ability to handle a HiPPO, a RHiNO, a ZEbRA, or a Seagull Manager by name is exactly the kind of situational judgment a résumé can't show. The final six closed a structural gap: the whole bank was individual-contributor-focused until Round 6 added a dedicated people-management layer for manager-track roles, alongside two general situational cards (market expansion, a new role's first 90 days). Three more cards then tested the judgment underneath engineering sizing frameworks, and three more — decision-rights ambiguity between peers, live diagnostic reasoning when metrics conflict, and reaching for a non-product lever — closed narrower gaps found by auditing a broad generic-question compendium against the active bank. A final six cards extended the AI-competency layer to six angles a portfolio-level or Director-track AI PM will actually face — verifying AI-synthesized research, stopping a zombie AI bet, making an AI feature's business case to finance, context engineering as a team discipline, bolt-on-vs-redesign strategy, and internal AI-project risk — mined from the repository owner's own public writing, not from any framework already in the bank. If future roles surface a competency this bank underserves, add a new card to the relevant type folder and this document, rather than stretching an existing card to cover ground it wasn't designed for.

## Real-World Feedback

This repository is in public preview. Rather than a controlled pilot, real usage in real interviews is the feedback mechanism — see [field-feedback-guide.md](field-feedback-guide.md) for how to try a card and report what you find.
