# Research Audit

## Purpose

Per [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 4 and `AGENTS.md`'s instruction to replace AI-style citation artifacts with stable, readable links before research is published as factual guidance, this is a status check on the four files in [`Research/`](../Research/).

This is a scoped audit — it identifies what needs fixing and why, not a completed source-by-source verification. Resolving it means someone with web access checking each claim against a primary source and replacing the citation, which is future work, not something completed here.

## Findings By File

### `Research/gpt.pm-interview-and-behavioral-questions.md` — Needs cleanup before public use

Contains roughly 30 inline citation markers in the form `citeturnNsearchN` or `citeturnNviewN` (e.g., "a mean operational validity of about .42. citeturn4search5"). These are leftover artifacts from an AI web-search-grounded generation process — they don't resolve to any readable link a reader could click or verify, and they're exactly what `AGENTS.md` flags as unacceptable for public references.

The underlying claims (e.g., OPM structured-interview guidance, the Sackett et al. personnel-selection meta-analysis, points attributed to specific named books like *Inspired* and *The Lean Startup*) are plausible and specific enough to be checkable, which is good — but each one needs its citation marker replaced with an actual stable link (a DOI, publisher page, or reputable summary) before this file's claims should be treated as verified fact rather than a working hypothesis.

The **questions themselves** in this file are original — the file states they're "synthesized from the literature, not copied from the books" — so they were safe to adapt into interview cards in [`docs/core-interview-loop.md`](core-interview-loop.md) without waiting on citation cleanup. It's the *research claims* (statistics, attributions to named studies) that need the citation fix before being repeated as fact in public-facing material like the README or competency model.

### `Research/plex.pm-interview-and-behavioral-questions.md` — Mostly clean

Contains real, resolvable URLs (roughly 38) rather than broken citation tokens. One stray occurrence of the word "cite" appears to be incidental prose, not an artifact. Spot-check a sample of the links for continued validity before treating as a stable public source, but this file does not have the systemic artifact problem `gpt...md` has.

### `Research/gem.Product Management Interview Questions.md` — Mostly clean

Same picture as the plex file: roughly 50 real URLs, one incidental "cite" occurrence, no systemic broken-citation problem. Spot-check link validity before public use.

### `Research/copilot.pm-interview-and-behavioral-questions copy.md` — No citations at all

Contains no citation markers and no URLs. This means its claims currently have **no traceable source attribution whatsoever** — a different problem than broken citations, but still not publication-ready. Any claim drawn from this file for public guidance needs a source added, not just cleaned up. The " copy" in the filename also suggests this may be a duplicate worth checking against the other three before further use.

## Recommendation

- Do not repeat statistics or study attributions from `gpt...md` in public-facing docs (README, competency model, etc.) until the citation markers are replaced with real, checkable links.
- Treat `plex...md` and `gem...md` as closer to usable, pending a link spot-check.
- Treat `copilot...md` as needing sourcing from scratch, or confirm it's a duplicate and can be superseded by one of the other three.
- This audit itself should be re-run (or the relevant section struck through) once someone actually does the link-by-link verification — don't let this document go stale and get treated as if the cleanup already happened.
