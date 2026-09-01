# Question Bank Triage

## Purpose

A working record of the disposition of every file in `Questions/` as of the Phase 2 curation pass described in [MODERNIZATION-PLAN.md](MODERNIZATION-PLAN.md). Each entry states what kind of prompt it is, which target type it maps to under the new structure, and what happens to it next.

Dispositions:

- **Retain & rewrite (exemplar)** — one of the three prompts the plan names explicitly as the first rewrites, to become the model for future interview cards.
- **Retain & rewrite** — kept as an active card, rewritten into the interview-card structure, but not a first-wave exemplar.
- **Legacy** — moved to `Questions/legacy/` unchanged in substance, labeled as historical material not recommended as a standalone hiring signal, per `AGENTS.md`.
- **Retire** — not currently used for any file; nothing is deleted without explicit direction.

## Triage Table

| File | Current Focus | Target Type | Disposition | Rationale |
|---|---|---|---|---|
| `Building-Trust-with-New-Teams.md` | Taking over an existing/new team, earning trust | Behavioral | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Strong behavioral prompt: elicits a real past situation, has a defensible rubric (servant-leadership, listening, respect for resistant teammates), assesses Influence/Collaboration and Ethics/Self-Awareness. |
| `Dealing-with-Seismic-Paradigm-Shifts.md` | Adjusting to a major organizational or priority shift | Behavioral / Situational | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Strong past-tense evidence question with clear positive/negative signals (learning orientation vs. blame). Assesses Delivery/Ownership and Ethics/Self-Awareness (how they talk about the change). |
| `Vanity-Analytics_vs_Action-Metrics.md` | Vanity metrics vs. actionable analytics | Judgment / Method | **Retain & rewrite (exemplar)** | Named explicitly in the plan. Clear, well-sourced rubric (Actionable/Accessible/Auditable) and directly assesses Metrics, Outcomes, And Learning — a named competency. Already has real attributions to rework into the new card format. |
| `AlarmClock-Design4Blind.md` | Designing an alarm clock for blind users | Situational | **Retain & rewrite** | Unlike the vending-machine prompt, this has real constraints (accessibility, a specific user) and a rubric centered on discovery questions before design — it primarily tests Customer Understanding And Discovery, not open-ended ideation. Rewrite to foreground the discovery-question behavior as the pass/fail signal, per `AGENTS.md`'s caution on abstract design exercises. |
| `technicalSizing.01.md` | Sanity-checking engineering size estimates | Method | **Retain & rewrite** | Narrow, has a clear rubric and a specific defensible use (engineer-run technical sanity check), which is exactly the exception `AGENTS.md` allows for craft/execution questions. Keep as a `method/` card; note in Role/Level Notes that it's best run by or with an engineer. |
| `ProductDesign-VendingMachine.md` | Open-ended "disrupt the vending machine industry" ideation | — | **Legacy** | Abstract product-design brainstorm without real constraints or a scoring rubric beyond "broad/deep/excited" — exactly what `AGENTS.md` and the plan flag to avoid as a primary hiring signal. Move to `Questions/legacy/` with a historical-context note. |
| `Number-of-Pianos.md` | Market-sizing / estimation puzzle | — | **Legacy** | Classic market-sizing brainteaser. The plan explicitly calls for moving estimation puzzles to legacy unless a future rubric establishes a specific, defensible use. The file already self-documents this concern reasonably well; preserve it as a labeled historical example. |
| `Interview Question Boilerplate.md` | N/A — template, not a question | — | **N/A (template)** | Already replaced with the interview-card template in this pass; not part of the question bank triage. |

## Summary

- **3 exemplars** to rewrite first: Building Trust, Seismic Paradigm Shifts, Vanity Metrics.
- **2 additional active rewrites**: Alarm Clock for the Blind, Technical Sizing Sanity Check.
- **2 moves to legacy**: Vending Machine, Number of Pianos.
- **0 retirements.**

## Next Steps

1. ~~Create `Questions/behavioral/`, `Questions/situational/`, `Questions/judgment/`, `Questions/method/`, `Questions/legacy/`.~~ Done.
2. ~~`git mv` each file into its target folder (legacy files move as-is, plus a short historical-context note; active files move as a prelude to being rewritten in place).~~ Done.
3. ~~Add an index (by competency and type) once files are settled in their folders.~~ Done — see [question-index.md](question-index.md).
4. ~~Rewrite the three exemplars into the new interview-card structure.~~ Done — Building Trust, Seismic Paradigm Shifts, Vanity Metrics.
5. ~~Rewrite the two additional retained cards (Alarm Clock for the Blind, Technical Sizing Sanity Check).~~ Done.
6. ~~Update `question-index.md` to mark each card *(rewritten)* as it's completed, and firm up its competency links.~~ Done.

Phase 2 is complete. Nine additional cards were then written to fill out a 14-question core bank for Phase 3 — see [core-interview-loop.md](core-interview-loop.md) and [question-index.md](question-index.md) for the full active set.

This table should be updated if a disposition changes — e.g., if a specific rubric is later developed that would justify moving `Number-of-Pianos.md` or `ProductDesign-VendingMachine.md` back into active use.
