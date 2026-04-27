# Token Burn Audit

The Token Burn Audit is a Stackfax report type for users who are spending too much on premium-model tokens, API calls, or overlapping Ai subscriptions.

The goal is to find where the stack is wasting tokens, using expensive models for simple work, loading too much context, or silently escalating to higher-cost models.

## Core Question

Is this stack using the right model, context, tool, and workflow for the task, or is it burning tokens because the workflow is poorly structured?

## Who This Is For

The Token Burn Audit is for:

- Users surprised by high API bills
- OpenClaw users who burned too many tokens on one task
- Builders using premium models for routine work
- Businesses running Ai automations without cost controls
- Users with overlapping model subscriptions
- Users using large context windows without understanding the cost
- Users relying on fallback chains that may silently escalate

## What The Audit Reviews

A Token Burn Audit reviews:

- Premium model overuse
- Model routing
- Model subscription overlap
- API/token costs
- Context bloat
- Memory loading
- Knowledge file loading
- Fallback escalation
- Repeated tool loops
- Workflow design
- Tasks that should use code instead of Ai
- Budget caps
- Model caps
- Logging and visibility

## Common Token Burn Patterns

### Premium Model Overuse

This happens when the strongest or most expensive model handles too much routine work.

Warning signs:

- Premium model drafts everything
- Premium model summarizes simple text
- Premium model does basic classification
- Premium model performs extraction work that code could handle
- No cheaper draft/review layers exist

Stackfax recommendation:

Use cheaper models for routine work and reserve strong models for judgment, reasoning, and final review.

### Context Bloat

This happens when the stack loads too much information into tasks that do not need it.

Warning signs:

- Large context loaded by default
- Knowledge files loaded into every call
- Long histories always included
- Irrelevant files attached to simple tasks
- Memory is always on
- Sensitive data is loaded unnecessarily

Stackfax recommendation:

Load only the context needed for the task.

### Silent Escalation

This happens when a fallback chain moves from cheaper models to expensive models without the user clearly noticing.

Warning signs:

- Fallback chain includes premium models
- No session budget cap
- No model cap
- No escalation alert
- No log showing which model handled which step
- User only notices after the bill arrives

Stackfax recommendation:

Add model caps, session budget caps, and escalation visibility.

### Tool Loop Burn

This happens when an agent repeatedly calls tools, searches, browsers, or APIs without clear stopping rules.

Warning signs:

- Repeated web searches
- Repeated browser actions
- Long tool loops
- No max step count
- No clear stop condition
- Broad task prompt with unclear output

Stackfax recommendation:

Set tool-call limits, task boundaries, and approval checkpoints.

### Ai Doing Code Work

This happens when Ai is used for deterministic work that code, filters, spreadsheets, or simple scripts could handle better.

Warning signs:

- Ai extracts simple structured fields
- Ai filters data that code could filter
- Ai repeatedly searches instead of using a structured source
- Ai compares raw data before it is cleaned
- Ai handles tasks that could be preprocessed cheaply

Stackfax principle:

Use code for extraction. Use Ai for judgment.

## Model Routing Pattern

A token-smart stack should separate work into layers.

Recommended pattern:

- Code or tools gather and filter
- Cheap model drafts
- Cheap or mid-tier model summarizes
- Strong model reasons or reviews
- Human approves important actions

The expensive model should not be doing every step.

## Budget Controls

A strong stack should include budget controls.

Recommended controls:

- Session budget cap
- Daily budget cap
- Model cap
- Context cap
- Tool-call cap
- Escalation alert
- Logging by model
- Logging by workflow
- Cost review after testing

## Subscription Fit

Token burn is not only API cost.

Users can also waste money by paying for overlapping subscriptions.

Stackfax checks whether the user really needs multiple paid tools such as:

- ChatGPT
- Claude
- Gemini
- OpenRouter
- Local models
- API credits
- Business Ai tools
- Agent platforms
- Automation platforms

The question is not which tool is best.

The question is which paid access actually fits the workflow.

## Example Token Burn Verdict

Verdict: Model Routing Needed

Risk flags:

- Premium Model Overuse
- Context Bloat Risk
- Silent Escalation Risk
- Tool Loop Burn
- Budget Cap Missing

Best next move:

Split the workflow into gather, filter, summarize, reason, and review steps. Use code or tools for extraction, cheaper models for routine work, and strong models only for judgment or final review.

## What Would Improve The Score

A stack can improve its Token Burn Audit score by adding:

- Clear task boundaries
- Cheaper draft layer
- Strong model only for review or judgment
- Session budget cap
- Model cap
- Tool-call cap
- Smaller task-specific context
- Fallback visibility
- Cost logging
- 30-day recheck

## Common Badges

Token Burn Audits may use badges such as:

- Token-Smart
- Token Burn Risk
- Context Bloat Risk
- Silent Escalation Risk
- Model Routing Needed
- Budget Cap Required
- Subscription Overlap Risk
- Tool Loop Burn
- Human Approval Required

## Final Rule

Do not spend premium-model money on intern tasks.

Stackfax helps users find where tokens are draining before the bill teaches the lesson.
