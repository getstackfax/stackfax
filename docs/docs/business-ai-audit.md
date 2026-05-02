# Business Ai Audit

Business Ai work should start with the workflow, not the agent.

For most businesses, the goal is not to “add Ai.” The goal is to reduce friction, risk, cost, delay, and manual cleanup in a real operating process.

> Compliance system first, Ai assistant second.

---

## Core Principle

A business should not add autonomous Ai on top of a messy workflow and expect the mess to disappear.

First, define the system:

- what work happens
- who owns it
- what data is required
- where mistakes happen
- what must be reviewed
- what requires approval
- what evidence must be kept
- what “done” means

Only then should Ai be added.

---

## What a Business Ai Audit Checks

A Stackfax Business Ai Audit looks at whether the business has the operating layer needed before automation.

Key checks include:

- **Workflow fit:** what job is Ai supposed to improve?
- **System readiness:** are the current tools organized enough to support automation?
- **Data quality:** is the input clean, structured, and available?
- **Permission control:** what can the Ai read, write, send, edit, or trigger?
- **Approval gates:** where must a human approve before action?
- **Audit trail:** can the business see what happened, when, why, and by whom?
- **Exception handling:** what happens when the Ai is uncertain or wrong?
- **Cost control:** will automation reduce cost, or create hidden token/tool spend?
- **Risk control:** could the workflow create compliance, financial, privacy, or reputation risk?
- **Outcome measurement:** how will the business know the system worked?

---

## Compliance Workflows

Regulated or compliance-heavy workflows need extra caution.

Examples include:

- accounting
- tax filing
- payroll
- legal intake
- insurance
- healthcare administration
- customer data handling
- financial reporting
- contract review
- regulated client communications

In these workflows, Ai should usually assist the review process rather than replace responsibility.

Useful Ai roles include:

- anomaly detection
- missing-information flags
- messy-record summaries
- client follow-up drafts
- review notes
- reconciliation assistance
- document classification
- checklist generation
- exception queues

Risky Ai roles include:

- filing without review
- sending regulated communications without approval
- changing records without logs
- making final compliance decisions
- handling sensitive data without access controls
- using private customer data in unapproved tools

---

## Example: Small Accounting Practice

A small accounting practice preparing for Making Tax Digital should not start by asking for an autonomous Ai filing agent.

The first layer should be boring and compliant:

- HMRC-compatible MTD software
- digital records
- bank feeds
- transaction categorization
- quarterly update workflow
- client review process
- approval before filing
- audit trail

Then Ai can sit on top of that system for:

- spotting anomalies
- summarizing messy client records
- flagging missing receipts or missing explanations
- drafting client follow-ups
- preparing review notes
- identifying transactions that need human attention

The correct stack is not:

> autonomous Ai agent files everything

The correct stack is closer to:

> compliant workflow plus Ai-assisted review layer

---

## Approval Gates

Approval gates are one of the most important parts of a business Ai stack.

A business should define which actions are:

### Safe to automate

Examples:

- summarize internal notes
- classify documents
- draft emails
- extract fields from records
- flag anomalies
- prepare reports for review

### Require human approval

Examples:

- send external email
- update customer records
- create invoices
- submit filings
- move money
- change legal/compliance documents
- publish public content
- contact customers about sensitive issues

### Should not be automated yet

Examples:

- final compliance decisions
- unsupervised tax filing
- account access changes
- broad payment authority
- irreversible customer-data changes
- actions without logs or rollback

---

## Audit Trail

A useful business Ai system should leave evidence.

The business should be able to answer:

- what did the Ai read?
- what did it change?
- what did it recommend?
- what did it send?
- who approved it?
- what model/tool was used?
- what failed?
- what was corrected?
- what should be improved next time?

If the system cannot explain what happened, it is not ready for high-trust business use.

---

## Stackfax Principle

For business workflows, Ai should make the system more reliable, not just more impressive.

The best first business Ai use cases are usually:

- boring
- repeated
- easy to verify
- expensive when missed
- attached to a clear workflow
- safe with human review

> Boring compliant plumbing before agents.
