# Run Receipts

A production agent needs a run receipt, not just logs.

Logs are useful for engineers.  
Run receipts are useful for owners, operators, reviewers, and future agents.

A run receipt explains what happened in plain language:

- what was attempted
- what inputs were used
- what model/config ran
- what tools were touched
- what changed
- what failed
- what cost was created
- what needs approval
- what should happen next

Stackfax treats run receipts as part of agent trust.

---

## Core principle

Do not let an agent simply declare success.

An agent can propose an outcome.

The system should verify the outcome against recorded state.

Stackfax verdict:

> Agent output is a claim. A run receipt is evidence.

---

## Why logs are not enough

Logs often answer:

> What technically happened?

But operators need to know:

> Did the useful job actually get done?

A raw log may show tool calls, timestamps, prompts, files, and errors.

A run receipt should turn that into a readable operational summary.

Example:

> The agent attempted to draft three customer follow-up emails. It found two complete customer records, skipped one incomplete record, drafted two emails, did not send anything, and needs human approval before sending.

That is more useful than a pile of raw events.

---

## What a run receipt should include

A useful run receipt should include:

- task name
- task owner
- agent name or role
- model/provider used
- prompt or config version
- start time
- end time
- inputs used
- files read
- files changed
- tools called
- external systems touched
- approvals requested
- approvals granted
- retries
- failures
- cost estimate
- final status
- evidence for final status
- recommended next action

---

## Final status options

Avoid vague status labels.

Bad:

- done
- complete
- successful
- handled
- fixed

Better:

- completed with evidence
- completed pending approval
- partially completed
- blocked
- failed safely
- failed with side effects
- skipped due to missing input
- escalated to human review

Stackfax verdict:

> Status should describe operational reality, not agent confidence.

---

## Approval state

A run receipt should clearly say whether an action:

- required no approval
- requested approval
- received approval
- was denied
- timed out
- was skipped because approval was missing

This matters most for:

- sending emails
- modifying files
- changing production systems
- spending money
- contacting customers
- deleting records
- publishing content
- executing code
- changing permissions

Stackfax verdict:

> Approval gates only matter if the receipt shows whether they were used.

---

## Tool touch list

Every run receipt should identify what the agent touched.

Examples:

- browser
- files
- terminal
- email
- calendar
- CRM
- database
- payment system
- source control
- deployment system
- cloud console
- customer records

For each tool, the receipt should answer:

- Was it read-only or write-capable?
- What was accessed?
- What was changed?
- Was approval required?
- Did the tool call succeed?

Stackfax verdict:

> Tool access without tool accounting creates invisible risk.

---

## Cost visibility

A run receipt should expose cost.

This does not need to be perfect at first.

At minimum, it should show:

- model used
- approximate tokens
- number of tool calls
- number of retries
- whether a premium model was used
- whether escalation happened
- whether the task could be routed cheaper next time

Stackfax verdict:

> If you cannot see where the tokens went, you cannot improve the stack.

---

## Failure visibility

Failure should be legible.

A failed run receipt should explain:

- what failed
- where it failed
- whether anything changed before failure
- whether retry is safe
- whether human review is needed
- what input is missing
- what tool or permission blocked progress

Stackfax verdict:

> A safe failure is one the operator can understand.

---

## Evidence before conclusion

The receipt should show evidence before final verdict.

Bad:

> Task complete.

Better:

> Completed with evidence: created `draft_followups.csv`, generated two draft emails, skipped one record missing a customer email address, and did not send messages.

Best:

> Completed pending approval: two customer follow-up drafts are ready for review. No external messages were sent. One record was skipped due to missing contact data. Next action: approve, edit, or reject the drafts.

Stackfax verdict:

> The agent should not be the only witness to its own success.

---

## Async agent work

Run receipts become more important when agents run asynchronously.

If the agent works while the human is away, the human needs to return to a clear summary:

- what happened
- what changed
- what needs review
- what is safe to ignore
- what requires action

Without a run receipt, asynchronous agents become invisible work that must be audited later.

Stackfax verdict:

> Async agents need an operations layer, not just a chat interface.

---

## Multi-agent work

In multi-agent systems, run receipts should show coordination.

Useful fields include:

- which agent started the work
- which agent received the task
- which agent changed files
- which agent reviewed the output
- which agent approved or rejected the next step
- whether agents passed state or dumped history
- whether any agent acted outside its role

Stackfax verdict:

> A multi-agent team without receipts is just a room full of workers wearing headphones.

---

## Run receipt template

```text
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
Stackfax scoring questions

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

⸻

Final rule

Do not ask only:

Did the agent finish?

Ask:

What evidence proves the useful work was completed, what changed, what did it cost, and what needs review next?

The best agent systems do not just act.

They leave receipts.
