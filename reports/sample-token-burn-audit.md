# Stackfax Sample Token Burn Audit

Report Type: Token Burn Audit

Use Case: OpenClaw task using model fallbacks, large context, knowledge files, web research, and premium-model routing

Overall Rating: ⭐⭐⭐

Stack Score: 61/100

Verdict: Model Routing Needed / Token Burn Risk

---

## Summary

This stack is functional, but the workflow is likely burning more tokens than necessary.

The main issue is not that the user is using Ai.

The main issue is that too much work is being routed through expensive model calls instead of being split into cheaper, clearer steps.

The stack should be restructured before it is used repeatedly.

---

## Risk Flags

- Token Burn Risk
- Premium Model Overuse
- Context Bloat Risk
- Silent Escalation Risk
- Tool Loop Burn
- Budget Cap Missing
- Model Routing Needed
- Cost Visibility Missing
- Run Receipts Missing

---

## What Fits

This stack fits for:

- research-heavy tasks
- report generation
- multi-step comparison work
- OpenClaw experimentation
- early workflow testing
- learning how agents behave

The user is working in the right general direction, but the workflow needs cost controls before it scales.

---

## Workflow Fit

Workflow fit: Basic

The workflow has a real use case, but it is too broad.

The task should be broken into smaller steps before repeated use.

A better workflow would separate:

- gathering
- filtering
- summarizing
- reviewing
- final judgment
- human approval

The current workflow is trying to do too much in one pass.

---

## What Is Draining Tokens

Likely token drains include:

- large context windows
- too much history loaded into each task
- knowledge files loaded by default
- premium models handling routine work
- broad prompts that ask one agent to do too much
- fallback chains that may escalate silently
- tool loops without clear stopping rules
- repeated research calls without a stop condition

---

## Model Routing Verdict

Current model routing appears too expensive for the task.

Recommended routing:

- Code or tools gather and filter data.
- Cheap model drafts or summarizes.
- Mid-tier model cleans and organizes.
- Strong model reviews, reasons, or makes final judgment.
- Human approves anything important.

The strongest model should not be responsible for every step.

---

## Context Bloat Review

Risk level: High

The stack may be loading more context than the task requires.

Recommended fixes:

- load only task-specific files
- keep history short
- do not attach broad knowledge files by default
- summarize long context before sending it to stronger models
- separate research context from final judgment context

More context is not always better.

Relevant context is better.

---

## Silent Escalation Review

Risk level: Medium-High

If the workflow uses fallback chains, the user needs to know when the stack moves from cheap models to expensive models.

Recommended fixes:

- add model caps
- add session budget caps
- add escalation alerts
- log which model handled each step
- require approval before premium fallback on repeated failures

The user should not discover escalation only after the bill arrives.

---

## Tool Loop Review

Risk level: Medium

Agent workflows can burn tokens through repeated searches, browser actions, retries, and tool calls.

Recommended fixes:

- set a max tool-call count
- set a max step count
- define a stopping condition
- break broad tasks into smaller workflows
- ask for approval before continuing expensive loops

---

## Cost Visibility Review

Cost visibility: Weak

The user needs to know which model, tool, provider, or fallback path created the cost.

A useful cost view should show:

- which model handled each step
- whether fallback happened
- how many tool calls were made
- how much context was loaded
- whether files were attached
- whether the task exceeded budget
- which step created the most cost

Without cost visibility, token burn becomes guesswork.

---

## Run Receipt Review

Run receipt status: Missing

A useful run receipt should show:

- requested task
- model used
- tools used
- files or context used
- fallback events
- tool calls made
- what changed
- what failed
- approximate cost
- what needs human review
- what to change next run

Agent output is a claim.

A run receipt is evidence.

---

## Subscription Fit

The user should review whether paid subscriptions and API usage overlap.

Possible overlap areas:

- ChatGPT subscription
- Claude subscription
- OpenRouter usage
- Gemini subscription
- local model setup
- agent platform costs
- automation platform costs

The goal is not to own every model.

The goal is to use the right paid access for the actual workflow.

---

## Best Next Move

Split the workflow into five steps:

1. Gather data.
2. Filter or extract with code/tools.
3. Summarize with a cheaper model.
4. Review or judge with a stronger model.
5. Ask for human approval before final output or action.

This should reduce token burn and make the workflow easier to debug.

---

## What Would Improve The Score

This stack could move from 61/100 to 80+/100 by adding:

- session budget cap
- model cap
- tool-call cap
- smaller task-specific context
- clear fallback logging
- cheaper draft layer
- strong model only for review or judgment
- subscription overlap review
- run receipt template
- 30-day cost recheck

---

## Stackfax Principle

Use code for extraction.

Use Ai for judgment.

Do not spend premium-model money on routine tasks.

---

## Final Stackfax Verdict

The stack is promising, but it is currently too easy for tokens to drain quietly.

Do not scale this workflow until model routing, context loading, fallback escalation, cost visibility, and budget caps are cleaned up.

Final recommendation: Add cost controls before repeating the workflow.
