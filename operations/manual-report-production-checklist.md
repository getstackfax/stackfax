# Stackfax Manual Report Production Checklist

This checklist defines the manual production process for creating early Stackfax reports.

The goal is to make every manual report clear, safe, useful, and repeatable before Stackfax becomes more automated.

## Core Goal

Turn a user intake into a useful Stackfax report without exposing private data, overpromising results, or creating unnecessary operational risk.

## Before Starting

Confirm:

- Report request was received
- Intake form was completed
- Contact email is available
- Report type is clear or can be inferred
- No unsafe private information was submitted
- Delivery window is understood
- User expectations are clear

## Intake Safety Review

Check that the intake does not include:

- Passwords
- API keys
- Recovery codes
- Payment details
- Wallet information
- Private customer data
- Private legal documents
- Private financial account information
- Sensitive personal information

If unsafe information is included:

1. Do not use the sensitive information.
2. Ask the user to remove it.
3. Request a cleaned-up intake.
4. Resume only after the intake is safe.

## Choose Report Type

Select the best-fit report type:

- Free Mini Report
- Stackfax Quick Report
- Mac Mini Hardware Verdict
- Token Burn Audit
- OpenClaw Starter Stack Check
- Model Subscription Fit Check
- Business Automation Safety Check
- Vendor Stack Verdict
- Noob To Expert Stack Path

If multiple report types apply, choose the main report type and mention secondary concerns inside the report.

## Choose Template

Use the closest template:

- templates/free-mini-report-template.md
- templates/stackfax-quick-report-template.md
- templates/token-burn-audit-template.md
- templates/model-subscription-fit-template.md
- templates/business-automation-safety-audit-template.md
- templates/pro-report-beta-preview-template.md

If no perfect template exists, use the Quick Report template and adapt it.

## Draft Report

Draft the report with:

- Report type
- Use case
- Overall rating
- Stack Score
- Main verdict
- Summary
- User goal
- Current stack
- Risk flags
- What fits
- What may be overkill
- Hardware fit
- Token burn review
- Model subscription fit
- Approval gate review
- Privacy or credential isolation notes
- Best next move
- Upgrade path
- 30-day recheck guidance
- Final recommendation

## Rating And Score Check

Confirm that the rating and score match the report.

Use the rough guide:

- 0–39: Poor fit
- 40–59: Risky or unclear fit
- 60–74: Usable starter stack
- 75–89: Strong stack
- 90–100: Excellent stack

Do not give a high score just because the stack is expensive or complex.

Reward:

- Fit
- Clarity
- Safety
- Cost discipline
- Upgrade path

## Risk Flag Check

Add only relevant risk flags.

Possible risk flags:

- Hardware Overbuild Risk
- Token Burn Risk
- Context Bloat Risk
- Silent Escalation Risk
- Subscription Overlap Risk
- Credential Isolation Risk
- Fragile UI Automation Risk
- Human Approval Required
- Customer Data Risk
- Production Not Ready
- Vendor Stack Overkill Risk
- Tool Loop Burn
- Business System Risk

## Safety Language Check

Make sure the report does not claim to be:

- Legal advice
- Financial advice
- Trading advice
- Security certification
- Compliance certification
- Guaranteed cost savings
- Guaranteed business outcome
- Guaranteed automation safety
- Guaranteed model performance

Use practical stack guidance, not professional guarantees.

## Approval Gate Check

If the stack touches business systems, customer data, credentials, files, payments, wallets, financial accounts, public posting, or production workflows, include human approval guidance.

Human approval should usually be required before:

- Sending messages
- Contacting customers
- Posting publicly
- Moving or deleting files
- Changing settings
- Connecting credentials
- Accessing wallets or financial accounts
- Editing customer records
- Changing inventory
- Processing payments
- Modifying production systems

## Clarity Check

Before delivery, confirm:

- Main verdict is easy to understand
- Best next move is specific
- The user knows what not to do yet
- The report matches the user’s skill level
- The report avoids unnecessary jargon
- The report does not shame beginners
- The report does not slow down experts
- The report gives a useful next step

## Delivery Check

Before sending:

- Subject line is clear
- Report type is included
- Main verdict is near the top
- Safety note is included when needed
- Delivery format is readable
- Optional feedback request is included
- No private sensitive data is repeated unnecessarily

## Suggested Delivery Email

Subject:

Your Stackfax Quick Report is ready

Body structure:

- Thank the user
- State the report type
- State the main verdict
- Include or link the report
- Mention any important safety warning
- Ask for optional feedback
- Mention Stackfax is early and improving

## Feedback Request

Ask:

- Was the verdict clear?
- Was the next move useful?
- What part helped most?
- What felt confusing?
- Would you want a deeper Pro Report?
- What should Stackfax check next time?

## After Delivery

Log internal notes:

- Report type
- Main verdict
- Score
- Risk flags
- Template used
- What was hard to answer
- What template section needs improvement
- Whether the user gave feedback

Do not store sensitive private information in the public repo.

## Final Rule

Manual reports are training data for the Stackfax standard.

Every report should make the next report easier, clearer, and safer.
