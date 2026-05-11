# Stackfax Quick Report Template

Report Type: Stackfax Quick Report  
Checked: [Date]  
Use Case: [Describe the user’s main use case]  
Overall Rating: [⭐ to ⭐⭐⭐⭐⭐]  
Stack Score: [0–100]  
Verdict: [Main verdict]  
Recheck Trigger: [What should make this user recheck the stack?]

---

## Summary

[Short plain-English summary of the user’s stack, goal, and current fit.]

---

## User Goal

The user wants to:

- [Goal 1]
- [Goal 2]
- [Goal 3]

---

## Current / Proposed Stack

The stack includes:

- Tools/models/subscriptions: [List]
- Hardware: [List or “none yet”]
- Agent/workflow layer: [Describe]
- Human approval or review process: [Describe or “unclear”]

---

## Main Verdict

[Clear recommendation.]

Common verdicts:

- Do Not Buy Yet
- Cloud-First
- Local-Ready
- Hardware Justified
- Overkill Warning
- Model Routing Needed
- Token Burn Risk
- Simplify Subscriptions
- Human Approval Required
- Business Automation Ready
- Production Not Ready
- Safe To Test
- Recheck Needed

---

## Badges

- StackChecked
- [Badge 2]
- [Badge 3]
- [Badge 4]

Common badges:

- Token-Smart
- Cloud-First
- Local-Ready
- Hardware Justified
- Human Approval Required
- Run Receipts Needed
- Workflow Fit Unclear
- Business Automation Ready
- Production Not Ready

---

## What Fits

This stack fits well for:

- [Fit 1]
- [Fit 2]
- [Fit 3]

---

## What Looks Overbuilt

This stack may be overbuilt if:

- [Overkill signal 1]
- [Overkill signal 2]
- [Overkill signal 3]

Common overkill signals:

- buying hardware before defining the workflow
- using premium models for routine tasks
- adding agents before approval gates exist
- paying for overlapping subscriptions
- copying a creator/vendor stack without matching the use case
- building around tools instead of the job

---

## Risk Review

### Token Burn Risk

Risk level: [Low / Medium / High]

[Explain token burn risks, model routing issues, context bloat, fallback escalation, or tool loops.]

Recommended checks:

- Is the strongest model doing every step?
- Is too much context loaded by default?
- Are long histories included in every call?
- Are knowledge files loaded into simple tasks?
- Are there repeated tool/browser/search loops?
- Is there a session budget cap?
- Can code/tools do extraction before Ai does judgment?

---

## Cost Visibility

Status: [Missing / Basic / Good / Strong]

[Explain whether the user can see which models, tools, subscriptions, API calls, retries, fallback events, or human review time created cost.]

Recommended checks:

- Which model handled each step?
- Why was that route selected?
- Did fallback escalation happen?
- How many tool calls or retries happened?
- Was a premium model used?
- Was the output useful enough to justify the cost?
- Could this route be cheaper next time?

---

## Hardware Fit

Verdict: [Do Not Buy Yet / Cloud-First / Local-Ready / Hardware Justified / Overkill Warning]

[Explain whether local hardware, Mac mini, GPU rig, local models, or cloud/server setup is justified.]

Hardware is more justified when the user needs:

- local model testing
- privacy isolation
- always-on local workflows
- high-volume repeatable tasks
- a dedicated Ai workspace
- separation from a personal machine

Hardware is less justified when the workflow is still undefined.

---

## Model / Subscription Fit

Verdict: [Keep Current Setup / Simplify Subscriptions / Subscription Overlap Risk / Model Routing Needed]

[Explain whether current paid tools, subscriptions, APIs, routers, or local models fit the workflow.]

Questions to check:

- Does each paid tool have a clear job?
- Are subscriptions overlapping?
- Is the user paying for tools they do not use?
- Should some tasks use API credits instead of subscriptions?
- Should local models handle routine tasks?

---

## Workflow Fit

Verdict: [Clear / Unclear / Needs Narrowing / Ready To Test]

[Explain whether the workflow is real, repeatable, and easy to verify.]

A good workflow has:

- clear input
- clear output
- clear owner
- clear done-state
- clear review point
- clear failure mode
- clear next step

---

## Approval Gates

Risk level: [Low / Medium / High]

Human approval should be required before Ai can:

- send messages
- post publicly
- contact customers
- move or delete files
- change settings
- access credentials
- touch wallets or financial accounts
- edit customer records
- change inventory, payments, or production systems

[Explain which actions should stay draft-only, read-only, or human-approved.]

---

## Privacy / Credential Isolation

Risk level: [Low / Medium / High]

[Explain whether personal files, business data, customer data, credentials, browser sessions, tools, or clients are properly isolated.]

Recommended checks:

- Are personal and business accounts separated?
- Are credentials isolated?
- Are private files protected?
- Are customer records restricted?
- Are browser sessions safe?
- Are agents limited to the tools they actually need?

---

## Run Receipts

Status: [Missing / Basic / Good / Strong]

A useful run receipt should show:

- requested task
- model used
- tools used
- files/context used
- actions taken
- what changed
- what failed
- approximate cost
- what needs human review
- what to change next run

[Explain whether the user can tell what happened after the workflow runs.]

---

## Context / Decision Receipts

Status: [Missing / Basic / Good / Strong]

[Explain whether the report can show what context was used and why the main verdict was chosen.]

A useful context or decision receipt should show:

- what context was used
- what context was excluded
- what assumptions were made
- what evidence supports the verdict
- what risks changed the recommendation
- what would change the verdict later

---

## Production Readiness

Risk level: [Low / Medium / High]

[Explain whether this stack is ready for real workflows or should remain experimental.]

Production readiness requires:

- repeatable workflow
- approval gates
- run receipts
- failure handling
- credential isolation
- cost visibility
- rollback path
- human owner

---

## Agent ROI

Status: [Unclear / Early Signal / Good / Strong]

[Explain whether the stack is producing useful verified work, or just activity.]

Agent ROI should consider:

- completed useful work
- supervision required
- cost created
- cleanup required
- risk introduced
- repeatability
- compounding value

---

## Best Next Move

The best next move is:

[One clear action.]

Example:

Build one safe starter workflow that observes, summarizes, and reports before giving agents access to private accounts, customer data, credentials, or production systems.

---

## Suggested Upgrade Path

To improve the score, add:

- [Upgrade 1]
- [Upgrade 2]
- [Upgrade 3]
- [Upgrade 4]

Common upgrades:

- clearer workflow definition
- model routing
- token budget cap
- approval gate checklist
- run receipt template
- credential isolation
- smaller task-specific context
- cheaper draft layer
- strong model only for review or judgment
- cost visibility
- context receipts
- decision receipts
- 30-day recheck

---

## 30-Day Recheck

Recheck this stack after 30 days of real use.

Track:

- which tools were actually used
- which models handled which tasks
- how much was spent
- where tokens drained
- what required human approval
- which workflows were repeated
- whether hardware became justified
- whether the stack produced useful work
- what still needed cleanup

---

## Decision Receipt

This verdict is based on:

- [Evidence 1]
- [Evidence 2]
- [Evidence 3]

The verdict would change if:

- [Change trigger 1]
- [Change trigger 2]
- [Change trigger 3]

---

## Final Stackfax Verdict

[Final short verdict.]

Final recommendation: [Direct recommendation.]
