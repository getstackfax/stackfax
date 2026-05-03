# Stackfax Token Burn Audit Template

Report Type: Token Burn Audit

Use Case: [Describe the workflow, agent task, model setup, or automation being audited]

Overall Rating: [⭐ to ⭐⭐⭐⭐⭐]

Stack Score: [0–100]

Verdict: [Main token burn verdict]

---

## Summary

[Short plain-English summary of where tokens may be draining, why it matters, and what should be fixed first.]

---

## User Goal

The user wants to:

- [Goal 1]
- [Goal 2]
- [Goal 3]

---

## Current Stack

The current or proposed stack includes:

The current or proposed stack includes:

- Model/provider/subscription/tool:
- Model/provider/subscription/tool:
- Agent/workflow/tool:
- Router/API/local model/tooling layer:
- Human approval or review process:
  
---

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
- Cost Visibility Missing
- Run Receipts Missing
- Strong Model Overused

---

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
- Cost Visibility Missing
- Run Receipts Missing
- Fallback Visibility Missing
- Workflow Too Broad

---

## What Fits

This workflow fits well for:

- [Fit 1]
- [Fit 2]
- [Fit 3]

Example fits:

- high-volume repeatable summaries
- classification
- extraction
- first-draft generation
- research prep
- internal workflow triage
- human-reviewed decision support

---

## What Is Draining Tokens

Likely token drains include:

- [Token drain 1]
- [Token drain 2]
- [Token drain 3]

Possible token drains:

- large context windows
- long chat histories
- knowledge files loaded by default
- premium models doing routine work
- broad prompts
- repeated tool calls
- repeated browser/search loops
- silent fallback escalation
- no session budget caps
- no step limit
- no model cap
- no cheap draft layer
- no extraction/filtering before model review

---

## Model Routing Review

Current routing: [Unclear / Basic / Good / Strong]

Recommended routing:

- Code or tools gather and filter.
- Cheap model drafts.
- Cheap or mid-tier model summarizes.
- Strong model reviews, reasons, or decides.
- Human approves important actions.

Notes:

[Explain whether the model routing fits the workflow.]

Good routing means each model has a job.

Bad routing means the strongest model is doing everything.

---

## Context Review

Context bloat risk: [Low / Medium / High]

Notes:

[Explain whether the stack is loading too much history, memory, knowledge, or unrelated files.]

Recommended fixes:

- Load only task-specific files.
- Keep history short.
- Summarize long context before review.
- Avoid broad memory access.
- Separate research context from final judgment context.
- Pass state, not full history.
- Retrieve only what the current step needs.

---

## Silent Escalation Review

Silent escalation risk: [Low / Medium / High]

Notes:

[Explain whether cheaper models may silently fall back to expensive models.]

Recommended fixes:

- Add model caps.
- Add session budget caps.
- Add escalation alerts.
- Log which model handled each step.
- Require approval before premium fallback on repeated failures.
- Define when fallback is allowed.
- Define when the system should stop instead of escalating.

---

## Tool Loop Review

Tool loop risk: [Low / Medium / High]

Notes:

[Explain whether agents may repeatedly browse, search, click, retry, call tools, or re-run the same failed step.]

Recommended fixes:

- Max tool-call count.
- Max step count.
- Stop condition.
- Human checkpoint before continuing.
- Logs of tool actions.
- Retry limit.
- Failure reason before retry.
- Manual review after repeated failure.

---

## Budget Control Review

Budget control: [Missing / Basic / Good / Strong]

Current controls:

- [Control 1]
- [Control 2]
- [Control 3]

Recommended controls:

- session budget cap
- daily or monthly budget cap
- per-task model cap
- tool-call cap
- fallback approval
- cost alert
- cost log
- 30-day recheck

Notes:

[Explain whether the user can predict or limit cost before the workflow runs.]

---

## Cost Visibility Review

Cost visibility: [Missing / Basic / Good / Strong]

The user should be able to see:

- which model ran
- how many calls happened
- which tool calls happened
- whether fallback occurred
- approximate cost
- what step created the most cost
- what failed or retried
- what should be changed next

Notes:

[Explain whether token spend is visible enough to diagnose.]

---

## Subscription And API Review

Subscription/API risk: [Low / Medium / High]

Notes:

[Explain whether subscriptions, API credits, routers, local models, or agent platforms overlap.]

Questions to check:

- Does each subscription have a clear job?
- Is the user paying for duplicate capabilities?
- Are API credits being used for tasks already covered by a subscription?
- Is a local model being used where it actually helps?
- Is the paid router adding clarity or hiding cost?

---

## Run Receipt Review

Run receipt status: [Missing / Basic / Good / Strong]

A useful token-burn run receipt should show:

- requested task
- model used
- tools used
- files/context used
- number of steps
- fallback events
- retries
- approximate cost
- output produced
- what needs human review
- what to change next run

Notes:

[Explain whether the user can reconstruct what happened after the workflow runs.]

---

## Best Next Move

The best next move is:

[One clear next action.]

Example:

Split the workflow into gather, filter, summarize, reason, and review steps. Use code or tools for extraction, cheaper models for routine work, and strong models only for judgment or final review.

---

## What Would Improve The Score

To improve the score, add:

- [Improvement 1]
- [Improvement 2]
- [Improvement 3]
- [Improvement 4]

Possible improvements:

- session budget cap
- model cap
- tool-call cap
- step limit
- retry limit
- smaller task-specific context
- fallback visibility
- cost logging
- cheap draft layer
- strong model only for review or judgment
- run receipt
- 30-day cost recheck
- clearer model jobs
- human approval before premium fallback

---

## Stackfax Principle

Use code for extraction.

Use Ai for judgment.

Do not spend premium-model money on routine tasks.

Strong models should earn their seat.

---

## Final Token Burn Verdict

[Final short verdict.]

Final recommendation: [Direct recommendation.]
