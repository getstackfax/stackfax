Stackfax Manual Report Production Checklist

This checklist defines the manual production process for creating early Stackfax reports.

The goal is to make every manual report clear, safe, useful, repeatable, and trust-first before Stackfax becomes more automated.

⸻

Core Goal

Turn a user intake into a useful Stackfax report without exposing private data, overpromising results, or creating unnecessary operational risk.

Manual reports are not just delivery work.

They are how Stackfax learns what the standard should become.

⸻

Before Starting

Confirm:

* report request was received
* intake form was completed
* contact email is available
* report type is clear or can be inferred
* no unsafe private information was submitted
* delivery window is understood
* user expectations are clear
* payment status is clear if this is a paid report
* the user’s main decision is identifiable

The report should answer a real decision.

If the user’s goal is unclear, ask a follow-up before writing the report.

⸻

Intake Safety Review

Check that the intake does not include:

* passwords
* API keys
* recovery codes
* payment details
* wallet information
* private keys
* seed phrases
* private customer data
* private legal documents
* private medical documents
* private financial documents
* financial account information
* identity documents
* employee records
* client confidential files
* sensitive personal information
* private inbox exports
* password manager exports
* production credentials
* source code secrets

If unsafe information is included:

1. Do not use the sensitive information.
2. Do not copy it into the report.
3. Do not store it in the public repo.
4. Ask the user to remove it.
5. Request a cleaned-up intake.
6. Resume only after the intake is safe.

Core rule:

Stackfax reviews the stack problem, not the user’s private life.

⸻

Choose Report Type

Select the best-fit report type.

Possible report types:

* Free Mini Report
* Stackfax Quick Report
* Hardware Verdict
* Token Burn Audit
* OpenClaw Starter Stack Check
* Model Subscription Fit Check
* Business Automation Safety Audit
* Vendor Stack Verdict
* Beginner To Builder Stack Path
* Pro Report Beta Preview
* Executive Audit

If multiple report types apply, choose the main report type and mention secondary concerns inside the report.

Examples:

* Hardware question plus token cost concern → Hardware Verdict with Token Burn notes
* OpenClaw setup plus safety concern → OpenClaw Starter Stack Check with Approval Gate review
* Business automation plus customer data → Business Automation Safety Audit with Data Boundary review
* Multiple subscriptions plus unclear workflow → Model Subscription Fit Check with Workflow Fit review

⸻

Choose Template

Use the closest template:

* templates/free-mini-report-template.md
* templates/stackfax-quick-report-template.md
* templates/token-burn-audit-template.md
* templates/model-subscription-fit-template.md
* templates/business-automation-safety-audit-template.md
* templates/pro-report-beta-preview-template.md

If no perfect template exists, use the Quick Report template and adapt it.

Do not invent a new structure unless the existing templates cannot answer the user’s decision.

⸻

Draft Report

Draft the report with:

* report type
* use case
* overall rating
* Stack Score
* main verdict
* summary
* user goal
* current stack
* risk flags
* what fits
* what may be overkill
* hardware fit
* token burn review
* model subscription fit
* workflow fit
* approval gate review
* run receipt review
* cost visibility review
* privacy or credential isolation notes
* best next move
* upgrade path
* 30-day recheck guidance
* final recommendation

The report should be practical, not performative.

The user should finish knowing what to do next.

⸻

Rating And Score Check

Confirm that the rating and score match the report.

Use this rough guide:

* 0–39: poor fit
* 40–59: risky or unclear fit
* 60–74: usable starter stack
* 75–89: strong stack
* 90–100: excellent stack

Do not give a high score just because the stack is expensive, complex, local, or technically impressive.

Reward:

* fit
* clarity
* safety
* cost discipline
* workflow definition
* approval gates
* run receipts
* realistic upgrade path

Penalize:

* unclear workflow
* overbuilt hardware
* tool sprawl
* subscription overlap
* missing approval gates
* weak data boundaries
* no cost visibility
* no run receipts
* production automation before readiness

Core rule:

The score should reward fit, not flex.

⸻

Risk Flag Check

Add only relevant risk flags.

Possible risk flags:

* Hardware Overbuild Risk
* Token Burn Risk
* Context Bloat Risk
* Model Routing Risk
* Silent Escalation Risk
* Subscription Overlap Risk
* Credential Isolation Risk
* Data Boundary Risk
* Prompt Governance Risk
* Fragile UI Automation Risk
* Approval Gates Missing
* Run Receipts Missing
* Cost Visibility Missing
* Evaluation Layer Missing
* Agent ROI Unclear
* Human Approval Required
* Customer Data Risk
* Production Not Ready
* Vendor Stack Overkill Risk
* Tool Loop Burn
* Business System Risk
* Workflow Fit Unclear
* Process Before Automation
* Agent Setup Overbuild Risk

A risk flag should help the user understand what to fix.

Do not add risk flags just to make the report look serious.

⸻

Workflow Fit Check

Confirm whether the workflow is defined enough to evaluate.

A good workflow has:

* clear trigger
* clear input
* clear output
* clear owner
* clear done-state
* clear approval point
* clear failure path
* clear recheck trigger

If the workflow is unclear, say so.

Possible workflow verdicts:

* Clear
* Basic
* Needs Narrowing
* Workflow Fit Unclear
* Ready To Test
* Production Not Ready

Core rule:

Do not automate chaos. Diagnose the process first.

⸻

Approval Gate Check

If the stack touches business systems, customer data, credentials, files, payments, wallets, financial accounts, public posting, or production workflows, include human approval guidance.

Human approval should usually be required before Ai can:

* send messages
* contact customers
* contact leads
* contact vendors
* post publicly
* move or delete files
* change settings
* connect credentials
* access wallets or financial accounts
* edit customer records
* change inventory
* process payments
* issue refunds
* modify production systems
* submit compliance-sensitive work
* make legal, financial, medical, or safety-sensitive claims

Default starter pattern:

Observe, summarize, draft, report, and ask for approval.

⸻

Run Receipt Check

If the report involves agents, automation, tools, business workflows, or production systems, check whether the user has run receipts.

A run receipt should help prove:

* what task ran
* what model or tool was used
* what context was used
* what data was accessed
* what action was proposed
* what action was executed
* what failed
* what was skipped
* what human approved
* what changed afterward

Possible run receipt verdicts:

* Missing
* Basic
* Good
* Strong
* Required Before Scaling

Core rule:

Agent output is a claim. A run receipt is evidence.

⸻

Cost Visibility Check

If the user has subscriptions, APIs, routers, local hardware, or agent loops, check whether cost visibility exists.

The user should know:

* which subscription was used
* which API or provider was used
* which model handled the task
* whether fallback happened
* approximate cost per run
* which workflow created the most cost
* which paid tool should be kept, paused, or replaced

Possible cost visibility verdicts:

* Missing
* Basic
* Good
* Strong

Core rule:

Cost visibility turns token burn from a surprise into a management problem.

⸻

Safety Language Check

Make sure the report does not claim to be:

* legal advice
* financial advice
* trading advice
* medical advice
* security certification
* compliance certification
* guaranteed cost savings
* guaranteed business outcome
* guaranteed automation safety
* guaranteed model performance
* guaranteed revenue improvement
* guaranteed risk elimination

Use practical stack guidance, not professional guarantees.

Stackfax can identify risk, workflow fit, cost concerns, and approval needs.

Stackfax should not promise outcomes it cannot guarantee.

⸻

Public Language Check

Before delivery, check that the report uses mature public language.

Use:

* beginner
* early builder
* first-time builder
* builder
* expert
* operator
* team
* small business owner

Avoid:

* noob
* first Ai report card
* fake testimonials
* fake urgency
* guaranteed savings
* guaranteed results
* overclaiming automation
* pretending Stackfax is fully automated before it is

⸻

Clarity Check

Before delivery, confirm:

* main verdict is easy to understand
* best next move is specific
* the user knows what not to do yet
* the report matches the user’s skill level
* the report avoids unnecessary jargon
* the report does not shame beginners
* the report does not slow down experts
* the report gives a useful next step
* safety warnings are clear without sounding alarmist
* secondary concerns are included without overwhelming the main verdict

A good report should feel like a decision aid, not a lecture.

⸻

Delivery Check

Before sending:

* subject line is clear
* report type is included
* main verdict is near the top
* safety note is included when needed
* delivery format is readable
* optional feedback request is included
* no private sensitive data is repeated unnecessarily
* the user’s main question is answered
* the next step is obvious

⸻

Suggested Delivery Email

Subject:

Your Stackfax Quick Report is ready

Body structure:

* thank the user
* state the report type
* state the main verdict
* include or link the report
* mention any important safety warning
* ask for optional feedback
* mention Stackfax is early and improving

Example:

Thanks for sending your stack.

Your Stackfax Quick Report is ready.

Main verdict: [Verdict]

The report includes the rating, Stack Score, risk flags, workflow notes, and best next move.

Stackfax is still early and reports are currently manual, so feedback is very useful.

After you read it, I’d appreciate knowing:

- Was the verdict clear?
- Was the next move useful?
- What part helped most?
- What felt confusing?

Feedback Request

Ask:

* Was the verdict clear?
* Was the next move useful?
* What part helped most?
* What felt confusing?
* Would you want a deeper Pro Report?
* What should Stackfax check next time?
* Did the report miss anything important?
* Did the risk flags feel accurate?
* Did the score feel fair?

Do not turn feedback into a testimonial unless the user gives clear permission.

⸻

After Delivery

Log internal notes:

* report type
* main verdict
* score
* risk flags
* template used
* what was hard to answer
* what template section needs improvement
* whether the user gave feedback
* whether the report created a new intake question
* whether the report created a new risk flag
* whether the report created a new sample scenario
* whether follow-up is needed

Do not store sensitive private information in the public repo.

⸻

Internal Improvement Loop

Every manual report should improve the Stackfax standard.

After each report, ask:

* Did the intake ask the right questions?
* Did the template fit the user’s decision?
* Did the score feel justified?
* Did any section feel missing?
* Did the user need a report type that does not exist yet?
* Did the report reveal a new risk flag?
* Did the report reveal a better scoring rule?
* Did the report reveal a better public explanation?
* Did the report reveal a better paid offer?

Manual review should improve the system, not just finish the current report.

⸻

Refusal Or Pause Cases

Pause, refuse, or narrow the request if the report would require:

* handling secrets
* reviewing private legal documents
* reviewing private medical documents
* processing identity documents
* accessing wallets
* accessing financial accounts
* accessing passwords or API keys
* making legal, medical, financial, or compliance judgments
* helping with unsafe automation
* helping bypass platform rules
* enabling fraud, deception, evasion, or harm
* evaluating customer records without proper safeguards

Stackfax can often still help by reviewing the stack shape, workflow boundary, or public/non-sensitive setup.

⸻

Final Rule

Manual reports are training data for the Stackfax standard.

Every report should make the next report easier, clearer, safer, and more useful.

Protect the user.

Clarify the stack.

Leave a better standard behind.
