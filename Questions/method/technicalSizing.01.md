# Technical Sizing Sanity Check

> Your engineers gave the same size estimate — one hour — for each of these three tasks. Which one feels wrong, and why?
> - Swap the order of two fields in a form. Estimate: 1 hour.
> - Make the delete button show a confirmation before it deletes. Estimate: 1 hour.
> - Make a paginated table sortable by any column. Estimate: 1 hour.

> **Follow-up** If they don't volunteer a "why" for each, drill into the why for each one individually.

## Type

Method

## Competencies Assessed

- Delivery, Execution, And Ownership

## Why This Matters

A PM doesn't need to write code, but does need enough technical fluency to sanity-check estimates, ask good questions of engineering, and avoid committing to timelines that don't hold up. This is a narrow, defensible use of a craft-style question: it has a clear right answer and a clear rubric, and is best run by or alongside an engineer, per `AGENTS.md`'s guidance on when method questions are appropriate.

## Neutral Follow-Up Probes

- Why does that one feel different from the other two?
- What would you expect to be involved in building it, even at a high level?
- Are you confident the other two are really one hour, or just less obviously wrong?

## Strong Evidence

1. Identifies that sortable-by-any-column on a paginated table is the one likely to be larger, because it typically requires server-side work, not just a UI change.
2. Explains the reasoning in plain terms — server-side sorting/pagination interaction — rather than just asserting a hunch.
3. Goes further and questions whether the other two are really trivial too (e.g., testing, edge cases), showing calibrated skepticism rather than accepting "small tasks are small" at face value.

## Warning Signs

1. Picks an answer without being able to explain the underlying technical reason.
2. Treats all three as equally simple with no distinction.
3. Shows no curiosity about what's actually involved in the harder task.

## Scoring Anchors

- **5:** Correctly identifies the sortable-table task, explains why in specific technical terms, and questions the other two estimates as well.
- **3:** Correctly identifies the harder task but the "why" is vague or partially right.
- **1:** Cannot identify a meaningful difference between the three tasks.

## Role Or Level Notes

Best run by, or in partnership with, an engineer on the panel. A missed answer on a web-related role should raise a flag about baseline technical fluency; weight accordingly for non-technical-product roles.

## Attributions

* First encountered from engineers at Reverb; adapted as a baseline technical-fluency check.

## Additional Reading

* (None yet — contributions welcome.)
