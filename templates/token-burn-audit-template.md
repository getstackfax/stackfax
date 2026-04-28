# Stackfax Token Burn Audit Template

Report Type: Token Burn Audit

Use Case: [Describe the workflow, agent task, or model setup being audited]

Overall Rating: [⭐ to ⭐⭐⭐⭐⭐]

Stack Score: [0–100]

Verdict: [Main token burn verdict]

## Summary

[Short plain-English summary of where tokens may be draining and why.]

## User Goal

The user wants to:

- [Goal 1]
- [Goal 2]
- [Goal 3]

## Current Stack

The current or proposed stack includes:

- [Model/provider/subscription/tool 1]
- [Model/provider/subscription/tool 2]
- [Agent/workflow/tool 3]

## Main Verdict

[Clear recommendation.]

Possible verdict examples:

- Token Burn Risk
- Model Routing Needed
- Context Bloat Risk
- Silent Escalation Risk
- Budget Cap Required
- Tool Loop Burn
- Subscription Overlap Risk

## Risk Flags

- [Risk flag 1]
- [Risk flag 2]
- [Risk flag 3]

Possible risk flags:

- Premium Model Overuse
- Context Bloat Risk
- Silent Escalation Risk
- Tool Loop Burn
- Budget Cap Missing
- Model Routing Needed
- Subscription Overlap Risk

## What Fits

This workflow fits well for:

- [Fit 1]
- [Fit 2]
- [Fit 3]

## What Is Draining Tokens

Likely token drains include:

- [Token drain 1]
- [Token drain 2]
- [Token drain 3]

Possible token drains:

- Large context windows
- Long chat histories
- Knowledge files loaded by default
- Premium models doing routine work
- Broad prompts
- Repeated tool calls
- Silent fallback escalation
- No budget caps

## Model Routing Review

Current routing: [Unclear / Basic / Good / Strong]

Recommended routing:

- Code or tools gather and filter
- Cheap model drafts
- Cheap or mid-tier model summarizes
- Strong model reviews or reasons
- Human approves important actions

Notes:

[Explain whether the model routing fits the workflow.]

## Context Review

Context bloat risk: [Low / Medium / High]

Notes:

[Explain whether the stack is loading too much history, memory, knowledge, or unrelated files.]

Recommended fixes:

- Load only task-specific files
- Keep history short
- Summarize long context before review
- Avoid broad memory access
- Separate research context from final judgment context

## Silent Escalation Review

Silent escalation risk: [Low / Medium / High]

Notes:

[Explain whether cheaper models may silently fall back to expensive models.]

Recommended fixes:

- Add model caps
- Add session budget caps
- Add escalation alerts
- Log which model handled each step
- Require approval before premium fallback on repeated failures

## Tool Loop Review

Tool loop risk: [Low / Medium / High]

Notes:

[Explain whether agents may repeatedly browse, search, click, retry, or call tools.]

Recommended fixes:

- Max tool-call count
- Max step count
- Stop condition
- Human checkpoint before continuing
- Logs of tool actions

## Subscription And API Review

Subscription/API risk: [Low / Medium / High]

Notes:

[Explain whether subscriptions, API credits, routers, or agent platforms overlap.]

## Best Next Move

The best next move is:

[One clear next action.]

Example:

Split the workflow into gather, filter, summarize, reason, and review steps. Use code or tools for extraction, cheaper models for routine work, and strong models only for judgment or final review.

## What Would Improve The Score

To improve the score, add:

- [Improvement 1]
- [Improvement 2]
- [Improvement 3]
- [Improvement 4]

Possible improvements:

- Session budget cap
- Model cap
- Tool-call cap
- Smaller task-specific context
- Fallback visibility
- Cost logging
- Cheaper draft layer
- Strong model only for review or judgment
- 30-day cost recheck

## Stackfax Principle

Use code for extraction.

Use Ai for judgment.

Do not spend premium-model money on intern tasks.

## Final Token Burn Verdict

[Final short verdict.]

Final recommendation: [Direct recommendation.]
