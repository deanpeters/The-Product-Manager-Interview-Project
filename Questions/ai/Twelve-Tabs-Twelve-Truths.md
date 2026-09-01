# Twelve Tabs, Twelve Truths

> Each PM on your team has built their own effective personal setup for working with AI tools — their own prompts, their own saved context, their own shortcuts. Individually, everyone's happy with their own results. But you start noticing the team's outputs — specs, research summaries, roadmap rationale — are quietly drifting apart in tone, assumptions, and even facts. How would you diagnose what's happening, and what would you do about it?

> **Follow-up** What would you actually build or change so this doesn't just become "everyone please use the same prompt," which nobody will follow?

## Type

Judgment

## Competencies Assessed

- Influence, Collaboration, And Communication

## AI Competency

[Data & Context Strategy](../../docs/ai-competency-model.md#data--context-strategy)

## Why This Matters

Only use this card for roles where AI is a real part of the product surface — see [ai-competency-model.md](../../docs/ai-competency-model.md). "What the Model Needs to Know" tests context strategy for a single AI product or feature; this card tests a different, easy-to-miss version of the same problem — context as a *team* infrastructure question. When every PM has their own private, ad hoc setup for working with AI, the team loses reproducibility: two people can ask a reasonable-sounding question and get quietly different, unreconciled answers, and nobody notices until the divergence shows up in a decision. This tests whether a candidate treats that as a real process problem worth solving, not an acceptable cost of individual productivity.

## Neutral Follow-Up Probes

- How would you actually detect this kind of drift before it causes a bad decision, rather than after?
- What's the difference between healthy variation in how people work and the kind of drift that's a real problem?
- Who owns keeping shared context accurate and up to date once it exists?
- What tradeoff are you accepting by standardizing this, and how would you know if it's not worth it?

## Strong Evidence

1. Diagnoses the actual mechanism — personal, unshared, unversioned context accumulating differently across people — rather than treating it as a vague culture problem.
2. Proposes something concrete: shared, versioned context artifacts, a common source of truth documents point back to, or a lightweight review step — not just an appeal to "better communication."
3. Addresses adoption realistically — why a shared setup would actually get used rather than quietly abandoned in favor of everyone's personal workaround.
4. Names an explicit owner or process for keeping the shared context current, since stale shared context is its own failure mode.

## Warning Signs

1. Treats this as a training or communication problem rather than an infrastructure one.
2. Proposes a fix that depends entirely on individual discipline ("just remind everyone to use the same prompt") with no structural backing.
3. No answer for who maintains the shared context once built, or how staleness gets caught.

## Scoring Anchors

- **5:** Correctly diagnoses the mechanism, proposes a concrete shared-context solution, addresses real-world adoption, and names ownership for keeping it current.
- **3:** Reasonable diagnosis and a plausible fix, but thin on adoption or maintenance.
- **1:** Treats it as a soft culture issue with no structural fix, or proposes something with no realistic chance of being adopted.

## Attributions

* Adapted from Dean Peters, "Day 05 - Context Engineering Is a Team Sport," *Confessions of a Feature Factory Escapee* (deanpeters.substack.com), a real, publicly published essay by the repository owner.

## Additional Reading

* [Confessions of a Feature Factory Escapee](https://deanpeters.substack.com/) — Dean Peters's Substack publication.
