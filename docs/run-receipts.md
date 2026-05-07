# Run Receipts

A production agent needs a run receipt, not just logs.

Logs are useful for engineers.

Run receipts are useful for owners, operators, reviewers, and future agents.

A run receipt explains what happened in plain language:

* what was attempted
* what inputs were used
* what model/config ran
* what tools were touched
* what changed
* what failed
* what cost was created
* what needs approval
* what should happen next

Stackfax treats run receipts as part of agent trust.

⸻

## Core Principle

Do not let an agent simply declare success.

An agent can propose an outcome.

The system should verify the outcome against recorded state.

Stackfax verdict:

Agent output is a claim. A run receipt is evidence.

⸻

## Why Logs Are Not Enough

Logs often answer:

What technically happened?

But operators need to know:

Did the useful job actually get done?

A raw log may show tool calls, timestamps, prompts, files, and errors.

A run receipt should turn that into a readable operational summary.

Example:

The agent attempted to draft three customer follow-up emails.

It found two complete customer records, skipped one incomplete record, drafted two emails, did not send anything, and needs human approval before sending.

That is more useful than a pile of raw events.

⸻

What A Run Receipt Should Include

A useful run receipt should include:

* task name
* task owner
* agent name or role
* model/provider used
* prompt or config version
* start time
* end time
* inputs used
* files read
* files changed
* tools called
* external systems touched
* approvals requested
* approvals granted
* retries
* failures
* cost estimate
* final status
* evidence for final status
* recommended next action

The receipt should be readable by a non-technical operator.

⸻

Final Status Options

Avoid vague status labels.

Bad:

* done
* complete
* successful
* handled
* fixed

Better:

* completed with evidence
* completed pending approval
* partially completed
* blocked
* failed safely
* failed with side effects
* skipped due to missing input
* escalated to human review

Stackfax verdict:

Status should describe operational reality, not agent confidence.

⸻

Approval State

A run receipt should clearly say whether an action:

* required no approval
* requested approval
* received approval
* was denied
* timed out
* was skipped because approval was missing

This matters most for:

* sending emails
* modifying files
* changing production systems
* spending money
* contacting customers
* deleting records
* publishing content
* executing code
* changing permissions

Stackfax verdict:

Approval gates only matter if the receipt shows whether they were used.

⸻

Tool Touch List

Every run receipt should identify what the agent touched.

Examples:

* browser
* files
* terminal
* email
* calendar
* CRM
* database
* payment system
* source control
* deployment system
* cloud console
* customer records

For each tool, the receipt should answer:

* Was it read-only or write-capable?
* What was accessed?
* What was changed?
* Was approval required?
* Did the tool call succeed?

Stackfax verdict:

Tool access without tool accounting creates invisible risk.

⸻

Cost Visibility

A run receipt should expose cost.

This does not need to be perfect at first.

At minimum, it should show:

* model used
* approximate tokens
* number of tool calls
* number of retries
* whether a premium model was used
* whether escalation happened
* whether the task could be routed cheaper next time

Stackfax verdict:

If you cannot see where the tokens went, you cannot improve the stack.

⸻

Failure Visibility

Failure should be legible.

A failed run receipt should explain:

* what failed
* where it failed
* whether anything changed before failure
* whether retry is safe
* whether human review is needed
* what input is missing
* what tool or permission blocked progress

Stackfax verdict:

A safe failure is one the operator can understand.

⸻

## Evidence Before Conclusion

The receipt should show evidence before final verdict.

Bad:

Task complete.

## Better:

Completed with evidence: created draft_followups.csv, generated two draft emails, skipped one record missing a customer email address, and did not send messages.

## Best:

Completed pending approval: two customer follow-up drafts are ready for review.

No external messages were sent.

One record was skipped due to missing contact data.

Next action: approve, edit, or reject the drafts.

Stackfax verdict:

The agent should not be the only witness to its own success.

⸻

Async Agent Work

Run receipts become more important when agents run asynchronously.

If the agent works while the human is away, the human needs to return to a clear summary:

* what happened
* what changed
* what needs review
* what is safe to ignore
* what requires action

Without a run receipt, asynchronous agents become invisible work that must be audited later.

Stackfax verdict:

Async agents need an operations layer, not just a chat interface.

⸻

Multi-Agent Work

In multi-agent systems, run receipts should show coordination.

Useful fields include:

* which agent started the work
* which agent received the task
* which agent changed files
* which agent reviewed the output
* which agent approved or rejected the next step
* whether agents passed state or dumped history
* whether any agent acted outside its role

Stackfax verdict:

A multi-agent team without receipts is just a room full of workers wearing headphones.

⸻

Run Receipts And Memory

Run receipts matter for agent memory.

A system should not save failed runs, bad assumptions, or unverified outputs as durable memory without review.

A memory-aware receipt should answer:

* Was anything saved to memory?
* What was saved?
* Why was it saved?
* Was the saved memory verified?
* Can the user inspect it?
* Can the user edit or delete it?
* Should this memory be injected into future runs?

Stackfax verdict:

Failed tool loops should enter quarantine, not memory.

⸻

Run Receipts And Approval Gates

Run receipts prove whether approval gates actually happened.

A stack can claim to have human-in-the-loop safety, but the receipt should show:

* what required approval
* who approved it
* what exact version was approved
* whether anything changed after approval
* whether action happened before or after approval
* what was skipped because approval was missing

Stackfax verdict:

Human approval is only real if the system can show what was approved.

⸻

## Run Receipt Template

Task:
Owner:
Agent:
Model/provider:
Config/prompt version:

Start:
End:
Status:

Inputs used:
Tools touched:
Files read:
Files changed:
External systems touched:

Approvals:
Retries:
Failures:
Cost estimate:

Evidence:
Next action:

## Expanded Run Receipt Template

Use this for higher-risk or business workflows.

Task:
Owner:
Agent:
Agent role:
Model/provider:
Model route:
Config/prompt version:
Workflow version:

Start:
End:
Status:

Requested outcome:
Actual outcome:
Evidence for outcome:

Inputs used:
Files read:
Files changed:
Tools called:
External systems touched:
Data accessed:
Credentials used:
Customer records touched:

Approval required:
Approval requested:
Approval granted/denied:
Approved version:
Action taken after approval:

Retries:
Fallbacks:
Failures:
Side effects:
Rollback needed:

Token estimate:
Cost estimate:
Premium model used:
Could this be routed cheaper next time?

Memory saved:
Memory injected:
Memory needs review:

Next action:
Human review needed:
Recheck trigger:

⸻

Stackfax Scoring Questions

A Stackfax report should ask:

* Can the system explain what the agent did?
* Can a non-technical owner read the result?
* Are tool calls visible?
* Are file changes visible?
* Are approvals visible?
* Are failures visible?
* Is cost visible?
* Is the next action clear?
* Can the run be repeated or inspected later?
* Can the system prove the useful work was completed?
* Can bad runs be excluded from memory?
* Can the user see what changed after approval?

⸻

What Would Improve The Score

A stack can improve its Run Receipts score by adding:

* plain-language receipt summary
* task status taxonomy
* model/provider trace
* config/prompt version
* tool touch list
* file change list
* external system list
* approval record
* failure summary
* retry summary
* cost estimate
* evidence section
* next action
* memory save/injection record
* operator-readable output

⸻

Possible Verdicts

Possible Run Receipt verdicts include:

* Run Receipts Required
* Cost Visibility Missing
* Tool Touch List Missing
* Approval Evidence Missing
* Failed Safely
* Completed Pending Approval
* Logs Exist / Receipts Missing
* Operator-Readable Receipts Needed
* Agent Output Is Unverified
* Receipt Layer Strong

⸻

Final Rule

Do not ask only:

Did the agent finish?

Ask:

What evidence proves the useful work was completed, what changed, what did it cost, and what needs review next?

The best agent systems do not just act.

They leave receipts.
