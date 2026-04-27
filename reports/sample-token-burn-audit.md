# Stackfax Sample Token Burn Audit

Report Type: Token Burn Audit

Use Case: OpenClaw task using model fallbacks, large context, knowledge files, web research, and premium-model routing

Overall Rating: ⭐⭐⭐

Stack Score: 61/100

Verdict: Model Routing Needed / Token Burn Risk

## Summary

This stack is functional, but the workflow is likely burning more tokens than necessary.

The main issue is not that the user is using Ai.

The main issue is that too much work is being routed through expensive model calls instead of being split into cheaper, clearer steps.

The stack should be restructured before it is used repeatedly.

## Risk Flags

- Token Burn Risk
- Premium Model Overuse
- Context Bloat Risk
- Silent Escalation Risk
- Tool Loop Burn
- Budget Cap Missing
- Model Routing Needed

## What Fits

This stack fits for:

- Research-heavy tasks
- Report generation
- Multi-step comparison work
- OpenClaw experimentation
- Early workflow testing
- Learning how agents behave

The user is working in the right general direction, but the workflow needs cost controls before it scales.

## What Is Draining Tokens

Likely token drains include:

- Large context windows
- Too much history loaded into each task
- Knowledge files loaded by default
- Premium models handling routine work
- Broad prompts that ask one agent to do too much
- Fallback chains that may escalate silently
- Tool loops without clear stopping rules

## Model Routing Verdict

Current model routing appears too expensive for the task.

Recommended routing:

- Code or tools gather and filter data
- Cheap model drafts or summarizes
- Mid-tier model cleans and organizes
- Strong model reviews, reasons, or makes final judgment
- Human approves anything important

The strongest model should not be responsible for every step.

## Context Bloat Review

Risk level: High

The stack may be loading more context than the task requires.

Recommended fixes:

- Load only task-specific files
- Keep history short
- Do not attach broad knowledge files by default
- Summarize long context before sending it to stronger models
- Separate research context from final judgment context

More context is not always better.

Relevant context is better.

## Silent Escalation Review

Risk level: Medium-High

If the workflow uses fallback chains, the user needs to know when the stack moves from cheap models to expensive models.

Recommended fixes:

- Add model caps
- Add session budget caps
- Add escalation alerts
- Log which model handled each step
- Require approval before premium fallback on repeated failures

The user should not discover escalation only after the bill arrives.

## Tool Loop Review

Risk level: Medium

Agent workflows can burn tokens through repeated searches, browser actions, and tool calls.

Recommended fixes:

- Set a max tool-call count
- Set a max step count
- Define a stopping condition
- Break broad tasks into smaller workflows
- Ask for approval before continuing expensive loops

## Subscription Fit

The user should review whether paid subscriptions and API usage overlap.

Possible overlap areas:

- ChatGPT subscription
- Claude subscription
- OpenRouter usage
- Gemini subscription
- Local model setup
- Agent platform costs
- Automation platform costs

The goal is not to own every model.

The goal is to use the right paid access for the actual workflow.

## Best Next Move

Split the workflow into five steps:

1. Gather data
2. Filter or extract with code/tools
3. Summarize with a cheaper model
4. Review or judge with a stronger model
5. Ask for human approval before final output or action

This should reduce token burn and make the workflow easier to debug.

## What Would Improve The Score

This stack could move from 61/100 to 80+/100 by adding:

- Session budget cap
- Model cap
- Tool-call cap
- Smaller task-specific context
- Clear fallback logging
- Cheaper draft layer
- Strong model only for review or judgment
- Subscription overlap review
- 30-day cost recheck

## Stackfax Principle

Use code for extraction.

Use Ai for judgment.

Do not spend premium-model money on intern tasks.

## Final Stackfax Verdict

The stack is promising, but it is currently too easy for tokens to drain quietly.

Do not scale this workflow until model routing, context loading, fallback escalation, and budget caps are cleaned up.

Final recommendation: Add cost controls before repeating the workflow.
