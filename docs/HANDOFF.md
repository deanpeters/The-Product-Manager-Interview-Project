# Handoff

## Current State

This repository is a public-preview toolkit for structured Product Manager interviews. The active interview bank remains 58 cards: 36 core cards, 18 optional AI-competency cards, and 4 optional people-management cards. `Questions/systems-thinking/` is a separate candidate lane and is not included in the active-card count unless a later promotion decision updates the README, index, core loop, role presets, and triage docs together.

The default GitHub branch is currently `master`, not `main`. A ruleset protects the default branch, so direct pushes to `master` are blocked. Use a feature branch and pull request for publishable changes.

## Recent Decisions

- `Questions/systems-thinking/` replaced the old generic historical bucket and now holds five systems-thinking candidates.
- Two older prompts were reframed into full systems-thinking cards while keeping their original file paths stable: `Number-of-Pianos.md` is now **Model the Facility Before You Count**, and `ProductDesign-VendingMachine.md` is now **Map the Vending Machine System**.
- The AI sourcing card must use the memorable terminology **Build / Borrow / Buy** in that order.
- In this project, `borrow` means using a third-party cloud service or hosted capability; `buy` means acquiring or purchasing the capability outright.
- **Build / Borrow / Buy** is not the same decision family as `Pivot / Punt / Pursue` or `Pivot / Punt / Pursue / Pause`; do not blend those vocabularies.
- Memorable Deanisms and named phrases are part of the teaching system when they carry meaning. Preserve them unless they are confusing or inaccurate.

## What We Learned

The earlier AI cards are structurally sound, but some are too polite. They often read as normal Product Manager judgment cards with AI vocabulary added. Dean's Substack material has sharper lessons that should drive the next editorial pass:

- AI multiplies the thinking it is pointed at; weak problem definition becomes faster, cleaner-looking failure.
- Tool strategy has a short half-life; durable judgment matters more than today's stack.
- Context is shared infrastructure, not private prompt craft.
- Agents require journey maps, decision gates, logs, and accountability before production.
- Evals are product judgment: thresholds, traces, failure cases, and decision rules, not model beauty contests.
- AI investments need named economic or operating levers, not activity theater.

## Next Suggested Work

Run a focused AI-card hardening pass from `origin/master` after any open PRs you need have landed. Start with these cards:

- `Questions/ai/Where-AI-Actually-Helps.md` — sharpen around leverage before agentifying.
- `Questions/ai/Testing-an-AI-Idea-Before-Its-Real.md` — sharpen around tiny bets before large assumptions.
- `Questions/ai/When-the-Model-Is-Wrong.md` — rewrite around eval thresholds, traces, and decision rules.
- `Questions/ai/Governing-an-Agent-That-Acts-on-Its-Own.md` — rewrite around agent journey maps, gates, logs, and accountability.
- `Questions/ai/What-the-Model-Needs-to-Know.md` — deepen from data/context gap to shared reality layer.
- `Questions/ai/Build-Borrow-Buy.md` — keep the sourcing vocabulary exact and sharpen around durable tradeoff judgment.

Use `/Users/deanpeters/Code/15-days-of-aipm/substack/deanpeters.substack.com` as source material for that pass. The strongest files to start with are:

- `day-02---the-ai-pm-skills-nobody-teaches.md`
- `day-03---stop-solving-the-wrong-problem.md`
- `day-05---context-engineering-is-a-team-sport.md`
- `day-10---your-agents-are-running-feral.md`
- `day-11---build-agents-that-dont-go-rogue.md`
- `ai-evals-are-not-model-beauty-pageants.md`
- `agentic-tool-tourism-is-not-a-strategy.md`
- `ai-first-is-cute-ai-shaped-is-survival-5-ai-pm-skills-2026.md`

## Verification Pattern

Before opening or merging a PR, run:

```bash
git diff --check
```

Run the relative Markdown link check from `AGENTS.md`. Also spot-check any renamed card in `docs/question-index.md`, `docs/core-interview-loop.md`, `docs/role-loop-presets.md`, `docs/question-bank-triage.md`, and any card that mentions it by name.
