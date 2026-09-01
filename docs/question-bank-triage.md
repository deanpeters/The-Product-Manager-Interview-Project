# Question Bank Triage

## Purpose

A working record of the disposition of every file in `Questions/` as of the Phase 2 curation pass described in [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md). Each entry states what kind of prompt it is, which target type it maps to under the new structure, and what happens to it next.

Dispositions:

- **Retain & rewrite (exemplar)** — one of the three prompts the plan names explicitly as the first rewrites, to become the model for future interview cards.
- **Retain & rewrite** — kept as an active card, rewritten into the interview-card structure, but not a first-wave exemplar.
- **Legacy** — moved to `Questions/legacy/` unchanged in substance, labeled as historical material not recommended as a standalone hiring signal, per `AGENTS.md`.
- **Retire** — not currently used for any file; nothing is deleted without explicit direction.

## Triage Table

| File | Current Focus | Target Type | Disposition | Rationale |
|---|---|---|---|---|
| `Building-Trust-with-New-Teams.md` | Taking over an existing/new team, earning trust | Behavioral | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Strong behavioral prompt: elicits a real past situation, has a defensible rubric (servant-leadership, listening, respect for resistant teammates), assesses Influence/Collaboration and Ethics/Self-Awareness. |
| `Dealing-with-Seismic-Paradigm-Shifts.md` | Adjusting to a major organizational or priority shift | Behavioral / Situational | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Strong past-tense evidence question with clear positive/negative signals (learning orientation vs. blame). Assesses Delivery/Ownership and Ethics/Self-Awareness (how they talk about the change). |
| `Vanity-Analytics_vs_Action-Metrics.md` | Vanity metrics vs. actionable analytics | Judgment / Method | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Clear, well-sourced rubric (Actionable/Accessible/Auditable) and directly assesses Metrics, Outcomes, And Learning — a named competency. Already has real attributions to rework into the new card format. |
| `AlarmClock-Design4Blind.md` | Designing an alarm clock for blind users | Situational | **Retain & rewrite** | Unlike the vending-machine prompt, this has real constraints (accessibility, a specific user) and a rubric centered on discovery questions before design — it primarily tests Customer Understanding And Discovery, not open-ended ideation. Rewrite to foreground the discovery-question behavior as the pass/fail signal, per `AGENTS.md`'s caution on abstract design exercises. |
| `technicalSizing.01.md` | Sanity-checking engineering size estimates | Method | **Retain & rewrite** | Narrow, has a clear rubric and a specific defensible use (engineer-run technical sanity check), which is exactly the exception `AGENTS.md` allows for craft/execution questions. Keep as a `method/` card; note in Role/Level Notes that it's best run by or with an engineer. |
| `ProductDesign-VendingMachine.md` | Open-ended "disrupt the vending machine industry" ideation | — | **Legacy** | Abstract product-design brainstorm without real constraints or a scoring rubric beyond "broad/deep/excited" — exactly what `AGENTS.md` and the plan flag to avoid as a primary hiring signal. Move to `Questions/legacy/` with a historical-context note. |
| `Number-of-Pianos.md` | Market-sizing / estimation puzzle | — | **Legacy** | Classic market-sizing brainteaser. The plan explicitly calls for moving estimation puzzles to legacy unless a future rubric establishes a specific, defensible use. The file already self-documents this concern reasonably well; preserve it as a labeled historical example. |
| `Interview Question Boilerplate.md` | N/A — template, not a question | — | **N/A (template)** | Already replaced with the interview-card template in this pass; not part of the question bank triage. |

## Summary

- **3 exemplars** to rewrite first: Building Trust, Seismic Paradigm Shifts, Vanity Metrics.
- **2 additional active rewrites**: Alarm Clock for the Blind, Technical Sizing Sanity Check.
- **2 moves to legacy**: Vending Machine, Number of Pianos.
- **0 retirements.**

## Next Steps

1. ~~Create `Questions/behavioral/`, `Questions/situational/`, `Questions/judgment/`, `Questions/method/`, `Questions/legacy/`.~~ Done.
2. ~~`git mv` each file into its target folder (legacy files move as-is, plus a short historical-context note; active files move as a prelude to being rewritten in place).~~ Done.
3. ~~Add an index (by competency and type) once files are settled in their folders.~~ Done — see [question-index.md](question-index.md).
4. ~~Rewrite the three exemplars into the new interview-card structure.~~ Done — Building Trust, Seismic Paradigm Shifts, Vanity Metrics.
5. ~~Rewrite the two additional retained cards (Alarm Clock for the Blind, Technical Sizing Sanity Check).~~ Done.
6. ~~Update `question-index.md` to mark each card *(rewritten)* as it's completed, and firm up its competency links.~~ Done.

Phase 2 is complete. Nine additional cards were then written to fill out a 14-question core bank for Phase 3 — see [core-interview-loop.md](core-interview-loop.md) and [question-index.md](question-index.md) for the full active set.

A further six cards (Defending a Roadmap Trade-off, The Business Case Behind the Ask, Separating a Funded Move From a Narrated One, Prepping for a Room You Don't Control, The Loaded Ask, A Critique You'd Stand Behind) were added afterward, adapted from decision-review and competitive-intelligence practice external to this repository — see each card's Attributions section and [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md) for the shared vocabulary they introduced.

A further ten cards form an optional AI-competency layer (Explaining AI Limits to a Skeptic, Where AI Actually Helps, Testing an AI Idea Before It's Real, What the Model Needs to Know, How Much Should the AI Decide, When the Model Is Wrong, The Line You Wouldn't Cross, Build Buy or Wait, Turning Usage Into a Better Model, AI as a Moat or Not), adapted from [`Research/AI Product Management Assessment.md`](../Research/AI%20Product%20Management%20Assessment.md) — see [ai-competency-model.md](ai-competency-model.md) for the domain and when to use it. Only use these for roles where AI is a real part of the product surface.

A final four cards closed remaining gaps identified from a further inspiration pass: [Sizing a Market You Can Defend](../Questions/method/Sizing-a-Market-You-Can-Defend.md) (a genuinely defensible bottom-up market-sizing method, adapted from a private market-sizing prompt loop) and [The Premortem](../Questions/situational/The-Premortem.md) (adapted from the MITRE Innovation Toolkit's Premortem technique) both close Round 2 gaps; [Governing an Agent That Acts on Its Own](../Questions/ai/Governing-an-Agent-That-Acts-on-Its-Own.md) and [Scanning External Forces Before You Bet on AI](../Questions/ai/Scanning-External-Forces-Before-You-Bet-on-AI.md) (both adapted from a private AI-PM training curriculum) extend the AI-competency layer to agentic-system governance and external risk-scanning, gaps the original ten AI cards didn't cover.

**Note on `Sizing a Market You Can Defend` and the legacy `Number-of-Pianos.md`:** this new card does not rehabilitate the legacy estimation puzzle — it's a different exercise entirely (structured bottom-up market sizing with sourced, labeled inputs, versus a general Fermi-estimation brainteaser about counting objects in a building). `Number-of-Pianos.md` stays in `Questions/legacy/`; the "future rubric" condition noted there was satisfied by writing a new, purpose-built card rather than retrofitting the old one.

A final six cards were added from *The Dangerous Animals of Product Management* (Productboard, in partnership with Dean Peters, 2022) and its companion 2021 ProductCamp talk transcript — both real, publicly published works of the repository owner's, stored in `Research/`. Each card is grounded in a named stakeholder-pressure archetype and a real case study from the source material: [Overruling the HiPPO](../Questions/situational/Overruling-the-HiPPO.md) (JCPenney/Ron Johnson), [The One Deal That Needs One Feature](../Questions/situational/The-One-Deal-That-Needs-One-Feature.md) (ScaleFactor), [A Confident Opinion With No Evidence](../Questions/situational/A-Confident-Opinion-With-No-Evidence.md) (Blockbuster/Netflix), [Negotiating the Technical-Debt Fire](../Questions/situational/Negotiating-the-Technical-Debt-Fire.md) (Knight Capital), [The Weekend Code Drop](../Questions/behavioral/The-Weekend-Code-Drop.md) (Seagull Manager), and [Catching Your Own Bias](../Questions/behavioral/Catching-Your-Own-Bias.md) (Dunkin' Donuts/Robert Rosenberg). See [research-audit.md](research-audit.md) for the citation approach.

A final six cards closed two gaps surfaced by comparing the bank against a list of common generic PM interview questions: most of that list either duplicated existing cards or failed the rubric standard (self-report, company-specific trivia), but two genuine gaps stood out — [Should We Expand Into That Market?](../Questions/situational/Should-We-Expand-Into-That-Market.md) (proactive new-market reasoning, distinct from Reading Market Signals' reactive framing) and [The First 90 Days](../Questions/situational/The-First-90-Days.md) (diagnosis before acting in a new role, distinct from Building Trust's relationship focus) — plus a structural gap: the entire bank was individual-contributor-focused. Four people-management cards ([Growing a PM You Manage](../Questions/people-management/Growing-a-PM-You-Manage.md), [Building the Team You Need](../Questions/people-management/Building-the-Team-You-Need.md), [Getting a Room Full of Strangers to Care](../Questions/people-management/Getting-a-Room-Full-of-Strangers-to-Care.md), [Leading Through a Bad Quarter](../Questions/people-management/Leading-Through-a-Bad-Quarter.md)) close it for manager-track roles, grounded in the same internal leveling worksheet ([`Research/Product Manager Assessment - December 11, 2021.csv`](../Research/Product%20Manager%20Assessment%20-%20December%2011%2C%202021.csv)) that informs the core scorecard — see [people-management-competency.md](people-management-competency.md).

A final three cards ([What Your Estimate Is Actually Measuring](../Questions/judgment/What-Your-Estimate-Is-Actually-Measuring.md), [Weeks for Leadership, Points for the Team](../Questions/judgment/Weeks-for-Leadership-Points-for-the-Team.md), [The 21-Point Story](../Questions/judgment/The-21-Point-Story.md)) were adapted from two internal engineering sizing rubrics (`Research/epic-sizing-considerations.png`, `Research/story-sizing-considerations.png`) — deliberately testing the judgment underneath a sizing framework (what an estimate actually measures, why the unit changes by audience, what an outlier number signals) rather than sizing mechanics, which `Questions/method/technicalSizing.01.md` already covers.

A final three cards ([Who Actually Owns This Decision](../Questions/judgment/Who-Actually-Owns-This-Decision.md), [One Signal Up, Another Down](../Questions/judgment/One-Signal-Up-Another-Down.md), [Not Every Fix Is a Feature](../Questions/behavioral/Not-Every-Fix-Is-a-Feature.md)) were adapted from a 70-question generic compendium ([`Research/gemini.pm-questions-compendium.md`](../Research/gemini.pm-questions-compendium.md)), after auditing all 70 against the active bank and finding most already covered under different phrasing. The three that survived close genuine gaps: peer-vs-peer decision-rights ambiguity (distinct from Overruling the HiPPO's exec-outranks-you scenario), live diagnostic reasoning when two metrics disagree (distinct from Vanity Metrics' framework literacy and Shipped-But-Didn't-Work's post-mortem framing), and whether a candidate's solution space extends past "build a feature" into pricing, packaging, process, or services.

The active bank is now 52 cards (36 core + 12 optional AI-competency + 4 optional people-management).

This table should be updated if a disposition changes — e.g., if a specific rubric is later developed that would justify moving `Number-of-Pianos.md` or `ProductDesign-VendingMachine.md` back into active use.
