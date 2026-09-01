# Modernization Plan

## Purpose

Update this repository from a small collection of Product Manager interview prompts into a practical, evidence-informed toolkit for running structured interviews.

The durable job of the project is to help interviewers assess product judgment in context: how a candidate makes decisions, works with others, learns from customers, uses evidence, and handles ambiguity. It is not a catalogue of clever prompts or a test of framework recall.

## What The Research Says

The research in [`Research/`](../Research/) points in the same direction:

- Favor behavioral, situational, and judgment questions over trivia, brainteasers, and generic product-design hypotheticals.
- Assess the reasoning behind an answer, not whether a candidate names a familiar framework.
- Use a structured loop: consistent questions, neutral follow-ups, and shared scoring anchors improve comparability and reduce interviewer bias.
- Maintain a large question bank, but run a short, deliberate interview loop. A 12-16 question core set is a useful starting point, not a 100-question interview.
- Assess a broader set of capabilities: customer understanding, judgment, strategy, delivery, metrics, influence, communication, ownership, ethics, and self-awareness.

The research files are working syntheses, not a ready-made source bibliography. Before material is published as factual guidance, verify primary sources and replace AI-style citation artifacts with stable, readable links.

## Recommended End State

```text
README.md                         Start here: purpose, use, principles
AGENTS.md                         Editorial and maintenance contract
docs/
  competency-model.md             What the interview assesses
  scoring-rubric.md               Shared 1-5 evidence-based scoring
  structured-interview-guide.md   How to assemble and run an interview loop
  MODERNIZATION-PLAN.md           This roadmap
Questions/
  behavioral/                     Evidence from past work
  situational/                    Judgment in a realistic future scenario
  judgment/                       Trade-offs, ethics, ambiguity, decisions
  method/                         Targeted execution or craft questions
  ai/                             Optional AI-competency layer (domain-based; added later as AI traffic grew)
  systems-thinking/               Problem breakdown, systems mapping, and Precedents Thinking candidates
```

Each current question should eventually become a complete interview card, not merely a prompt. The card should contain:

- The question and its type
- The competency or competencies it assesses
- Why it matters
- Neutral follow-up probes
- Strong evidence and warning signs
- A 1-5 scoring anchor
- Level, context, or role-fit notes where genuinely useful

## Question Design Standard

Questions should invite specific evidence and make room for the candidate to explain their own thinking. Good questions have a clear purpose, avoid hidden gotchas, and can be scored consistently by more than one interviewer.

Prefer:

- "Tell me about a time..." questions that elicit context, action, outcome, and learning.
- Situations with real constraints and trade-offs.
- Prompts about customer evidence, prioritization, communication, conflict, delivery, recovery, and responsible decisions.
- Follow-ups that clarify a candidate's own contribution and reasoning.

Avoid using as primary assessment:

- Market-sizing puzzles, unless quantitative estimation is genuinely central to the role.
- Abstract product-design prompts without real constraints or a scoring rubric.
- Questions that reward rehearsed frameworks, company trivia, or a particular background.
- Questions about protected characteristics, personal circumstances, or cultural conformity.

## Treatment Of Existing Material

Do not delete the old questions merely because they are dated. They document the project's original shape and may still be useful as teaching examples or secondary exercises.

- Keep and rewrite the strongest behavior-oriented prompts first: building trust with a new team, responding to paradigm shifts, and distinguishing vanity metrics from actionable metrics.
- Move broad design prompts and estimation puzzles into `Questions/systems-thinking/` only when their real value is problem breakdown, systems mapping, estimation-as-modeling, or Precedents Thinking. Otherwise, leave them as background context rather than active interview material.
- Label retained systems-thinking candidates clearly: useful for future exercise design, not recommended as standalone hiring signals until rewritten with a defensible rubric.
- Replace the current boilerplate with the interview-card template before adding new questions.

## Phased Work

### Phase 1: Establish The New Contract — Done

1. ~~Rewrite the README to state the behavior-first purpose, explain the repository layout, and give a simple route for using the material.~~
2. ~~Add `AGENTS.md` to preserve the editorial standard and future maintenance decisions.~~
3. ~~Replace `Questions/Interview Question Boilerplate.md` with the full interview-card template.~~
4. ~~Create the competency model, scoring rubric, and structured interview guide in `docs/`.~~ See [competency-model.md](competency-model.md), [scoring-rubric.md](scoring-rubric.md), [structured-interview-guide.md](structured-interview-guide.md).

### Phase 2: Curate The Existing Bank — Done

1. ~~Tag every existing prompt as retain-and-rewrite, legacy, or retire.~~ See [question-bank-triage.md](question-bank-triage.md).
2. ~~Rewrite the three strongest retained prompts as exemplar interview cards.~~ Building Trust, Seismic Paradigm Shifts, Vanity Metrics.
3. ~~Move historical material without changing its original text, adding a short context note where needed.~~ Later refined: these two prompts now live in `Questions/systems-thinking/` because their best future use is problem breakdown and systems modeling.
4. ~~Add an index so contributors can find questions by competency and type.~~ See [question-index.md](question-index.md).

The two remaining retained prompts (Alarm Clock for the Blind, Technical Sizing Sanity Check) were also rewritten into full cards, beyond the plan's original three-exemplar minimum.

### Phase 3: Build A Usable Core Loop — Done

1. ~~Define a 12-16 question core bank across judgment, customer understanding, strategy, execution, influence, metrics, communication, ownership, ethics, and self-awareness.~~ Started at 14 cards, grew to 20 after a pass drawing inspiration from adjacent decision-review and competitive-intelligence practice, to 30 after adding an optional AI-competency layer, to 34 after a further pass adding a defensible market-sizing method, a premortem exercise, and two more AI cards, to 40 after adding six named stakeholder-pressure scenarios from the repository owner's own published work, to 46 after closing a structural gap — the whole bank was individual-contributor-focused — with a new optional people-management layer (Round 6) plus two general situational cards, to 49 after three cards testing the judgment underneath engineering sizing frameworks, distinct from the mechanics-level Technical Sizing Sanity Check, to 52 after auditing a 70-question generic compendium against the active bank and closing three narrower gaps it surfaced (decision-rights ambiguity between peers, live diagnostic reasoning when metrics conflict, and reaching for a non-product lever), and to 58 after mining the repository owner's own public Substack essays for six angles the AI-competency layer didn't yet cover (verifying AI-synthesized research, stopping a zombie AI bet, making an AI feature's business case to finance, context engineering as a team practice, bolt-on-vs-redesign strategy, and internal AI-project risk) — see [core-interview-loop.md](core-interview-loop.md), [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md), [ai-competency-model.md](ai-competency-model.md), and [people-management-competency.md](people-management-competency.md).
2. ~~Define which questions are appropriate for each interview stage; no single interviewer should try to assess everything.~~ Four rounds, one interviewer per round — see [core-interview-loop.md](core-interview-loop.md).
3. ~~Add interviewer calibration guidance and example evidence-based score rationales.~~ See the Calibration and Worked Examples sections of [scoring-rubric.md](scoring-rubric.md).
4. ~~Pilot the loop with experienced interviewers and revise questions that create uneven interpretation.~~ Superseded: this repository is a public preview, so real-world usage across many interviewers and roles is the feedback mechanism, not a single controlled pilot. See [field-feedback-guide.md](field-feedback-guide.md) for how usage turns into a fix.

A further pass added a 4-level pressure taxonomy (`constructive`/`skeptical`/`resistant`/`hostile-room`, adapted from a private adversarial-review tool with an explicit Candidate Safety Cap since a real candidate hasn't consented to adversarial rehearsal) and [interviewer-voices.md](interviewer-voices.md), four named interviewer personas built on those levels — see [evidence-and-pressure-standard.md](evidence-and-pressure-standard.md).

The original 12 AI-competency cards were then moved from `judgment/`/`method/` into a new `Questions/ai/` folder, a peer to `behavioral/`/`situational/`/`judgment/`/`method/` rather than nested inside them — anticipating that AI-specific questions will see disproportionately frequent traffic and may eventually warrant splitting into their own repository as the AI-PM discipline stabilizes. `ai/` is domain-based, not format-based (each card still records its own Type internally). The folder grew to 18 cards after a later mining pass — see the Phase 3 history above. `Questions/systems-thinking/` is now the other domain-style exception: not active cards, but a deliberate lane for problem-breakdown, systems-mapping, and Precedents Thinking exercises.

### Phase 4: Publish With Provenance — Done

1. ~~Audit the research for stable primary sources and clear attribution.~~ All `Research/` files are now audited — see [research-audit.md](research-audit.md). `gpt...md` had 43 broken AI-citation artifacts resolved to real links (plus a corrected validity statistic); `plex...md` and `gem...md` were link-checked (a small number of dead links fixed or flagged inline); `copilot...md` was confirmed to be an original question bank needing no per-claim sourcing, not a duplicate of the other three. One residual issue remains open in `gem...md` (an inline-citation-numbering integrity problem, not a link-validity one) — see research-audit.md for detail.
2. ~~Add a contributor guide with the question-card standard and review criteria.~~ See [`CONTRIBUTING.md`](../CONTRIBUTING.md).
3. ~~Document scope and limitations: this is an interviewing aid, not a replacement for legal guidance, interviewer training, or a hiring process.~~ See the Scope section of [`README.md`](../README.md).

## Backlog: Further Inspiration Mining (Not Yet Scheduled)

Two sources reviewed during the Phase 3 inspiration passes weren't fully mined — noted here so the ideas aren't lost, not because they're committed to:

- **[MITRE Innovation Toolkit](https://itk.mitre.org/toolkit/tools-at-a-glance/)** — 25 of its 27 facilitation tools remain unreviewed beyond Premortem (already adapted into [`Questions/situational/The-Premortem.md`](../Questions/situational/The-Premortem.md)). Candidates worth a look: Problem Framing, Retro Rundown, Rose Bud Thorn, Stakeholder Power/Map. Same filter as always applies — a tool becomes an interview card only if it has a real, scoreable signal, not just a facilitation format.
- **A private prompt-generator library** — JTBD, DACI, and discovery-interview prompt generators not yet reviewed for interview-card potential; likely relevant to Round 1 (Customer Understanding And Discovery).

Revisit when there's appetite for another mining pass; don't let this silently expand scope on its own. Tracked on the [Role & Domain Coverage board](https://github.com/users/deanpeters/projects/3), alongside any role- or domain-specific coverage requests that come in through [field-feedback-guide.md](field-feedback-guide.md).

## Definition Of Done

The refresh is complete when a new interviewer can select a role-appropriate loop, ask each question consistently, record evidence, score it against shared anchors, and understand why a question belongs in the process. The repository should make that path clear without requiring the reader to infer an interviewing philosophy from a collection of prompts.
