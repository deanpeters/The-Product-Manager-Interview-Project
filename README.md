# The Product Manager Interview Project

A practical, open collection for running better Product Manager interviews.

This repository is being updated from a flat catalogue of prompts into a structured interview toolkit. The focus is product judgment in context: how someone understands customers, makes decisions with incomplete information, works through trade-offs, collaborates, learns, and delivers outcomes.

It is not designed to reward memorized frameworks, brainteasers, or a performance of confidence.

## Start Here

If you are running an interview, use the project in this order:

1. Read the [modernization plan](docs/MODERNIZATION-PLAN.md) to understand the direction and what is still being built.
2. Use the [core interview loop](docs/core-interview-loop.md) — a ready-to-run 34-question core bank organized into four interviewer rounds, plus an optional fifth round for AI-heavy roles — or select individual questions from [`docs/question-index.md`](docs/question-index.md) that match the role and the decisions the person will need to make. See [`docs/role-loop-presets.md`](docs/role-loop-presets.md) for four worked examples (Growth PM, Platform PM, AI Product PM, Director/VP) rather than starting from scratch.
3. Ask the same core questions consistently across comparable candidates.
4. Use neutral follow-ups to understand the candidate's specific contribution, reasoning, evidence, and learning.
5. Record evidence before assigning a score, using the [scorecard template](docs/interview-scorecard-template.md). Score against the [shared rubric](docs/scoring-rubric.md) rather than an overall impression.

See [`docs/structured-interview-guide.md`](docs/structured-interview-guide.md) for the full process — assembling a loop, running each interview, and debriefing.

## What We Assess

A strong Product Manager interview normally looks for evidence across several areas:

- Customer understanding and discovery
- Product judgment, strategy, and prioritization
- Metrics, outcomes, and learning
- Delivery, execution, and ownership
- Influence, collaboration, and communication
- Ethics, self-awareness, and responsible decision-making

No single question can assess all of these well. Use a short, deliberate interview loop with clear ownership across interviewers.

## Repository Status

The [`Questions/`](Questions/) directory is now organized by type:

```text
Questions/
  behavioral/    Past-work evidence
  situational/   Judgment in a realistic future scenario
  judgment/      Trade-offs, ambiguity, and responsible decisions
  method/        Targeted craft or execution questions
  legacy/        Historical prompts retained for context, not a standalone hiring signal
```

All 34 active cards follow the full interview-card structure (question, type, competencies assessed, why it matters, neutral probes, strong evidence, warning signs, scoring anchors) described in [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) and the [interview-card template](Questions/Interview%20Question%20Boilerplate.md). See [`docs/question-index.md`](docs/question-index.md) to find one by type or competency, and [`docs/question-bank-triage.md`](docs/question-bank-triage.md) for how each file was categorized, including the two moved to `Questions/legacy/`.

The research that informed the refresh is in [`Research/`](Research/). It is working material, not yet a publication-ready bibliography — see [`docs/research-audit.md`](docs/research-audit.md) for what still needs citation cleanup before any of it is repeated as fact in public guidance.

See [`docs/competency-model.md`](docs/competency-model.md), [`docs/scoring-rubric.md`](docs/scoring-rubric.md), and [`docs/structured-interview-guide.md`](docs/structured-interview-guide.md) for what to assess, how to score it, and how to run the loop. Optionally, [`docs/interviewer-voices.md`](docs/interviewer-voices.md) offers named interviewer personas for a consistent round style, built on the pressure levels in [`docs/evidence-and-pressure-standard.md`](docs/evidence-and-pressure-standard.md) — read the Candidate Safety Cap there before using anything past the default level.

## Contributing

This repository is in public preview — the best contribution is usage. Try a card in a real interview and report back; see [`docs/field-feedback-guide.md`](docs/field-feedback-guide.md) for what's worth reporting and how. Track progress on the [Field Feedback](https://github.com/users/deanpeters/projects/2) and [Role & Domain Coverage](https://github.com/users/deanpeters/projects/3) boards.

Contributions should make an interviewer more consistent and a candidate experience more respectful. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the full process — how to add or edit a question, what review criteria apply, and how to contribute research responsibly.

- Propose questions that elicit evidence, context, decisions, and learning.
- Explain the competency the question assesses and why it belongs in the process.
- Provide neutral follow-ups and a clear basis for scoring.
- Avoid prompts that depend on trivia, protected characteristics, or conformity to a particular personal style or background.
- Preserve and clearly label legacy material rather than silently removing project history.

The editorial contract for future work lives in [AGENTS.md](AGENTS.md).

## Scope

This is an interviewing aid, not legal guidance or a substitute for interviewer training, a thoughtfully designed hiring process, or human judgment.
