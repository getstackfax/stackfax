# Stackfax Sample Business Automation Safety Audit

Report Type: Business Automation Safety Audit

Use Case: Small business wants to use Ai for customer inquiries, outreach drafts, sales report summaries, inventory checks, and internal operations support

Overall Rating: ⭐⭐⭐

Stack Score: 63/100

Verdict: Draft With Approval / Production Not Ready

## Summary

This stack has useful business automation potential, but it should not be allowed to take customer-facing or production actions yet.

The current best use is observe, summarize, draft, and report.

Human approval should remain required before anything is sent, posted, changed, purchased, refunded, deleted, or connected to production systems.

## Risk Flags

- Human Approval Required
- Customer Data Risk
- Credential Isolation Risk
- Production Not Ready
- Business System Risk
- Automation Overreach Risk

## What Fits

This stack fits well for:

- Customer inquiry summaries
- Drafting email replies
- Sales report explanations
- SEO/content drafts
- Inventory status summaries
- Internal research
- Operations notes
- Weekly business recaps

These are useful workflows as long as the Ai stack is not taking direct action without approval.

## What May Be Unsafe

This stack becomes risky if it can:

- Send customer messages automatically
- Change customer records
- Access payment tools
- Issue refunds
- Change inventory
- Contact vendors
- Post publicly
- Delete or move business files
- Modify production systems
- Use shared credentials across workflows

## Automation Level Verdict

Current recommended automation level: Level 2 — Draft With Approval

Allowed:

- Summarize
- Draft
- Flag issues
- Suggest next steps
- Prepare reports

Not allowed yet:

- Send
- Post
- Purchase
- Refund
- Delete
- Modify records
- Change systems
- Use credentials without approval

## Approval Gate Review

Risk level: High

Human approval should be required before the stack can:

- Send messages
- Contact customers
- Contact leads
- Contact vendors
- Post publicly
- Edit customer records
- Change inventory
- Process payments
- Issue refunds
- Move or delete files
- Access credentials
- Modify production systems

Approval gates should be written down before any real automation is connected.

## Customer Data Review

Risk level: Medium-High

The stack may interact with customer or business data.

Data that needs careful handling:

- Customer names
- Customer emails
- Phone numbers
- Addresses
- Order history
- Support history
- Private notes
- Sales records
- Internal reports
- Client files

The stack should only load customer data when the workflow clearly requires it.

## Credential Isolation Review

Risk level: High

The stack should not use one shared credential or browser session for everything.

Separate:

- Personal accounts
- Business accounts
- Client accounts
- Email sessions
- CRM access
- Payment tools
- File storage
- API keys
- Browser sessions

Do not give one agent broad access to all systems.

## Production Readiness Review

Current verdict: Production Not Ready

The stack is not ready for unsupervised production use.

Before production use, it needs:

- Written approval rules
- Logs
- Tool permission limits
- Failure handling
- Escalation rules
- Access boundaries
- Human owner for mistakes
- Rollback plan
- 30-day recheck

## Best First Business Workflow

Start with a low-risk workflow.

Recommended starter workflow:

1. Pull a small set of non-sensitive business notes or public information.
2. Summarize the information.
3. Draft a short internal report.
4. Flag risks, missing data, or uncertain claims.
5. Ask for human approval before saving, sending, posting, or connecting tools.

The goal is to prove usefulness before expanding permissions.

## What Would Improve The Score

This stack could move from 63/100 to 80+/100 by adding:

- Written approval gates
- Credential isolation
- Customer data boundaries
- Tool permission limits
- Logging
- Budget caps
- List of forbidden actions
- Failure handling
- Human review checkpoints
- 30-day recheck

## Stackfax Principle

Business automation should start with trust, not speed.

Observe first.

Draft second.

Approve third.

Automate last.

## Final Stackfax Verdict

This stack has real business value, but it is not ready for autonomous action.

Use it to summarize, draft, report, and flag issues first.

Final recommendation: keep the workflow human-approved until approval gates, credential isolation, and production safeguards are documented.
