# AGENTS.md

## Project Purpose

This repository is a practical toolkit for structured Product Manager interviews. Its primary purpose is to help interviewers assess product judgment in context, not framework recall, trivia, or cleverness under pressure.

The source of truth for the intended direction is [`docs/MODERNIZATION-PLAN.md`](docs/MODERNIZATION-PLAN.md). Read it before making substantive editorial or structural changes.

## Read First

Before editing, inspect:

1. `README.md` for the public promise and repository orientation.
2. `docs/HANDOFF.md` for the current state, recent decisions, branch/protection notes, and next suggested work.
3. `docs/MODERNIZATION-PLAN.md` for the roadmap, phase history, and the standing backlog of not-yet-mined sources.
4. `Interview Question Style Guide.md` and `Questions/Interview Question Boilerplate.md` for the current authoring conventions.
5. `docs/question-index.md` and `docs/question-bank-triage.md` to see what already exists before proposing a new card — most "new" ideas turn out to be a rephrasing of something already in the bank. `docs/core-interview-loop.md` shows how cards assemble into a runnable loop, and `docs/role-loop-presets.md` shows that worked for specific role shapes.
6. Relevant files in `Research/` when adding or changing claims about interviewing practice — and see `docs/research-audit.md` for what's already been checked and how each source was attributed.

## Repository Shape (for a new agent picking this up cold)

- `Questions/behavioral/`, `situational/`, `judgment/`, `method/` — format-based folders, the core (non-optional) bank.
- `Questions/ai/` and `Questions/people-management/` — domain-based folders, peers to the format folders rather than nested inside them. Each card in these still records its own format Type internally. Both are optional layers — only relevant for AI-heavy or manager-track roles respectively; see `docs/ai-competency-model.md` and `docs/people-management-competency.md`.
- `Questions/systems-thinking/` — problem-breakdown, systems-mapping, and Precedents Thinking candidates. These are not part of the active 58-card bank until rewritten as full cards; see `docs/systems-thinking-exercises.md`.
- `docs/` — the full editorial and operational apparatus: handoff state, competency models (core, AI, people-management), the scoring rubric, the evidence/pressure standard, interviewer voices, negotiation signals, the scorecard template, the core interview loop, role-loop presets, the question index, the triage history, the research audit, and this roadmap. Skim `docs/question-index.md`'s "Purpose" line for how they all connect — most docs cross-link the others rather than repeating content.
- Every doc that states a card count (`README.md`, `docs/core-interview-loop.md`, `docs/role-loop-presets.md`, `docs/question-index.md`, `docs/question-bank-triage.md`) must be updated together whenever a card is added, moved, or retired — they're expected to agree. Run the relative-link check described in Verification below before committing, since a missed rename or move breaks a link silently otherwise.

## Editorial Principles

- Favor behavioral, situational, and judgment questions that invite evidence and reasoning.
- Assess decisions, trade-offs, collaboration, customer understanding, learning, and outcomes.
- Make every question usable by an interviewer: include purpose, neutral probes, positive and warning signals, and scoring guidance.
- Reward specific evidence and clear reasoning, not polished framework recitation.
- Use plain language. The audience includes experienced interviewers, Product Managers, hiring managers, and people learning to interview.
- Preserve memorable project language when it carries real meaning. Do not sand off sharp Deanisms, named phrases, or sticky triads such as `Build / Borrow / Buy` or `Pivot / Punt / Pursue` into blander synonyms unless the phrase is confusing or inaccurate.
- Separate validated claims from recommendations or hypotheses. Do not turn research synthesis into an unsupported fact.
- Use stable, readable sources when publishing research-backed assertions. AI-generated citation artifacts are not acceptable public references.

## Question Standards

New or substantially rewritten question files should use the interview-card structure:

1. Question
2. Type
3. Competencies assessed
4. Why this matters
5. Neutral follow-up probes
6. Strong evidence
7. Warning signs
8. Scoring anchors
9. Role or level notes, only when needed

Questions should not assess protected characteristics, personal circumstances, cultural conformity, company trivia, or an arbitrary preferred background.

Avoid using brainteasers, abstract design exercises, and market-sizing puzzles as primary hiring signals unless the role calls for that skill and the question has a clear scoring rubric.

## Repository Care

- Preserve historical questions; move or label them as systems-thinking candidates or background context instead of deleting them without explicit direction.
- Keep changes focused. Do not rewrite the full bank in a cosmetic pass.
- Keep Markdown readable in plain text and on GitHub.
- Do not add dependencies, build tooling, or automation unless there is a concrete maintenance or user benefit.
- Do not commit changes unless explicitly asked.
- The GitHub default branch is `master` and is protected by ruleset. Publish through a feature branch and PR; do not assume a `main` branch exists.

## Verification

For documentation changes, check that internal links resolve, headings are consistent, and the README gives a newcomer a clear starting path. For question changes, check that the card can be asked, probed, and scored without unstated interviewer assumptions.

Before committing, check every relative Markdown link in the repo actually resolves — this has caught real breakage after folder moves and renames in the past. A minimal check (run from the repo root):

```python
import re, os, urllib.parse

for dirpath, _, filenames in os.walk("."):
    if ".git" in dirpath:
        continue
    for fn in filenames:
        if not fn.endswith(".md"):
            continue
        path = os.path.join(dirpath, fn)
        text = open(path, encoding="utf-8", errors="ignore").read()
        for m in re.finditer(r'\[[^\]]*\]\(([^)]+)\)', text):
            link = m.group(1)
            if link.startswith(("http", "#", "mailto:")):
                continue
            target = link.split("#")[0]
            if not target:
                continue
            full = os.path.normpath(os.path.join(dirpath, urllib.parse.unquote(target)))
            if not os.path.exists(full):
                print(f"BROKEN: {path} -> {link}")
```

## Adding A New Card

The recurring pattern for adding one or more cards, in order:

1. Write the card(s) in the interview-card structure (see Question Standards above), in the format-appropriate folder — `Questions/ai/` or `Questions/people-management/` if it's one of those domain layers, otherwise the folder matching its Type.
2. Update `docs/question-index.md` — By Type, By Core Competency (every competency the card names, not just the primary one), and By AI/People-Management Competency if relevant. Update the Coverage Status paragraph.
3. Update `docs/core-interview-loop.md` — add the card to its round, update the bank-size numbers in the Purpose line and "Do Not Ask All N" heading, and update the Coverage Note.
4. Update `docs/question-bank-triage.md` — add a paragraph describing what was added and why, and update the final "active bank is now N cards" line.
5. Update `docs/role-loop-presets.md` if the card is a natural fit for one of the four presets (as a swap-in note is usually enough, not a rewrite).
6. Update `README.md`'s badge, ASCII banner stat line, and "All N active cards" sentence.
7. If the card is adapted from a source in `Research/` or from an external local checkout, add or extend an entry in `docs/research-audit.md`; if the card cites something outside `Research/` proper, note in that entry that the source lives elsewhere. Never cite a private/unpublished local path directly in a card's own Attributions section — describe the practice instead, or use a real public link if the source is genuinely published (see the Provenance and Attribution rule in `CONTRIBUTING.md`).
8. Run the link check above, then stage and commit.
