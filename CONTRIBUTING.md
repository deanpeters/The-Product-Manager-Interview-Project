# Contributing to The Product Manager Interview Project

Thanks for your interest in contributing! This repository helps interviewers run structured, evidence-based Product Manager interviews by providing complete, ready-to-use interview cards.

This guide is the practical, contributor-facing companion to [`AGENTS.md`](AGENTS.md), which remains the source of truth for editorial standards — read it first if there's ever a conflict between the two.

---

## Design Philosophy — Read This First

This repository exists to test **product judgment in context**, not framework recall, trivia, or a performance of confidence. Every card should:

- Elicit specific evidence, not a rehearsed answer
- Name the competency it assesses and why that competency matters for the job
- Give an interviewer neutral probes, strong-evidence and warning-sign markers, and scoring anchors — not just a clever question
- Leave the interviewer with better judgment about the candidate, not just a transcript

**The most common contribution mistake:** writing a question that's fun to ask but has no real scoring signal behind it. A market-sizing puzzle or an open-ended "design an X" prompt might feel clever; without a defensible rubric it belongs outside the active bank. If the prompt is really about decomposing a system, modeling an unfamiliar domain, or learning from precedents, it may belong in [`Questions/systems-thinking/`](Questions/systems-thinking/) as a candidate exercise; see [`docs/systems-thinking-exercises.md`](docs/systems-thinking-exercises.md).

---

## Who Can Contribute?

**Anyone!** You don't need to be a hiring manager. If you:

- Have run an interview and found a question that reliably surfaces real signal
- Spotted an ambiguity or gap in an existing card
- Want to improve a probe, a warning sign, or a scoring anchor
- Have feedback from actually using the [core interview loop](docs/core-interview-loop.md) — see [`docs/field-feedback-guide.md`](docs/field-feedback-guide.md)

...then you can contribute.

---

## What Can You Contribute?

### 1. New Interview Cards

Have a question that reliably surfaces real judgment? Submit it.

**Examples of good candidates:**
- A behavioral question you've asked repeatedly that reliably separates strong and weak answers
- A judgment scenario tied to a real decision type (a trade-off, a business case, a risk call)
- A card that fills a gap in [`docs/question-index.md`](docs/question-index.md)'s coverage

**Not a good fit:**
- One-off trivia or a "gotcha" question with no real evidence signal
- Company-specific or product-specific questions (cards should be broadly usable)
- Brainteasers or abstract design exercises without a defensible scoring rubric

### 2. Improvements To Existing Cards

Found something unclear? A probe that leaks the answer? An anchor that's ambiguous?

**Good improvements:**
- Sharpen a Strong Evidence or Warning Signs bullet so it matches what a real answer actually looks like
- Add a Role Or Level Notes section for senior candidates
- Fix a broken link or an inaccurate attribution

**Please avoid:**
- Softening scoring anchors into vague generalities ("shows good judgment")
- Adding filler explanation that doesn't change what an interviewer would actually do
- Changing the card's core structure (every card follows the same interview-card template)

### 3. Feedback & Suggestions

Not ready to write a full card? Share what you found using this in a real interview — see [`docs/field-feedback-guide.md`](docs/field-feedback-guide.md) for what's worth reporting. Open an issue using the **Field Feedback** template and we'll discuss.

---

## How To Contribute (Step-By-Step)

### For Non-Technical Contributors (No GitHub Experience Required)

**Option 1: Open a GitHub Issue**
1. Go to the [Issues tab](https://github.com/deanpeters/The-Product-Manager-Interview-Project/issues)
2. Click "New Issue" and pick the **Field Feedback** template for reporting friction, or a plain issue for proposing a new card
3. Describe your suggestion — for a new card: what's the question, what does it assess, when did it work well for you? For feedback: which card, what happened, what would you change?
4. Submit — we'll follow up

**Option 2: Track progress**
See the [Field Feedback](https://github.com/users/deanpeters/projects/2) and [Role & Domain Coverage](https://github.com/users/deanpeters/projects/3) boards for what's already been reported and what's being worked on.

### For Technical Contributors (Comfortable With GitHub)

1. **Fork this repository**
2. **Clone your fork:**
   ```bash
   git clone https://github.com/YOUR-USERNAME/The-Product-Manager-Interview-Project.git
   cd The-Product-Manager-Interview-Project
   ```
3. **Create a new branch:**
   ```bash
   git checkout -b add-card-name
   ```
4. **Before You Start:**
   - Read [`README.md`](README.md) for the project's purpose and structure.
   - Read [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) for the roadmap and how existing material is treated.
   - Read [`docs/competency-model.md`](docs/competency-model.md) so any new question maps to a real, named competency rather than inventing one.
   - Browse [`docs/question-index.md`](docs/question-index.md) to see what's already covered — a card that fills a genuine gap is worth more than a fourth card testing something three cards already cover well.
5. **Make your changes** (see Interview Card Format below)
6. **Commit and push:**
   ```bash
   git add .
   git commit -m "Add [card-name] card"
   git push origin add-card-name
   ```
7. **Submit a pull request.** We'll review within a week and provide feedback.

---

## Interview Card Format (Required Structure)

Copy [`Questions/Interview Question Boilerplate.md`](Questions/Interview%20Question%20Boilerplate.md) into the correct type folder: `behavioral/`, `situational/`, `judgment/`, or `method/`. See [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md) for what distinguishes each type. If the card requires AI to be a real part of the product surface (see [`docs/ai-competency-model.md`](docs/ai-competency-model.md)), put it in `ai/` instead — a domain-based folder, not a format-based one — and still fill in the card's own Type field as normal.

**Non-negotiable sections**, every card:

- The question and its type
- Competencies Assessed (one to three, from [`docs/competency-model.md`](docs/competency-model.md); add an AI Competency line only if it also applies to [`docs/ai-competency-model.md`](docs/ai-competency-model.md))
- Why This Matters
- Neutral Follow-Up Probes
- Strong Evidence
- Warning Signs
- Scoring Anchors

**Optional sections:** Role Or Level Notes, Additional Reading.

**Naming:** filenames should describe the question's content, not a contributor's handle or a company name — the card belongs to the toolkit once merged.

---

## Provenance and Attribution

Cards earn trust by citing their sources honestly. But an attribution can itself disclose something it shouldn't, so there is one rule:

**Cite public, linkable work by name. For unpublished internal or private material, cite the practice or the framework shape — not the artifact or its file path.**

**Cite freely, with a link:**
- Published books, articles, research papers, and their named authors
- Public repositories, blog posts, and talks

**Never name:**
- Private training material, internal playbooks, or unpublished compendia
- Company or client names, even pseudonymized — a placeholder still signals a real engagement
- Local file paths on anyone's machine

Write "Adapted from a private [X] practice" or "Adapted from practitioner experience running [the technique]" instead. It's true, useful, and points at nothing that can't be independently verified by a reader.

---

## Contributing Research

- New material in [`Research/`](Research/) should be treated as a working synthesis, not a finished bibliography — see [`docs/research-audit.md`](docs/research-audit.md) for what "not ready for public use" looks like in practice.
- If you're citing a study, statistic, or claim from a named book, link to something a reader can actually check — a DOI, publisher page, or reputable summary. Don't leave placeholder or broken citation markers in anything intended for public-facing use.

---

## Quality Checklist (Before Submitting)

Your card should pass these checks:

- [ ] **Judgment-tested, not framework-tested:** Does it reward specific evidence and reasoning over reciting a memorized framework?
- [ ] **Self-contained:** Could a new interviewer pick it up and run it — ask it, probe it, score it — without guessing at anything you didn't write down?
- [ ] **Competency-mapped:** Does every named competency trace to `docs/competency-model.md` (or `docs/ai-competency-model.md` for an AI card)?
- [ ] **Neutral probes:** Do the follow-up probes avoid leaking the "correct" answer?
- [ ] **Concrete anchors:** Are Strong Evidence and Warning Signs specific and observable, not vague ("shows good judgment")?
- [ ] **Attributed correctly:** See Provenance and Attribution above — nothing looks copied without credit, and no private material or local file path is named.
- [ ] **Not a duplicate:** Does it fill a genuine gap rather than re-testing something three existing cards already cover well?
- [ ] **Links resolve:** Any internal links you added or changed actually resolve (relative paths from the file's own location, not the repo root).
- [ ] **Index updated:** Is [`docs/question-index.md`](docs/question-index.md) updated with your new card, under both its type and its competency?

---

## Writing Style Guide

### Do This:
- Write like you're briefing an experienced colleague, not a junior intern
- Use short sentences and active voice
- Name trade-offs, not just "best practices"
- Make Strong Evidence and Warning Signs concrete enough that two interviewers would score the same answer the same way

### Don't Do This:
- Use filler phrases ("It's important to note...")
- Moralize or preach ("Candidates MUST always...")
- Hedge excessively ("This might potentially indicate...")
- Assume shared context — define any competency or term a new interviewer might not already know

**Tone:** Professional but plain. Clear over clever.

---

## Editing An Existing Card

- Keep changes focused on the specific problem you're fixing. Don't use a small fix as an excuse to rewrite the whole card.
- If you're moving a card between `Questions/` type folders (e.g., promoting something out of `systems-thinking/`), update `docs/question-bank-triage.md` and `docs/question-index.md` to match, and explain why in your PR description.
- Never silently delete historical material. If a question should leave the active bank, propose moving it to `Questions/systems-thinking/` only when it has a real problem-breakdown purpose; otherwise label it as background context in the relevant doc, per `AGENTS.md`.

---

## Review Process

**What happens after you submit:**

1. **We review within 7 days** — checking whether it follows the card structure, maps to a real competency, and would actually work in a live interview.
2. **We provide feedback** — if approved, merged; if changes are needed, we'll suggest edits; if it's not a fit, we'll explain why.
3. **You get credit** — your attribution stays in the card's history, and significant contributions get a mention in the repository's activity.

---

## What We're Looking For

**High-priority:** cards that close a real gap in [`docs/question-index.md`](docs/question-index.md)'s coverage; sharper Strong Evidence / Warning Signs language on existing cards, informed by actual interview use.

**Medium-priority:** additional Role Or Level Notes for senior candidates; cross-references between related cards.

**Low-priority:** pure reformatting (cards already follow the standard structure) unless clarity is meaningfully improved.

## What We Won't Accept

- Questions about protected characteristics, personal circumstances, cultural conformity, or an arbitrary preferred background
- Brainteasers, market-sizing puzzles, or abstract design exercises without a defensible scoring rubric (see [`Questions/systems-thinking/`](Questions/systems-thinking/) for examples that need a stronger systems-thinking rubric before active use)
- Company-specific or product-specific trivia
- Duplicate content — check [`docs/question-index.md`](docs/question-index.md) first
- Self-promotion or copyrighted content submitted without permission
- Attribution that names private material or a local file path — see Provenance and Attribution above

---

## Questions?

If something in this guide conflicts with `AGENTS.md`, `AGENTS.md` wins — open an issue or note the discrepancy so this file can be corrected.

Not sure if your idea fits? Open an issue and describe it — we'll let you know if it's a good candidate.

---

## License Note

By contributing, you agree that your contributions will be licensed under the **CC BY-NC-SA 4.0** license (same as this repository) — see [`LICENSE`](LICENSE) and the License section of [`README.md`](README.md).

---

**Thank you for making this toolkit better!** Every contribution helps interviewers assess product judgment more fairly and consistently.
