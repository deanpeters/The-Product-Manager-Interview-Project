# Field Feedback Guide

## Purpose

This repository is in public preview. Instead of a controlled pilot with recruited interviewers, the plan is simpler: real people use the [core interview loop](core-interview-loop.md) in real interviews, and report back what worked and what didn't. This guide is that on-ramp — how to try a card, what to capture, and how to send it back so it actually improves the bank rather than staying a private observation.

This replaces an earlier, heavier "controlled pilot" checklist that assumed recruiting interviewers and coordinating sessions. That model doesn't fit a public-preview project — open usage in the wild is the pilot now.

## If You're Trying This In A Real Interview

1. **Pick a [role-loop preset](role-loop-presets.md)** that's close to the role you're hiring for, or hand-select questions from the [question index](question-index.md).
2. **Use the [scoring rubric](scoring-rubric.md) and [scorecard template](interview-scorecard-template.md)** as written — the feedback that matters most is whether they work as documented, not a modified version.
3. **Note friction as it happens**, not after the fact: a question that landed oddly, a follow-up probe that didn't get you anywhere, a warning sign that didn't show up the way the card predicted, timing that ran long or short. A note taken in the moment beats a reconstructed memory a week later.

## What's Worth Reporting

Not everything needs a report — a single so-so answer from one candidate isn't a pattern. Report when:

- **The same card creates confusion across more than one interview or interviewer** — that's a signal about the card, not the candidate.
- **A card's Strong Evidence or Warning Signs section doesn't match what a real answer actually looks like** in practice.
- **Two interviewers score the same answer noticeably differently** — see [scoring-rubric.md](scoring-rubric.md)'s Calibration section for how to tell whether that's the question's fault, the rubric's fault, or just uncalibrated interviewers (the fix differs for each, so say which you think it is if you have a view).
- **A role-loop preset's weighting felt wrong** for the role it claims to fit.
- **Something in the AI-competency layer, the evidence-and-pressure standard, or any other doc didn't hold up** when actually used, not just read.

## How To Report It

Open a GitHub issue on this repository using the **Field Feedback** template. It'll prompt for the same fields below:

- **Which card or doc**, linked directly.
- **What happened** — the specific friction, not a general impression.
- **What you'd change**, if you have a view — a rewritten Strong Evidence bullet, a different follow-up probe, a different competency mapping. Concrete beats vague.
- **Context that matters**: role, seniority level, how many times you've now seen this same issue.

See [`CONTRIBUTING.md`](../CONTRIBUTING.md) for how feedback turns into an actual edit — the short version is: a card gets fixed directly (not just noted), and [question-bank-triage.md](question-bank-triage.md) and [question-index.md](question-index.md) get updated if a card's disposition changes.

Track what's been reported and what's being worked on: [Field Feedback board](https://github.com/users/deanpeters/projects/2). If your feedback is about adding coverage for a specific role or domain rather than fixing something existing, that's tracked separately on the [Role & Domain Coverage board](https://github.com/users/deanpeters/projects/3).

## What This Isn't

This isn't a substitute for the discipline in [structured-interview-guide.md](structured-interview-guide.md) — consistent questions, neutral probes, independent scoring before debrief all still apply in a real interview, public-preview or not. Field feedback improves the toolkit; it doesn't relax how any single interview should be run.

## What "Working" Looks Like

Per [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md)'s Definition of Done: a new interviewer can select a role-appropriate loop, ask each question consistently, record evidence, score it against shared anchors, and understand why a question belongs in the process — without inferring the philosophy from scratch. If field usage keeps turning up the same friction points, that's evidence something still isn't there yet, and worth fixing directly rather than treating as an isolated complaint.
