# Stackfax Business Automation Safety Audit Template

Report Type: Business Automation Safety Audit

Use Case: [Describe the business workflow, automation plan, or operational system being reviewed]

Overall Rating: [⭐ to ⭐⭐⭐⭐⭐]

Stack Score: [0–100]

Verdict: [Main business automation verdict]

Checked: [Date]

Recheck Trigger: [What should make this business recheck the automation stack?]

---

## Summary

[Short plain-English summary of whether the business automation stack is safe enough for the workflow.]

---

## Business Goal

The business wants to use Ai for:

* [Goal 1]
* [Goal 2]
* [Goal 3]

---

## Current Stack

The current or proposed stack includes:

* Tool/model/platform:
* Tool/model/platform:
* Business system:
* Customer data source:
* Human approval or review process:

---

## Main Verdict

[Clear recommendation.]

Possible verdict examples:

* Observe Only
* Draft With Approval
* Approval Gates Missing
* Credential Isolation Needed
* Customer Data Risk
* Production Not Ready
* Safe To Test
* Human Review Required
* Automation Overreach
* Business System Risk
* Process Before Automation
* Compliance System First

--- 

## Risk Flags

* [Risk flag 1]
* [Risk flag 2]
* [Risk flag 3]

Possible risk flags:

* Human Approval Required
* Customer Data Risk
* Credential Isolation Risk
* Production Not Ready
* Business System Risk
* Automation Overreach Risk
* Fragile UI Automation Risk
* Approval Gates Missing
* Run Receipts Missing
* Cost Visibility Missing
* Process Before Automation
* Agent ROI Unclear

---

## What Fits

This business automation stack fits well for:

* [Fit 1]
* [Fit 2]
* [Fit 3]

Possible fits:

* customer inquiry summaries
* draft email replies
* lead triage
* sales report explanations
* SEO/content drafts
* inventory status summaries
* internal research
* operations notes
* weekly business recaps
* missing-information flags
* review notes
* internal task preparation

---

## What May Be Unsafe

This stack may be unsafe if it can:

* [Unsafe action 1]
* [Unsafe action 2]
* [Unsafe action 3]

Possible unsafe actions:

* send customer messages automatically
* change customer records
* access payment tools
* issue refunds
* change inventory
* contact vendors
* post publicly
* delete or move business files
* modify production systems
* use shared credentials across workflows
* make claims without human review
* file, submit, or approve compliance-sensitive work without review

---

## Automation Level Verdict

Current recommended automation level: [Level 1 / Level 2 / Level 3 / Level 4]

Levels:

* Level 1: Observe Only
* Level 2: Draft With Approval
* Level 3: Limited Approved Actions
* Level 4: Production Automation

Notes:

[Explain why this level fits.]

Default recommendation:

Most early business Ai workflows should start at Level 1 or Level 2.

---

## Process Fit Review

Process fit: [Unclear / Basic / Good / Strong]

Notes:

[Explain whether the business process is clear enough to automate.]

A business process should be mapped before automation if it lacks:

* clear trigger
* clear owner
* clear input
* clear output
* clear done-state
* clear approval point
* clear exception path
* clear failure owner

Principle:

Do not automate chaos.

Diagnose the process first.

---

## Data Quality And Monday Morning Test

Data readiness: [Unclear / Basic / Good / Strong]

Notes:

[Explain whether the workflow has been tested against real-world messy data, not just clean demo data.]

Check whether the data includes:

* duplicate records
* missing fields
* inconsistent names
* old folders
* stale statuses
* edge cases
* real volume
* mixed formats
* incomplete customer records

The Monday morning test asks:

Can this workflow survive the business as it actually exists when nobody is watching it live?

Principle:

Clean demo data tests the logic.

Production data tests the business.

---

## Approval Gate Review

Risk level: [Low / Medium / High]

Human approval should be required before Ai can:

* send messages
* contact customers
* contact leads
* contact vendors
* post publicly
* edit customer records
* change inventory
* process payments
* issue refunds
* move or delete files
* access credentials
* modify production systems
* submit compliance-sensitive work
* make legal, financial, medical, or safety-sensitive claims

Notes:

[Explain which approval gates are missing or needed.]

---

## Customer Data Review

Risk level: [Low / Medium / High]

Customer or business data involved may include:

* customer names
* customer emails
* phone numbers
* addresses
* order history
* support history
* private notes
* sales records
* internal reports
* client files
* invoices
* payment status
* contracts
* operational records

Notes:

[Explain whether customer data is being handled safely.]

---

## Data Boundary Review

Data boundary status: [Unclear / Basic / Good / Strong]

Notes:

[Explain what the Ai system can see and what should stay restricted.]

Recommended boundaries:

* public data
* internal non-sensitive data
* customer data
* financial data
* credentials
* production systems
* compliance-sensitive records

The stack should define:

* what Ai can read
* what Ai can draft
* what Ai can modify
* what Ai can never touch
* what requires approval
* what must stay manual

---

## Credential Isolation Review

Risk level: [Low / Medium / High]

The stack should separate:

* personal accounts
* business accounts
* client accounts
* email sessions
* CRM access
* payment tools
* file storage
* API keys
* browser sessions
* automation accounts
* production admin access

Notes:

[Explain whether credentials and sessions are separated properly.]

---

## Forbidden Actions

The stack should not be allowed to do these without explicit human approval:

* send customer-facing messages
* issue refunds
* process payments
* change inventory
* delete files
* change production records
* submit official filings
* modify legal, financial, medical, or compliance-sensitive documents
* publish posts
* rotate or expose credentials
* contact vendors or customers
* make irreversible changes

Notes:

[Add any workflow-specific forbidden actions.]

---

## Fragile UI Automation Review

Risk level: [Low / Medium / High]

Notes:

[Explain whether the automation depends on clicking websites, reading screenshots, browser sessions, or unstable UI flows.]

Recommended controls:

* prefer APIs when available
* limit browser automation
* add human review before submit/click actions
* add screenshot/run receipt evidence
* add retry limits
* stop if buttons, labels, or page states change
* do not run fragile UI automation on payment, refund, or production systems without review

---

## Cost Visibility Review

Cost visibility: [Missing / Basic / Good / Strong]

Notes:

[Explain whether the business can see what the workflow costs and whether the cost produces useful work.]

A business automation cost receipt should show:

* model used
* tool/platform used
* API/router used
* number of retries
* fallback events
* approximate cost
* human review time
* cleanup required
* output produced
* business value created
* cheaper route next time

Principle:

Cost should leave a receipt.

--- 

## Production Readiness Review

Current verdict: [Demo Only / Safe To Test / Controlled Pilot / Production Candidate / Production Ready With Controls]

Before production use, the stack needs:

* written approval rules
* logs
* run receipts
* tool permission limits
* failure handling
* escalation rules
* access boundaries
* human owner for mistakes
* rollback plan
* budget caps
* 30-day recheck

Notes:

[Explain what is missing.]

---

## Run Receipt Review

Run receipt status: [Missing / Basic / Good / Strong]

A useful business automation run receipt should show:

* requested task
* business system involved
* model/tool used
* data source used
* actions taken
* records touched
* drafts created
* messages prepared
* what changed
* what failed
* approximate cost
* what needs human review
* next recommended action

Notes:

[Explain whether the business can prove what the automation did.]

---

## Context And Decision Receipt Review

Receipt status: [Missing / Basic / Good / Strong]

A useful business automation receipt should show:

* what context was used
* what customer or business data was included
* what context was excluded
* what assumptions were made
* why the verdict or action was recommended
* what evidence supports the recommendation
* what would change the verdict later

Notes:

[Explain whether the business can understand what information shaped the output and why the recommendation was made.]



## Agent ROI Review

Agent ROI status: [Unclear / Early Signal / Good / Strong]

Notes:

[Explain whether the automation is producing useful verified work, or just activity.]

Agent ROI should consider:

* time saved
* errors reduced
* response speed improved
* human supervision required
* cleanup required
* cost created
* risk introduced
* repeatability
* customer impact
* operational value

---

## Best First Business Workflow

The best first workflow is:

[One clear low-risk workflow.]

Example:

1. Pull a small set of non-sensitive business notes or public information.
2. Summarize the information.
3. Draft a short internal report.
4. Flag risks, missing data, or uncertain claims.
5. Ask for human approval before saving, sending, posting, or connecting tools.

Good first workflows are usually:

* internal
* read-only
* low-risk
* repeated often
* easy to verify
* useful even before full automation

---

## What Should Stay Manual For Now

These actions should stay manual until the stack proves reliability:

* [Manual action 1]
* [Manual action 2]
* [Manual action 3]

Examples:

* refunds
* payments
* customer record changes
* inventory changes
* production edits
* public posting
* compliance-sensitive submissions
* credential changes
* deletion of files or records

---

## What Would Improve The Score

To improve the score, add:

* [Improvement 1]
* [Improvement 2]
* [Improvement 3]
* [Improvement 4]

Possible improvements:

* written approval gates
* credential isolation
* customer data boundaries
* tool permission limits
* forbidden action list
* run receipt template
* context receipt template
* decision receipt template
* logging
* budget caps
* failure handling
* human review checkpoints
* sandbox test
* production-shaped data test
* 30-day recheck
* process map before automation

---

## Business Automation Recheck

Recheck this workflow if:

* customer data is added
* credentials are connected
* the workflow starts sending messages
* the workflow moves from draft-only to action-taking
* payments, refunds, inventory, or production systems are added
* model routing changes
* costs spike
* the business changes tools
* the workflow becomes scheduled or unattended
* a failure happens
* the stack moves from test to pilot or production

---

## Decision Receipt

This business automation verdict is based on:

* [Evidence 1]
* [Evidence 2]
* [Evidence 3]

The verdict would change if:

* [Change trigger 1]
* [Change trigger 2]
* [Change trigger 3]

---

## Stackfax Principle

Business automation should start with trust, not speed.

Observe first.

Draft second.

Approve third.

Automate last.

Compliance system first.

Ai assistant second.

The failure log is the trust layer.

---

## Final Business Automation Verdict

[Final short verdict.]

Final recommendation: [Direct recommendation.]
