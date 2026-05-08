# Stackfax Evaluation Layer

The Evaluation Layer is the Stackfax doctrine for checking whether an Ai stack, model, agent, or workflow actually performs well enough for the job.

The goal is not to chase benchmark scores.

The goal is to test whether the stack produces useful, safe, repeatable, reviewable work in the real workflow.

⸻

Core Idea

Benchmarks rank models.

Workflow tests reveal fit.

A model can win the chart and still lose the job.

A stack should not be judged only by model leaderboard position, demo quality, or how impressive the output sounds.

It should be judged by whether the workflow works.

⸻

Core Question

Can this stack produce the right output, safely, repeatedly, at an acceptable cost, with enough evidence to review?

If the answer is unclear, the stack needs an evaluation layer.

⸻

What The Evaluation Layer Checks

The Evaluation Layer checks:

* output quality
* task completion
* repeatability
* cost
* review burden
* failure behavior
* approval gates
* run receipts
* source quality
* tool behavior
* model routing
* human trust
* workflow fit
* safe escalation

The question is not:

Which model is best?

The better question is:

Which setup works for this job?

⸻

Why Benchmarks Are Not Enough

Benchmarks can be useful.

They can show model strength, reasoning ability, coding skill, math ability, long-context ability, or general capability.

But business and agent workflows fail in messier ways.

Real workflows include:

* unclear inputs
* partial information
* bad data
* missing files
* tool errors
* browser issues
* stale memory
* customer data
* approval needs
* wrong-channel risk
* budget limits
* operator review time

A benchmark does not prove the stack can handle those.

Stackfax verdict:

Clean benchmarks miss the mess that breaks real agents.

⸻

Workflow Test

A good evaluation starts with one real workflow.

Ask:

* What task should the stack complete?
* What input starts the task?
* What output counts as done?
* Who reviews it?
* What tools are allowed?
* What should require approval?
* What should never happen?
* What evidence proves completion?
* What cost is acceptable?
* What failure mode is safe?

The workflow test should be small enough to repeat.

⸻

Good Evaluation Questions

Stackfax should ask:

* Did the stack complete the task?
* Was the output usable?
* Was the output accurate enough?
* Was the reasoning inspectable?
* Were sources or evidence included?
* Did the model use the right context?
* Did the agent stay inside permissions?
* Did the workflow require too much supervision?
* Did the result justify the cost?
* Did the system leave a run receipt?
* Could the same workflow run again?

⸻

Output Quality

Output quality should be judged against the job.

A useful output should be:

* relevant
* accurate enough for the use case
* structured
* reviewable
* actionable
* source-aware when needed
* safe to use after the expected level of review

Bad output may be:

* polished but wrong
* long but not useful
* confident without evidence
* generic
* unsupported
* hard to review
* missing the next action

Stackfax rule:

Pretty output is not the same as usable output.

⸻

Repeatability

One good run is not enough.

A stack has stronger evaluation when it can repeat the workflow across multiple runs.

Check:

* Does it work twice?
* Does it work with slightly different inputs?
* Does it fail in understandable ways?
* Does it keep the same output format?
* Does cost stay controlled?
* Does quality stay acceptable?
* Does the receipt make review easier?

Stackfax verdict:

One lucky run is not a system.

⸻

Failure Evaluation

A serious evaluation should test failure.

Ask:

* What happens when input is missing?
* What happens when a source is unclear?
* What happens when a tool fails?
* What happens when the model is uncertain?
* What happens when approval is missing?
* What happens when the cost cap is reached?
* What happens when the agent cannot finish?

Good failure behavior:

* stops safely
* explains what failed
* avoids risky action
* asks for missing input
* escalates to human review
* leaves a receipt
* does not loop forever

Stackfax verdict:

Recovery is not noise. Recovery is proof the system can survive reality.

⸻

Cost Evaluation

A stack can pass quality tests and still fail cost tests.

Check:

* Which model handled each step?
* Was a premium model used unnecessarily?
* Was too much context loaded?
* Were tools called repeatedly?
* Did retries burn tokens?
* Was fallback escalation visible?
* Was cost tied to useful output?

Stackfax rule:

The leak is not token use. The leak is misrouted intelligence.

⸻

Human Review Burden

Evaluation should include review cost.

Ask:

* How long did review take?
* What had to be corrected?
* Were sources easy to inspect?
* Was the output structured for review?
* Did the reviewer trust the receipt?
* Did the agent reduce work or move work into cleanup?

If human review takes longer than doing the task manually, the stack may not be ready.

Stackfax verdict:

Saved time does not count until cleanup is counted.

⸻

Approval Gate Evaluation

A stack should be tested against its approval rules.

Check whether the system correctly asks for approval before:

* sending messages
* posting publicly
* contacting customers
* changing records
* moving or deleting files
* connecting credentials
* processing payments
* changing inventory
* modifying production systems

Approval gates only matter if the system can show whether they were used.

Stackfax rule:

Human approval is only real if the receipt shows what was approved.

⸻

Run Receipt Evaluation

The evaluation layer should inspect the receipt.

A useful receipt should show:

* what task was requested
* what model was used
* what tools were touched
* what files or systems were accessed
* what changed
* what failed
* what it cost
* what approval was requested or granted
* what needs review next

Without receipts, evaluation becomes guesswork.

Stackfax rule:

Agent output is a claim. A run receipt is evidence.

⸻

Multi-Model Evaluation

Multi-model comparison can be useful, but it is not automatic verification.

Two models agreeing does not prove correctness.

Three models disagreeing does not mean the average answer is best.

Model disagreement should trigger review.

Useful comparison questions:

* Which model produced the most usable output?
* Which model required less cleanup?
* Which model cited better evidence?
* Which model followed instructions better?
* Which model stayed inside the workflow?
* Which model cost less for acceptable quality?
* Which model failed safely?

Stackfax principle:

Multi-model consensus is not verification. It is a risk spotlight.

⸻

Evaluation Layer Verdicts

Possible verdicts include:

* Evaluation Layer Missing
* Workflow Test Needed
* Output Quality Unclear
* Repeatability Not Proven
* Review Burden Too High
* Cost Test Failed
* Failure Mode Missing
* Run Receipts Required
* Approval Gate Test Needed
* Safe To Test
* Ready For Next Workflow
* Agent ROI Unclear
* Agent ROI Verified

⸻

Common Risk Flags

Evaluation reviews may include:

* Evaluation Layer Missing
* Agent ROI Unclear
* Run Receipts Missing
* Cost Visibility Missing
* Approval Gates Missing
* Token Burn Risk
* Context Bloat Risk
* Model Routing Needed
* Fragile UI Automation Risk
* Production Not Ready
* Workflow Fit Unclear

⸻

What Would Improve The Score

A stack can improve its evaluation score by adding:

* one defined workflow test
* expected output format
* success criteria
* failure criteria
* source/evidence requirements
* cost cap
* review checklist
* approval gate test
* run receipt
* repeat test
* 30-day recheck
* examples of good and bad outputs

The goal is not to build a perfect eval system first.

The goal is to make the next workflow test more honest.

⸻

Example Evaluation Test

Workflow:
Draft a customer follow-up email from approved notes.

Input:
One customer note, one product/service description, one desired next step.

Expected output:
One draft email, no sending, uncertainty flags, approval request.

Pass criteria:
Correct customer context, no invented claims, clear next action, human approval required before send.

Fail criteria:
Wrong customer, unsupported promise, message sent without approval, missing uncertainty flag, no receipt.

Receipt required:
Model used, input used, draft created, no message sent, approval pending.

Example Report Language

Use language like:
This stack has Evaluation Layer Missing because the model choice appears based on general capability rather than a repeatable workflow test.

Before scaling, define one workflow test, expected output, pass/fail criteria, cost cap, approval point, and run receipt.

Short version:

Benchmarks rank models. Workflow tests reveal fit.

⸻

Stackfax Principle

Benchmarks rank models.

Workflow tests reveal fit.

A model can win the chart and still lose the job.

⸻

Final Rule

Do not ask only whether the model is good.

Ask whether the workflow produced useful, safe, repeatable, reviewable work at an acceptable cost.
