# AI Competency Model

## Purpose

An optional, additional competency layer for roles where building AI-powered products is a meaningful part of the job — a PM shipping LLM features, an agentic-workflow product, or a recommendation/personalization system. It sits alongside, not instead of, the six core competencies in [competency-model.md](competency-model.md): every AI-competency card also maps to a core competency, because judgment about an AI feature is still judgment, evidence about a shipped AI capability is still evidence. This model names the AI-specific *content* that judgment needs to be applied to.

**Don't use this for a role where AI isn't a real part of the product surface.** Testing AI literacy on a candidate for a role with no AI component tests trivia, not job-relevant judgment — exactly what `AGENTS.md` warns against.

The ten categories below, and their level benchmarks (Product Manager / Senior PM / Director / VP), are adapted from [`Research/AI Product Management Assessment.md`](../Research/AI%20Product%20Management%20Assessment.md) — an internal framework contributed to this project, in the same spirit as the [PM self-assessment worksheet](../Research/Product%20Manager%20Assessment%20-%20December%2011%2C%202021.csv) that informed the core [scorecard's level-benchmark table](interview-scorecard-template.md). Treat the benchmarks as a starting default to calibrate against your own org, not a validated external standard.

## The Categories

### AI Fundamentals
Understands AI capabilities, limitations, probabilistic behavior, hallucination, context windows, and basic model concepts — enough to reason about a product decision, not enough to build the model.

**Look for:** explaining a real limitation in plain language, a specific instance where a limitation changed a product decision, and calibrated confidence (neither dismissive of AI nor treating it as infallible).

### AI Opportunity Discovery
Identifies where AI can meaningfully improve customer outcomes, workflows, decisions, or economics — as opposed to adding AI because it's expected or trendy.

**Look for:** a real decision *not* to use AI where it was proposed, articulated reasoning for where AI does and doesn't add value, and connection back to a customer or business outcome rather than a capability for its own sake.

### AI Product Discovery & Validation
Tests AI use cases for desirability, feasibility, and uncertainty before committing to production — treating an AI feature's behavior as something to be discovered, not assumed.

**Look for:** a real validation method used before a full build, honest acknowledgment of what was still uncertain going in, and a plan for what evidence would have stopped the project.

### Data & Context Strategy
Understands what data, knowledge, retrieval, feedback, and permissions an AI product actually needs to work — and what happens when that data doesn't exist yet.

**Look for:** a specific data or context gap discovered during the work, not just planned for in advance, and a concrete response to that gap.

### AI Experience & Human Agency
Designs the right interaction between AI and humans — augmentation vs. automation, appropriate confidence signaling, and escalation paths — rather than defaulting to maximum autonomy or maximum caution.

**Look for:** a specific, reasoned line drawn between what the AI decides and what a human decides, and conditions that would move that line in either direction.

### AI Evaluation & Metrics
Defines how AI quality and product outcomes are actually evaluated — task success, accuracy, reliability, cost, latency, and downstream behavioral consequences — not just whether it shipped.

**Look for:** a specific evaluation method beyond "users didn't complain," and evidence the candidate distinguishes a one-off bad output from a systemic quality problem.

### AI Risk, Safety & Responsible Use
Recognizes and manages privacy, security, bias, explainability, compliance, misuse, and inappropriate delegation of agency to the system.

**Look for:** a real capability delayed, scoped down, or not shipped because of a named risk, and evidence of who else was brought into that decision.

### AI Economics & Technical Tradeoffs
Understands model choice, build/buy/partner decisions, inference cost, latency, and the quality/cost tradeoff space well enough to make or contribute to that call.

**Look for:** a specific build/buy/partner decision with real reasoning, and honesty about what the cost or latency estimate got wrong going in.

### AI Product Operations & Learning
Uses telemetry, evaluation results, and user feedback to actually change how the AI product behaves over time — closing the loop, not just reporting on it.

**Look for:** a specific behavior change made as a result of production data, and a way of knowing the change was actually an improvement rather than just different.

### AI Strategy & Competitive Advantage
Connects AI capabilities to product strategy, differentiation, defensibility, and business model — distinguishing a capability that's a real moat from one any competitor can replicate quickly.

**Look for:** a specific reasoned judgment about whether an AI capability was defensible, and what would actually make it hard to copy (proprietary data, workflow integration, distribution) versus what wouldn't.

## Using This Model

Each AI-competency card lives in [`Questions/ai/`](../Questions/ai/) and names both its AI category (from this document) and its underlying core competency (from [competency-model.md](competency-model.md)) — see [question-index.md](question-index.md) for the full listing. `Questions/ai/` is organized by domain rather than by assessment format (unlike `behavioral/`, `situational/`, `judgment/`, `method/`); each card still records its own format Type in its content. Use these cards as an optional add-on round for AI-heavy roles, not a replacement for the core [interview loop](core-interview-loop.md).
