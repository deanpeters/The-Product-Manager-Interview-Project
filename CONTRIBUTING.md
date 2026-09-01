# Contributing

Thanks for considering a contribution to this Product Manager interview toolkit. This guide is the practical, contributor-facing companion to [`AGENTS.md`](AGENTS.md), which remains the source of truth for editorial standards — read it first if there's ever a conflict between the two.

## Before You Start

1. Read [`README.md`](README.md) for the project's purpose and current structure.
2. Read [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) for the roadmap and how existing material is being treated.
3. Read [`docs/competency-model.md`](docs/competency-model.md) so any new question maps to a real, named competency rather than inventing one.
4. Browse [`docs/question-index.md`](docs/question-index.md) to see what's already covered — and, more usefully, what isn't. A new question that fills a genuine gap is more valuable than a fourth question testing the same thing three existing cards already test well.

## Contributing A New Question

1. Copy [`Questions/Interview Question Boilerplate.md`](Questions/Interview%20Question%20Boilerplate.md) into the correct type folder: `behavioral/`, `situational/`, `judgment/`, or `method/`. See `docs/MODERNIZATION-PLAN.md` for what distinguishes each type.
2. Fill in every section — Type, Competencies Assessed, Why This Matters, Neutral Follow-Up Probes, Strong Evidence, Warning Signs, Scoring Anchors. A card missing any of these isn't ready for review.
3. Name one to three competencies from `docs/competency-model.md`. If your question doesn't map cleanly to any of them, that's a sign either the question needs rework or the competency model itself is incomplete — raise the latter as its own discussion rather than forcing a fit.
4. Write neutral follow-up probes. A probe that hints at the "right" answer defeats the purpose — see the probe examples in `docs/structured-interview-guide.md` and the existing cards in `Questions/behavioral/` and `Questions/judgment/` for the tone to match.
5. Avoid the disqualified categories from `AGENTS.md`: protected characteristics, personal circumstances, cultural conformity, company trivia, or an arbitrary preferred background. Avoid brainteasers, abstract design exercises, and market-sizing puzzles as primary hiring signals unless the role specifically calls for that skill and you've written a clear scoring rubric for it — see `Questions/legacy/` for examples of prompts that didn't clear this bar.
6. Add attributions for anything you didn't originate yourself. Do not submit copyrighted content without permission, and no self-promotion.
7. Update [`docs/question-index.md`](docs/question-index.md) with your new card, under both its type and its competency section.

## Editing An Existing Question

- Keep changes focused on the specific problem you're fixing. Don't use a small fix as an excuse to rewrite the whole card.
- If you're moving a card between `Questions/` type folders (e.g., promoting something out of `legacy/`), update `docs/question-bank-triage.md` and `docs/question-index.md` to match, and explain why in your PR description.
- Never silently delete historical material. If a question should be retired, propose moving it to `Questions/legacy/` with a short context note instead, per `AGENTS.md`.

## Contributing Research

- New material in `Research/` should be treated as a working synthesis, not a finished bibliography — see `AGENTS.md` and [`docs/research-audit.md`](docs/research-audit.md) for what "not ready for public use" looks like in practice (mainly: unresolved AI-generated citation artifacts, or claims with no traceable source at all).
- If you're citing a study, statistic, or claim from a named book, link to something a reader can actually check — a DOI, publisher page, or reputable summary. Don't leave placeholder or broken citation markers in anything intended for public-facing use.

## Review Criteria

A submission is ready for review when:

- It follows the interview-card structure completely (for new questions), or clearly explains the specific problem being fixed (for edits).
- Every named competency traces to `docs/competency-model.md`.
- Neutral follow-up probes exist and don't leak the "correct" answer.
- Strong evidence and warning signs are concrete and observable, not vague ("shows good judgment") — a reviewer should be able to picture the actual interview moment being described.
- Attributions are present and accurate; nothing looks copied without credit.
- It doesn't duplicate an existing, well-covered competency without a clear reason.

## Verification Before Submitting

- Confirm any internal links you added or changed actually resolve (relative paths from the file's own location, not the repo root).
- Confirm headings are consistent with the interview-card template.
- Ask yourself: could a new interviewer pick up this card and run it — ask it, probe it, and score it — without having to guess at anything you didn't write down? If not, it's not done yet.

## Questions

If something in this guide conflicts with `AGENTS.md`, `AGENTS.md` wins — open an issue or note the discrepancy so this file can be corrected.
