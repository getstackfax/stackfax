# Stackfax Sample Business Automation Safety Audit

Report Type: Stackfax Quick Report / Business Automation Safety Audit

Use Case: Small business wants to use Ai for customer inquiries, outreach drafts, sales report summaries, inventory checks, and internal operations support

Overall Rating: ⭐⭐⭐

Stack Score: 63/100

Verdict: Draft With Approval / Production Not Ready

---

## Summary

This stack has useful business automation potential, but it should not be allowed to take customer-facing or production actions yet.

The current best use is:

observe → summarize → draft → report → human approval

Human approval should remain required before anything is sent, posted, changed, purchased, refunded, deleted, or connected to production systems.

---

## Main Verdict

The stack can help the business move faster, but it should not own the outcome yet.

The user should treat Ai as an assistant layer, not an autonomous operator.

The safest first move is to prove low-risk internal workflows before connecting tools that touch customers, money, credentials, inventory, files, or production systems.

---

## Risk Flags

- Human Approval Required
- Customer Data Risk
- Credential Isolation Risk
- Production Not Ready
- Business System Risk
- Automation Overreach Risk
- Approval Gates Missing
- Run Receipts Missing
- Agent ROI Unclear

---

## What Fits

This stack fits well for:

- customer inquiry summaries
- drafting email replies
- sales report explanations
- SEO/content drafts
- inventory status summaries
- internal research
- operations notes
- weekly business recaps
- missing-information flags
- review notes
- internal task preparation

These are useful workflows as long as the Ai stack is not taking direct action without approval.

---

## What May Be Unsafe

This stack becomes risky if it can:

- send customer messages automatically
- change customer records
- access payment tools
- issue refunds
- change inventory
- contact vendors
- post publicly
- delete or move business files
- modify production systems
- use shared credentials across workflows
- make claims without human review
- file, submit, or approve compliance-sensitive work without review

---

## Automation Level Verdict

Current recommended automation level: Level 2 — Draft With Approval

Allowed:

- summarize
- draft
- classify
- flag issues
- suggest next steps
- prepare reports
- identify missing information

Not allowed yet:

- send
- post
- purchase
- refund
- delete
- modify records
- change systems
- use credentials without approval
- contact customers or vendors without approval

Most early business Ai workflows should start at Level 1 or Level 2.

---

## Process Fit Review

Process fit: Basic

The business has useful candidate workflows, but the process should be mapped before deeper automation.

A business process should be mapped if it lacks:

- clear trigger
- clear owner
- clear input
- clear output
- clear done-state
- clear approval point
- clear exception path
- clear failure owner

Principle:

Do not automate chaos.

Diagnose the process first.

---

## Approval Gate Review

Risk level: High

Human approval should be required before the stack can:

- send messages
- contact customers
- contact leads
- contact vendors
- post publicly
- edit customer records
- change inventory
- process payments
- issue refunds
- move or delete files
- access credentials
- modify production systems
- submit compliance-sensitive work
- make legal, financial, medical, or safety-sensitive claims

Approval gates should be written down before any real automation is connected.

---

## Customer Data Review

Risk level: Medium-High

The stack may interact with customer or business data.

Data that needs careful handling:

- customer names
- customer emails
- phone numbers
- addresses
- order history
- support history
- private notes
- sales records
- internal reports
- client files
- invoices
- payment status
- contracts
- operational records

The stack should only load customer data when the workflow clearly requires it.

---

## Data Boundary Review

Data boundary status: Basic

The user should define what the Ai system can see, draft, modify, and never touch.

Recommended boundaries:

- public data
- internal non-sensitive data
- customer data
- financial data
- credentials
- production systems
- compliance-sensitive records

The stack should define:

- what Ai can read
- what Ai can draft
- what Ai can modify
- what Ai can never touch
- what requires approval
- what must stay manual

---

## Credential Isolation Review

Risk level: High

The stack should not use one shared credential or browser session for everything.

Separate:

- personal accounts
- business accounts
- client accounts
- email sessions
- CRM access
- payment tools
- file storage
- API keys
- browser sessions
- admin accounts

Do not give one agent broad access to all systems.

Credentials should not live inside memory, prompts, notes, reports, or shared context files.

---

## Production Readiness Review

Current verdict: Production Not Ready

The stack is not ready for unsupervised production use.

Before production use, it needs:

- written approval rules
- logs
- run receipts
- tool permission limits
- failure handling
- escalation rules
- access boundaries
- human owner for mistakes
- rollback plan
- 30-day recheck

Production readiness is not just whether the workflow works once.

It is whether the workflow can fail safely.

---

## Run Receipt Review

Run receipts: Missing / Needed

Every meaningful business automation should leave evidence showing:

- what triggered the workflow
- what data was used
- which model handled the task
- which tools were called
- what was drafted
- what was approved
- what was sent or changed
- what failed
- what needs review
- who owns the next step

If the business cannot reconstruct what happened, the workflow is not ready for trust-sensitive automation.

---

## Agent ROI Review

Agent ROI: Unclear

The stack should not be judged by activity alone.

Useful business automation should reduce work without adding more supervision, cleanup, risk, or hidden cost.

Track:

- time saved
- drafts accepted
- drafts rewritten
- issues caught
- missed follow-ups reduced
- support tickets routed
- manual steps removed
- cost per workflow run
- review burden
- errors created

Agent ROI is useful work minus supervision, cost, risk, and cleanup.

---

## Forbidden Actions

Until the stack is proven, it should not:

- send customer messages without review
- issue refunds
- edit payment records
- change inventory
- update customer records automatically
- delete files
- publish content
- contact vendors
- access wallets
- access financial accounts
- use credentials without approval
- modify production systems
- submit compliance-sensitive work

Forbidden actions should be written down before tools are connected.

---

## Best First Business Workflow

Start with a low-risk workflow.

Recommended starter workflow:

1. Pull a small set of non-sensitive business notes or public information.
2. Summarize the information.
3. Draft a short internal report.
4. Flag risks, missing data, or uncertain claims.
5. Ask for human approval before saving, sending, posting, or connecting tools.

The goal is to prove usefulness before expanding permissions.

---

## What Would Improve The Score

This stack could move from 63/100 to 80+/100 by adding:

- written approval gates
- credential isolation
- customer data boundaries
- tool permission limits
- run receipts
- budget caps
- list of forbidden actions
- failure handling
- escalation rules
- human review checkpoints
- 30-day recheck

---

## Stackfax Principle

Business automation should start with trust, not speed.

Observe first.

Draft second.

Approve third.

Automate last.

Compliance system first.

Ai assistant second.

---

## Final Stackfax Verdict

This stack has real business value, but it is not ready for autonomous action.

Use it to summarize, draft, report, and flag issues first.

Keep the workflow human-approved until approval gates, credential isolation, data boundaries, run receipts, and production safeguards are documented.

Final recommendation:

Draft with approval. Do not allow autonomous production action yet.
