# Research Audit

## Purpose

Per [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md) Phase 4 and `AGENTS.md`'s instruction to replace AI-style citation artifacts with stable, readable links before research is published as factual guidance, this is a status check on the files in [`Research/`](../Research/).

This is a scoped audit — it identifies what needs fixing and why, not a completed source-by-source verification. Resolving it means someone with web access checking each claim against a primary source and replacing the citation, which is future work, not something completed here.

## Findings By File

### `Research/gpt.pm-interview-and-behavioral-questions.md` — Citations resolved

Previously contained 43 inline citation spans using private-use Unicode delimiters around tokens like `citeturn4search8turn4search4` (invisible in normal rendering, which is why they were easy to miss) — leftover artifacts from an AI web-search-grounded generation process that never resolved to a readable link. All 43 have now been replaced with real, checkable markdown links, resolved via direct web search against primary or reputable secondary sources:

- The three hiring-science claims (OPM structured-interview guidance, the Sackett et al. personnel-selection meta-analysis, and Campion, Palmer & Campion's 1997 review of interview structure) now link to opm.gov, the actual Cambridge Core / SIOP sources for Sackett et al., and the Wiley DOI page for Campion et al., respectively.
- The mean operational validity figure was corrected from a bare "about .42" to "around .42 (the 80% credibility interval spans roughly .18 to .66, so this is a central estimate, not a precise figure)" — the original text stated the point estimate without its uncertainty, which risked being read as more precise than the underlying research supports.
- The fourteen book attributions (Cagan, Lin, McDowell & Bavaro, Patton, Haines, Ries, Christensen, Perri, Torres, Dunford, Eyal, Mehta/Agashe/Detroja, Olsen) now link to a publisher page, the author's own site, or a stable bookseller listing for each.
- The claim that Lin's "PM Interview Workbook" was later retitled was checked directly: it's accurate — the workbook became "PM Interview Questions" (2nd edition), a separate book from *Decode and Conquer*. The original sentence didn't claim otherwise, but it's easy to misread that way; the citation now links to the author's own page confirming the relationship.

No claim required correction beyond the validity-figure caveat above, and no citation was left unresolved. The **questions themselves** in this file remain original — the file states they're "synthesized from the literature, not copied from the books" — which is why they were safe to adapt into interview cards in [`docs/core-interview-loop.md`](core-interview-loop.md) even before this cleanup.

### `Research/plex.pm-interview-and-behavioral-questions.md` — Mostly clean

Contains real, resolvable URLs (roughly 38) rather than broken citation tokens. One stray occurrence of the word "cite" appears to be incidental prose, not an artifact. Spot-check a sample of the links for continued validity before treating as a stable public source, but this file does not have the systemic artifact problem `gpt...md` has.

### `Research/gem.Product Management Interview Questions.md` — Mostly clean

Same picture as the plex file: roughly 50 real URLs, one incidental "cite" occurrence, no systemic broken-citation problem. Spot-check link validity before public use.

### `Research/copilot.pm-interview-and-behavioral-questions copy.md` — No citations at all

Contains no citation markers and no URLs. This means its claims currently have **no traceable source attribution whatsoever** — a different problem than broken citations, but still not publication-ready. Any claim drawn from this file for public guidance needs a source added, not just cleaned up. The " copy" in the filename also suggests this may be a duplicate worth checking against the other three before further use.

### `Research/Product Manager Assessment - December 11, 2021.csv` — Different kind of asset, no citation issue

This is a proprietary PM self-assessment worksheet, not AI-synthesized research — it has no citations because it isn't making external claims; it's the worksheet author's own leveling framework (Product Expertise / Practices & Skills / People Skills, each benchmarked 1-5 by role level: PM, Senior PM, Director, VP). Nothing to clean up here, but it should be attributed as an internal source, not presented as an external validated standard, wherever it's used. It directly informed the level-benchmark table in [`docs/interview-scorecard-template.md`](interview-scorecard-template.md) — see that file for how it was adapted (not copied) into this project's six-competency model.

## Recommendation

- `gpt...md`'s citations are resolved — statistics and study attributions from it can now be repeated in public-facing docs (README, competency model, etc.) with a real link behind each claim. Still spot-check a link before leaning on it heavily years from now; publisher and author-site URLs do occasionally move.
- Treat `plex...md` and `gem...md` as closer to usable, pending a link spot-check — that pass hasn't been done yet.
- Treat `copilot...md` as needing sourcing from scratch, or confirm it's a duplicate and can be superseded by one of the other three.
- This audit should be re-run (or the relevant section struck through) if `plex...md` or `gem...md` get the same link-by-link verification `gpt...md` just received — don't let this document go stale and get treated as if cleanup already happened for files it hasn't.
