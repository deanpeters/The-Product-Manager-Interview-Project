<a id="pminterview"></a>

# The Product Manager Interview Project

[![GitHub stars](https://img.shields.io/github/stars/deanpeters/The-Product-Manager-Interview-Project?style=flat-square)](https://github.com/deanpeters/The-Product-Manager-Interview-Project/stargazers) [![GitHub forks](https://img.shields.io/github/forks/deanpeters/The-Product-Manager-Interview-Project?style=flat-square)](https://github.com/deanpeters/The-Product-Manager-Interview-Project/forks) [![GitHub watchers](https://img.shields.io/github/watchers/deanpeters/The-Product-Manager-Interview-Project?style=flat-square)](https://github.com/deanpeters/The-Product-Manager-Interview-Project/watchers) [![Contributors](https://img.shields.io/github/contributors/deanpeters/The-Product-Manager-Interview-Project?style=flat-square)](https://github.com/deanpeters/The-Product-Manager-Interview-Project/graphs/contributors) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)

[![Status](https://img.shields.io/badge/status-public%20preview-yellow?style=flat-square)](docs/field-feedback-guide.md) ![Interview cards](https://img.shields.io/badge/interview%20cards-49-informational?style=flat-square) [![Last commit](https://img.shields.io/github/last-commit/deanpeters/The-Product-Manager-Interview-Project?style=flat-square)](https://github.com/deanpeters/The-Product-Manager-Interview-Project/commits/master) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey?style=flat-square)](LICENSE)

```text
                                                                               
▄▄▄▄▄▄▄   ▄▄▄      ▄▄▄   ▄▄▄▄▄
███▀▀███▄ ████▄  ▄████    ███         ██                     ▀▀
███▄▄███▀ ███▀████▀███    ███  ████▄ ▀██▀▀ ▄█▀█▄ ████▄ ██ ██ ██  ▄█▀█▄ ██   ██
███▀▀▀▀   ███  ▀▀  ███    ███  ██ ██  ██   ██▄█▀ ██ ▀▀ ██▄██ ██  ██▄█▀ ██ █ ██
███       ███      ███   ▄███▄ ██ ██  ██   ▀█▄▄▄ ██     ▀█▀  ██▄ ▀█▄▄▄  ██▀██
                                                                               

  49 interview cards • 4 core rounds + 2 optional rounds • Public Preview
```

**A ready-to-run interview toolkit that tests product judgment — not memorized frameworks, brainteasers, or a performance of confidence.**

> **Public preview.** This toolkit hasn't been through a formal internal pilot — real usage in real interviews *is* the pilot. Try a card, report what happened, help make it better. See [Report What You Find](#report-what-you-find) below.

---

## Why This Exists

Most PM interview banks are either a pile of unstructured "gotcha" questions, or a single trendy framework dressed up as a full interview process. Neither tells you whether someone can actually do the job: understand customers, make decisions with incomplete information, work through trade-offs, collaborate, learn, and deliver outcomes.

This toolkit is different in three ways:

- **Every card is complete**, not just a prompt — competencies assessed, why it matters, neutral follow-up probes, strong-evidence and warning-sign markers, and scoring anchors. An interviewer can pick it up and run it without inventing anything.
- **Evidence over performance.** The whole system — the [scoring rubric](docs/scoring-rubric.md), the [evidence ladder](docs/evidence-and-pressure-standard.md), the [scorecard](docs/interview-scorecard-template.md) — is built to reward specific, checkable evidence over a confident-sounding story.
- **Organized for a real loop**, not a grab-bag. Cards are grouped into rounds by competency, with worked [role-loop presets](docs/role-loop-presets.md) so assembling a loop isn't a research project.

---

## Get Your First Win

You don't need to read the whole repository before using it. Find your situation below.

| Your situation | Start here |
|---|---|
| **I'm interviewing someone soon and need questions now** | Jump to [Your First 4 Questions](#your-first-4-questions) below, or pick the closest [role-loop preset](docs/role-loop-presets.md) |
| **I know the role but not which cards fit** | Browse [`docs/question-index.md`](docs/question-index.md) by type or competency |
| **I'm hiring across a full loop with multiple interviewers** | Use the [core interview loop](docs/core-interview-loop.md) — assign one round per interviewer |
| **I'm hiring an AI-focused PM** | Read [`docs/ai-competency-model.md`](docs/ai-competency-model.md), then add the optional AI round from the [AI Product PM preset](docs/role-loop-presets.md#preset-ai-product-pm) |
| **I'm hiring a Director or VP** | Use the [Director/VP preset](docs/role-loop-presets.md#preset-director--vp-level-any-domain) layered on top of the domain preset that fits — add the optional [people-management round](docs/people-management-competency.md) only if the role actually manages other PMs |
| **I want to understand the philosophy before I touch anything** | Read [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) and [`AGENTS.md`](AGENTS.md) |
| **I tried a card and something felt off** | See [Report What You Find](#report-what-you-find) below |

### Your First 4 Questions

No preset, no setup — four cards you can ask in your very next interview, one from each core round:

1. **[The Feature That Wasn't the Problem](Questions/behavioral/Feature-That-Wasnt-The-Problem.md)** (Customer Understanding) — tests whether a candidate separates a stakeholder's request from the real underlying problem.
2. **[Deciding Before You're Certain](Questions/judgment/Deciding-Before-Youre-Certain.md)** (Product Judgment) — tests how they reason under incomplete information.
3. **[Influence Without Authority](Questions/behavioral/Influence-Without-Authority.md)** (Collaboration) — tests how they get things done through people they don't manage.
4. **[A Decision You Got Wrong](Questions/behavioral/A-Decision-You-Got-Wrong.md)** (Self-Awareness) — tests real ownership, not a rehearsed success story.

Ask each question as written, use its neutral follow-up probes, and log evidence on the [scorecard template](docs/interview-scorecard-template.md) as you go. That's it — you're running a structured interview.

---

## What We Assess

A strong Product Manager interview normally looks for evidence across several areas:

- Customer understanding and discovery
- Product judgment, strategy, and prioritization
- Metrics, outcomes, and learning
- Delivery, execution, and ownership
- Influence, collaboration, and communication
- Ethics, self-awareness, and responsible decision-making

No single question can assess all of these well. Use a short, deliberate interview loop with clear ownership across interviewers — see [`docs/competency-model.md`](docs/competency-model.md) for what each one means, [`docs/ai-competency-model.md`](docs/ai-competency-model.md) for the optional AI-specific layer, and [`docs/people-management-competency.md`](docs/people-management-competency.md) for the optional manager-track layer.

## How It's Organized

```text
Questions/
  behavioral/    Past-work evidence
  situational/   Judgment in a realistic future scenario
  judgment/      Trade-offs, ambiguity, and responsible decisions
  method/        Targeted craft or execution questions
  ai/            Optional AI-competency layer, AI-heavy roles only (domain-based, not format-based)
  people-management/  Optional layer for manager-track roles only (domain-based, not format-based)
  legacy/        Historical prompts retained for context, not a standalone hiring signal
```

All 49 active cards follow the full interview-card structure (question, type, competencies assessed, why it matters, neutral probes, strong evidence, warning signs, scoring anchors) described in [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) and the [interview-card template](Questions/Interview%20Question%20Boilerplate.md). See [`docs/question-index.md`](docs/question-index.md) to find one by type or competency, and [`docs/question-bank-triage.md`](docs/question-bank-triage.md) for how each file was categorized, including the two moved to `Questions/legacy/`.

The research that informed the refresh is in [`Research/`](Research/). It is working material, not yet a publication-ready bibliography — see [`docs/research-audit.md`](docs/research-audit.md) for what still needs citation cleanup before any of it is repeated as fact in public guidance.

See [`docs/competency-model.md`](docs/competency-model.md), [`docs/scoring-rubric.md`](docs/scoring-rubric.md), and [`docs/structured-interview-guide.md`](docs/structured-interview-guide.md) for what to assess, how to score it, and how to run the loop. Optionally, [`docs/interviewer-voices.md`](docs/interviewer-voices.md) offers named interviewer personas for a consistent round style, built on the pressure levels in [`docs/evidence-and-pressure-standard.md`](docs/evidence-and-pressure-standard.md) — read the Candidate Safety Cap there before using anything past the default level. [`docs/negotiation-signals.md`](docs/negotiation-signals.md) names specific Voss/Ury negotiation techniques worth listening for (not asking about) on the stakeholder-pressure cards.

## Report What You Find

This repository is in public preview — the best contribution is usage. Try a card in a real interview and report back; see [`docs/field-feedback-guide.md`](docs/field-feedback-guide.md) for what's worth reporting and how. Track progress on the [Field Feedback](https://github.com/users/deanpeters/projects/2) and [Role & Domain Coverage](https://github.com/users/deanpeters/projects/3) boards.

## Contributing

Contributions should make an interviewer more consistent and a candidate experience more respectful. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the full process — how to add or edit a question, what review criteria apply, and how to contribute research responsibly.

- Propose questions that elicit evidence, context, decisions, and learning.
- Explain the competency the question assesses and why it belongs in the process.
- Provide neutral follow-ups and a clear basis for scoring.
- Avoid prompts that depend on trivia, protected characteristics, or conformity to a particular personal style or background.
- Preserve and clearly label legacy material rather than silently removing project history.

The editorial contract for future work lives in [AGENTS.md](AGENTS.md).

## License

[CC BY-NC-SA 4.0](LICENSE) — non-commercial use with share-alike.

**Everything in this repository — every question card, template, and doc — is licensed CC BY-NC-SA 4.0. There is no mix of licenses here.**

Several cards' Attributions sections note they were adapted from the same author's other private tooling and research (decision-review practice, an AI-PM training curriculum, a market-sizing prompt loop) or from public frameworks (the MITRE Innovation Toolkit's Premortem technique). Same-author adaptations carry no license conflict — a license grants permissions to *other* people, and a copyright holder is free to adapt and relicense their own work. Those Attributions lines are lineage — a breadcrumb back to where an idea started — not a license dependency.

**In plain terms:**

- ✅ **Use this toolkit in your day job** — running interviews, training other interviewers, adapting cards for your team. That's what it's for.
- ✅ **Adapt and remix it** — share what you build under this same license, with credit.
- ✅ **Teach with it** — interviewer training, calibration sessions, sending the ladder down.
- ❌ **Don't sell it** — no repackaging this toolkit itself into a paid product, course, or service without expressed written permission.
- 🤔 **Not sure your use qualifies?** [Open an issue](https://github.com/deanpeters/The-Product-Manager-Interview-Project/issues) and ask. If you're using this in the spirit it was built — to run fairer, more consistent interviews — the answer is almost certainly yes.

## Scope

This is an interviewing aid, not legal guidance or a substitute for interviewer training, a thoughtfully designed hiring process, or human judgment.
