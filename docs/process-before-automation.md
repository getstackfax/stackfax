# Stackfax Process Before Automation

Process Before Automation is the Stackfax doctrine for checking whether the underlying workflow is clear enough before adding Ai agents, automations, tools, model routing, or scheduled actions.

The goal is to prevent businesses, builders, and teams from automating broken handoffs, unclear ownership, messy data, or unsafe decisions.

⸻

Core Idea

Do not automate chaos.

Diagnose the process first.

Ai can speed up a workflow, but it can also speed up confusion, mistakes, cost, and cleanup.

Core rule:

Process first. Automation second.

⸻

Core Question

Is the process clear enough that automation would improve it instead of hiding the mess?

If the process is unclear, the next move is process mapping, not more automation.

⸻

Why This Matters

Many automation failures are not model failures.

They are process failures.

The stack may have:

* strong models
* good tools
* agent framework
* local hardware
* browser automation
* memory
* workflow prompts
* scheduled tasks

But if the business process is unclear, the automation may still fail.

Stackfax verdict:

Ai does not fix chaos. It scales chaos.

⸻

What A Process Includes

A business or workflow process should define:

* owner
* trigger
* input
* source of truth
* required data
* steps
* handoffs
* decision points
* approval points
* output
* definition of done
* exception path
* failure owner
* evidence to keep
* review schedule

If these are missing, automation may make the workflow faster but less trustworthy.

⸻

Process Questions

Before automating, ask:

* Who owns this workflow?
* What starts it?
* What input is required?
* Where does the input come from?
* What data is trusted?
* What happens manually today?
* Where does work get stuck?
* Where do mistakes happen?
* What decision is being made?
* What should require human approval?
* What should never be automated?
* What evidence proves the work was done?
* What happens when something is missing, wrong, or unclear?

These questions come before tool choice.

⸻

Bad Automation Starting Point

A weak starting point sounds like:

* We need Ai for sales.
* We need an agent for support.
* We need to automate follow-up.
* We need Ai to run operations.
* We need a chatbot.
* We need a dashboard.
* We need OpenClaw connected to everything.
* We need to replace manual work.

These may become valid later.

But first, define the process.

⸻

Better Automation Starting Point

A stronger starting point sounds like:

* We miss lead follow-ups after the first reply.
* Intake forms are incomplete and delay quoting.
* Support tickets need triage before human review.
* Weekly sales reports take too long to summarize.
* Customer reply drafts need faster first pass.
* Inventory alerts need a daily summary before reorder decisions.
* We need receipts showing what the agent touched.

These are process problems.

They can be mapped, tested, and improved.

⸻

Common Process Failures

Unclear Ownership

No one owns the workflow.

Warning signs:

* unclear who reviews output
* unclear who fixes mistakes
* unclear who approves actions
* unclear who receives alerts
* unclear who updates the process

Stackfax verdict:

If no one owns the workflow, no one owns the automation.

⸻

Messy Input

The automation starts with bad or incomplete data.

Warning signs:

* missing fields
* inconsistent formats
* unclear source of truth
* duplicate records
* outdated information
* screenshots instead of structured data
* private data mixed with public data

Stackfax verdict:

Automation quality cannot outrun input quality.

⸻

Weak Handoffs

Work breaks when moving from one person, tool, channel, or system to another.

Warning signs:

* no handoff owner
* no status label
* no next action
* no receipt
* no deadline
* no escalation path
* no approval state

Stackfax verdict:

Revenue leaks live in the handoffs.

⸻

No Definition Of Done

The workflow has no clear completion state.

Warning signs:

* agent says “done” without evidence
* output cannot be reviewed
* no expected format exists
* no acceptance criteria
* no human sign-off
* no receipt
* no next action

Stackfax verdict:

“Done” should mean operationally complete, not just agent-confident.

⸻

No Exception Path

The workflow assumes everything goes right.

Warning signs:

* no plan for missing input
* no plan for uncertain output
* no stop condition
* no escalation rule
* no rollback
* no failure owner
* no manual fallback

Stackfax verdict:

Exceptions are not edge cases. They are the operating layer.

⸻

Automation Readiness Levels

Level 1: Process Unclear

The workflow is not ready for automation.

Best next move:

* map the process
* define owner
* define input/output
* identify approval points
* identify what should not be automated

Verdict:

Process Before Automation

⸻

Level 2: Assistive Ai Ready

The workflow can use Ai for low-risk support.

Allowed:

* summarize
* classify
* draft
* flag missing info
* prepare reports
* suggest next actions

Not allowed:

* send
* post
* delete
* purchase
* modify production systems
* change customer records without approval

Verdict:

Safe To Assist

⸻

Level 3: Draft With Approval

Ai can draft outputs that a human reviews.

Allowed:

* draft emails
* draft replies
* draft reports
* draft checklists
* draft summaries
* prepare customer follow-up notes

Requires:

* human approval
* clear source data
* review checklist
* run receipt

Verdict:

Draft With Approval

⸻

Level 4: Limited Automation

Ai or automation can take narrow actions inside a defined process.

Requires:

* scoped permissions
* clear rule
* cost cap
* failure path
* logs or receipts
* human override
* rollback
* exception handling

Verdict:

Limited Approved Actions

⸻

Level 5: Production Automation

Ai operates in real business workflows.

Requires:

* tested process
* governance
* monitoring
* approval policy
* credential isolation
* customer-data boundaries
* run receipts
* escalation
* rollback
* owner accountability
* recheck schedule

Verdict:

Production Review Required

Most early stacks should not start here.

⸻

Business Examples

Lead Follow-Up

Process question:

Where do leads get lost?

Ai role:

* summarize inquiry
* classify lead type
* draft follow-up
* flag missing info
* prepare next step

Approval:

* human approves before sending

Do not start with:

Agent automatically contacts every lead.

⸻

Customer Support

Process question:

Which support questions are safe to draft, and which require escalation?

Ai role:

* summarize ticket
* classify issue
* draft reply
* flag uncertainty
* recommend escalation

Approval:

* human approves customer-facing reply

Do not start with:

Agent closes support conversations automatically.

⸻

Inventory

Process question:

What data source is trusted for inventory state?

Ai role:

* summarize inventory changes
* flag anomalies
* prepare reorder recommendation

Approval:

* human approves reorder or vendor contact

Do not start with:

Agent buys inventory automatically.

⸻

Reporting

Process question:

Which numbers are source-of-truth, and what conclusion is allowed?

Ai role:

* explain trends
* summarize changes
* flag anomalies
* draft report

Approval:

* human reviews before business decision

Do not start with:

Agent makes final accounting or financial decision.

⸻

What Ai Should Do First

Good first Ai roles:

* summarize
* classify
* draft
* compare
* flag
* extract
* prepare
* explain
* route
* create checklists
* generate review notes

These roles help the process without granting too much authority.

⸻

What Should Wait

Do not automate these too early:

* final customer replies
* refunds
* payments
* purchases
* legal decisions
* compliance filings
* inventory changes
* public posts
* credential changes
* customer record changes
* production changes
* financial account actions
* wallet actions

These require strong process controls, approval gates, and receipts.

⸻

Process And Agent ROI

A process should produce measurable improvement.

Agent ROI should ask:

* Did response time improve?
* Did missed follow-ups decrease?
* Did manual cleanup decrease?
* Did review quality improve?
* Did cost stay controlled?
* Did risk stay bounded?
* Did the next step become clearer?
* Did the run receipt make review easier?

If the process does not improve, automation may be theater.

Core rule:

Agent ROI is not activity. It is verified useful work.

⸻

Process And Run Receipts

Process improvement needs evidence.

A run receipt should show:

* what process ran
* what input was used
* what output was produced
* what system was touched
* what changed
* what approval was requested
* what failed
* what needs review next

Without receipts, it is hard to know whether the process improved.

⸻

Common Verdicts

Possible verdicts include:

* Process Before Automation
* Workflow Fit Unclear
* Safe To Assist
* Draft With Approval
* Approval Gates Needed
* Run Receipts Required
* Process Owner Missing
* Source Of Truth Missing
* Exception Path Missing
* Production Not Ready
* Business Automation Safety Audit Recommended

⸻

Common Risk Flags

Process reviews may include:

* Process Before Automation
* Workflow Fit Unclear
* Approval Gates Missing
* Run Receipts Required
* Agent ROI Unclear
* Customer Data Risk
* Credential Isolation Risk
* Communication Channel Risk
* Fragile UI Automation Risk
* Cost Visibility Missing
* Production Not Ready
* Agentic Trap Risk

⸻

What Would Improve The Score

A process can improve by adding:

* workflow owner
* source of truth
* clean input
* defined output
* definition of done
* approval gates
* exception path
* run receipts
* escalation owner
* forbidden actions
* review checklist
* cost boundary
* repeat test
* 30-day process review

The goal is not to automate faster.

The goal is to make the process trustworthy enough to automate.

⸻

Example Report Language

Use language like:

This workflow is not ready for automation yet.

The process needs clearer ownership, input requirements, approval points, exception handling, and run receipts before Ai should take action.

Start with assistive Ai: summarize, classify, draft, and flag missing information for human review.

Short version:
⸻

Stackfax Principle

Process first.

Automation second.

Do not automate chaos.

Do not let Ai scale a broken handoff.

⸻

Final Rule

Before asking what to automate, ask what process needs to become clearer.

The safest automation starts with a workflow that already knows its owner, input, output, approval gate, failure path, and definition of done.
