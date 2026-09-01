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

### `Research/plex.pm-interview-and-behavioral-questions.md` — Link check complete

All 38 reference URLs checked directly (HTTP status, with a Wayback Machine lookup for anything that failed). Result:

- 34 resolve normally (200).
- 1 (reference 8, a Decode and Conquer PDF) returned 404 at its original URL; replaced in the file with a working Wayback Machine snapshot of the same source (dated 2023-09-24), noted inline.
- 3 are flagged inline with `<!-- DEAD LINK -->` comments rather than silently fixed, since no working replacement or archive exists: reference 4 (pminterviewcopilot.com, backing several footnoted claims — treat those specific footnotes as currently unsourced), reference 22 and reference 32 (both dead, but each backs a claim already covered by a still-live reference elsewhere in the same file — 20 and 1, respectively — so no content is left completely unsourced).
- 1 (reference 13, supersummary.com) returned HTTP 429 (rate-limited) rather than a clear pass or fail; likely a live site blocking automated requests, not confirmed dead — left as-is, worth a manual check if leaned on heavily.

No content changed beyond the citation fixes above. Safe to treat as a stable source with the four caveats above.

### `Research/gem.Product Management Interview Questions.md` — Link check complete, with a separate structural caveat

All 25 works-cited URLs checked directly. 23 resolve normally (200); 2 (both `medium.com` links) returned 403 in both a direct request and a WebFetch retry — Medium blocks most non-browser traffic including this, so this is inconclusive rather than confirmed dead, and neither was flagged or altered.

**Separate finding, not fixed here:** this file's inline citation markers (superscript numbers like "value creation5") appear to reuse the same reference number across multiple, unrelated claims in several places, rather than each number mapping cleanly to one claim. That's a citation-integrity problem distinct from link validity — a reader can't always tell which specific works-cited entry backs a specific sentence. Fixing it would mean re-mapping every inline number against its actual source, which is a larger remapping task than this pass covered; flagging it here so it isn't mistaken for "fully audited" the way `gpt...md` now is.

### `Research/copilot.pm-interview-and-behavioral-questions copy.md` — Confirmed not a duplicate; no citations needed

Read in full. It is **not** a duplicate of `gpt...md`, `plex...md`, or `gem...md` — those three are narrative research syntheses citing named books and studies; this file is a self-contained, original 100-question tabular bank with its own competency-weighting model and no book citations or external statistics anywhere in it. The " copy" in the filename appears to be an artifact of how the file was saved, not evidence of duplicated content.

Because it makes no external factual claims, it needed no per-claim sourcing — the earlier "needs sourcing from scratch" framing assumed it made claims like the other three files do, which it doesn't. It contains exactly one uncited appeal to authority ("The literature converges around four reinforcing PM responsibilities"); an audit note was added inline at the top of the file marking this as original synthesis, not a sourced claim, consistent with how `gpt...md` already flags its own weighting choices as synthesis rather than prescription.

### `Research/Product Manager Assessment - December 11, 2021.csv` — Different kind of asset, no citation issue

This is a proprietary PM self-assessment worksheet, not AI-synthesized research — it has no citations because it isn't making external claims; it's the worksheet author's own leveling framework (Product Expertise / Practices & Skills / People Skills, each benchmarked 1-5 by role level: PM, Senior PM, Director, VP). Nothing to clean up here, but it should be attributed as an internal source, not presented as an external validated standard, wherever it's used. It directly informed the level-benchmark table in [`docs/interview-scorecard-template.md`](interview-scorecard-template.md) — see that file for how it was adapted (not copied) into this project's six-competency model. Its "People Skills And Related Competencies" section later also informed [`docs/people-management-competency.md`](people-management-competency.md) and the four people-management interview cards.

### `Research/AI Product Management Assessment.md` — Same kind of asset as the CSV above, no citation issue

Added after the pass above — another proprietary leveling framework, this one for ten AI-specific PM competencies (AI Fundamentals through AI Strategy & Competitive Advantage), each benchmarked 1-5 by role level. Same treatment as the CSV: no citation needed since it isn't making an external claim, but it should be attributed as an internal source, not a validated external standard, wherever it's used. It directly informed [`docs/ai-competency-model.md`](ai-competency-model.md), the optional AI-PM benchmark table in [`docs/interview-scorecard-template.md`](interview-scorecard-template.md), and the ten AI-competency interview cards indexed in [`docs/question-index.md`](question-index.md).

### `Research/epic-sizing-considerations.png` and `Research/story-sizing-considerations.png` — Internal sizing rubrics, no citation issue

Two proprietary engineering sizing rubrics contributed to this project — a "Guide for Sizing Epics by Complexity" (release planning, sized in calendar weeks with playful size labels) and a "Sizing Consideration" guide for story refinement (sized in Fibonacci points). Both score work across the same underlying dimensions: time to doneness, reuse of existing functionality, architectural impact, new technology introduced, similarity to past work, and team/multi-team coordination factors. No citation needed since these make no external claim — they're the contributing team's own internal practice, images not text. They directly informed three interview cards testing the judgment underneath sizing frameworks rather than sizing mechanics: [What Your Estimate Is Actually Measuring](../Questions/judgment/What-Your-Estimate-Is-Actually-Measuring.md), [Weeks for Leadership, Points for the Team](../Questions/judgment/Weeks-for-Leadership-Points-for-the-Team.md), and [The 21-Point Story](../Questions/judgment/The-21-Point-Story.md).

### `Research/EBOOK-Dangerous-Animals-of-Product-Management.pdf` and `Research/ProductCamp-2021.Dean-Peters-Presents.Dangerous-Animals-of-Product-Management.Transcript.txt` — Publicly published, real citations used

Unlike the private repos cited elsewhere in this project, these two are genuinely public works: *The Dangerous Animals of Product Management* is a Productboard publication co-authored by Dean Peters (2022), and the transcript is from Dean Peters's 2021 ProductCamp talk of the same name. Both are cited by name in the six cards adapted from them, with a link to productboard.com (the real, verifiable publisher) — no specific deep-link URL was fabricated for the ebook or talk recording itself since none was available to verify. Each card's real-world case study (JCPenney/Ron Johnson, ScaleFactor, Blockbuster/Netflix, Knight Capital, Dunkin' Donuts/Robert Rosenberg) is drawn directly from the source material, not invented.

### `Research/gemini.pm-questions-compendium.md` — Original question bank, no citation issue

Read in full. Like `copilot...md`, this is a self-contained original question bank (70 questions across seven categories) with a stated philosophy ("can this person recognize important problems, reason through uncertainty..." rather than "perform Product Manager improv theater") — it makes no external factual claims requiring a citation. Three genuine gaps not already covered by the active bank were adapted into cards: [Who Actually Owns This Decision](../Questions/judgment/Who-Actually-Owns-This-Decision.md) (peer-vs-peer decision-rights ambiguity), [One Signal Up, Another Down](../Questions/judgment/One-Signal-Up-Another-Down.md) (live diagnostic reasoning when two metrics disagree), and [Not Every Fix Is a Feature](../Questions/behavioral/Not-Every-Fix-Is-a-Feature.md) (solving via a non-product lever). The remaining ~67 questions were judged to duplicate existing cards under different phrasing and were not adapted.

## Recommendation

All four Research files with external claims (`gpt...md`, `plex...md`, `gem...md`) plus the question-bank file (`copilot...md`) are now audited:

- `gpt...md` — citations resolved. Statistics and study attributions can be repeated in public-facing docs with a real link behind each claim.
- `plex...md` — link-checked. 34 of 38 references are live; 1 was fixed with an archive link; 3 are flagged inline as dead (one, reference 4, backs several currently-unsourced footnotes — don't lean on those specific claims until a replacement is found).
- `gem...md` — link-checked. 23 of 25 references are live; 2 Medium links are inconclusive (bot-blocked, not confirmed dead). Separately, this file has an inline-citation-numbering integrity problem (see its findings section above) that a future pass should address — don't treat it as fully clean the way `gpt...md` is.
- `copilot...md` — confirmed not a duplicate, and confirmed not to need per-claim sourcing (it's an original question bank, not a research synthesis). One uncited "the literature" appeal is now flagged inline as synthesis, not fact.
- Two of the two proprietary worksheets (`Product Manager Assessment - December 11, 2021.csv`, `AI Product Management Assessment.md`) need no citation work, as noted above.
- `gemini.pm-questions-compendium.md` — confirmed not to need per-claim sourcing (original question bank, not a research synthesis), same treatment as `copilot...md`.
- Spot-check any individual link again before leaning on it heavily years from now — URLs do move, and this audit reflects link state as of when each pass was run, not a permanent guarantee.
