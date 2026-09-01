# Governing an Agent That Acts on Its Own

> Tell me about a time you had to decide how much an AI agent should be allowed to do autonomously across multiple steps — not just answer one question, but actually take action. What guardrails did you put around it, and why?

> **Follow-up** If the agent's exact plan can't be predicted step by step in advance, how would you know it was about to do something wrong?

## Type

Judgment

## Competencies Assessed

- Ethics, Self-Awareness, And Responsible Decision-Making

## AI Competency

[AI Experience & Human Agency](../../docs/ai-competency-model.md#ai-experience--human-agency) (also relevant to [AI Risk, Safety & Responsible Use](../../docs/ai-competency-model.md#ai-risk-safety--responsible-use))

## Why This Matters

Only use this card for roles where AI is a real part of the product surface — see [ai-competency-model.md](../../docs/ai-competency-model.md). "Agentic" AI — systems that plan, decide, and act across multiple steps rather than answering a single prompt — carries governance demands beyond a normal single-turn AI feature: guardrails, approval gates, and a way to catch a bad action mid-execution rather than only after the fact. This question tests whether a candidate actually distinguishes agentic autonomy from ordinary automation, a distinction easy to claim and easy to get wrong.

## Neutral Follow-Up Probes

- What could the agent actually do on its own — read-only, or could it take real-world actions (send, spend, delete, publish)?
- What would trigger it to stop and ask for human approval?
- Has it ever done something you didn't expect? What happened?

## Strong Evidence

1. Describes a genuinely multi-step, autonomous system — not a single-turn AI feature mislabeled as an "agent."
2. Names specific, concrete guardrails: scope limits on what actions are allowed, an approval gate before consequential actions, a kill switch, or logging for review.
3. Gives a real, specific answer for detecting a problem mid-execution — not just "we'd review it afterward."
4. Describes what actually happened when the agent did something unexpected, if it has, including how they responded.

## Warning Signs

1. The described system is really a single-turn AI feature, not a multi-step autonomous one — conflating automation with agentic AI.
2. No concrete guardrail named — just "we were careful."
3. No real answer for catching a problem before it completes, only after-the-fact review.

## Scoring Anchors

- **5:** Genuinely agentic system, specific concrete guardrails, a real mid-execution detection method, and an honest account of an unexpected action if one occurred.
- **3:** A real AI feature is described but it's unclear whether it's truly agentic, or the guardrails are vague.
- **1:** Conflates a simple AI feature with an "agent," or has no real guardrail or detection method.

## Attributions

* Adapted from a private AI-PM training curriculum's unit on orchestrating agents and agentic AI, which frames agentic AI through five hallmarks: autonomy, goal orientation, context awareness, decision-making, and accountability within guardrails.

## Additional Reading

* (None yet — contributions welcome.)
