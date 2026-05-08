# Stackfax Evidence Assembly

Evidence Assembly is the Stackfax doctrine for collecting the proof needed to judge whether an Ai stack, agent, workflow, report, or automation actually did useful work.

The goal is to prevent decisions from being based only on agent confidence, polished output, or vague claims of completion.

⸻

Core Idea

Ai output is not evidence by itself.

A useful stack should assemble the facts, sources, receipts, tool records, approvals, costs, and outcomes needed to support a verdict.

Core rule:

Evidence before conclusion.

⸻

Core Question

What evidence proves the work was completed, the output is usable, the risk is bounded, and the next decision is justified?

If the evidence is missing, the verdict is weaker.

⸻

Why This Matters

Ai systems can produce confident answers without showing enough proof.

Agents can say:

* done
* fixed
* sent
* reviewed
* safe
* optimized
* ready
* complete

But operators need to know:

* what was attempted
* what was used
* what changed
* what failed
* what was approved
* what it cost
* what still needs review
* what evidence supports the final status

Stackfax verdict:

Agent output is a claim. A run receipt is evidence.

⸻

What Counts As Evidence

Evidence may include:

* source documents
* tool call records
* files read
* files changed
* data inputs
* screenshots
* logs
* run receipts
* approval records
* model/config version
* prompt version
* cost estimate
* test results
* reviewer notes
* before/after comparison
* external system status
* error messages
* timestamps
* output artifacts

Evidence should be tied to the workflow.

Not every task needs the same proof.

⸻

Evidence Types

Source Evidence

Source evidence shows where the information came from.

Examples:

* document name
* public URL
* file path
* database record
* spreadsheet row
* customer note
* support ticket
* transcript
* repository file
* product page
* policy document

Stackfax checks:

* Is the source known?
* Is it current?
* Is it relevant?
* Is it private or public?
* Is it reliable enough for the decision?
* Was it actually used?

⸻

Action Evidence

Action evidence shows what the agent or workflow did.

Examples:

* tool calls
* browser actions
* file edits
* API calls
* form fills
* messages drafted
* messages sent
* records updated
* commands run
* automations triggered

Stackfax checks:

* What action happened?
* Was it read-only or write-capable?
* Was approval required?
* Was approval granted?
* Did anything change?
* Can the action be reviewed?

⸻

Output Evidence

Output evidence shows what was produced.

Examples:

* draft email
* report
* summary
* code diff
* spreadsheet
* checklist
* analysis
* status update
* classification result
* recommendation
* run receipt

Stackfax checks:

* Is the output usable?
* Is it structured?
* Is it reviewable?
* Does it match the requested job?
* Does it include uncertainty when needed?
* Does it cite or reference evidence?

⸻

Approval Evidence

Approval evidence shows whether a human approved a risky action.

Examples:

* approved draft
* approval timestamp
* reviewer note
* explicit approval state
* denied action
* pending approval
* skipped due to missing approval

Stackfax checks:

* Was approval required?
* Was approval requested?
* Was approval granted?
* What exactly was approved?
* Did action happen before or after approval?

Core rule:

Human approval is only real if the receipt shows what was approved.

⸻

Cost Evidence

Cost evidence shows what the work consumed.

Examples:

* model used
* token estimate
* API calls
* tool calls
* retries
* fallback escalation
* subscription/tool used
* hardware/runtime cost
* human review time
* cleanup time

Stackfax checks:

* What did the task cost?
* Was a premium model needed?
* Were retries controlled?
* Did cost create useful output?
* Could the task be routed cheaper next time?

Stackfax verdict:

The leak is not token use. The leak is misrouted intelligence.

⸻

Failure Evidence

Failure evidence shows what did not work.

Examples:

* missing input
* tool error
* failed command
* timeout
* login problem
* wrong source
* approval missing
* cost cap reached
* failed retrieval
* uncertain result
* partial completion

Stackfax checks:

* What failed?
* Did anything change before failure?
* Is retry safe?
* Is human review needed?
* What input is missing?
* Was failure contained?

A safe failure is one the operator can understand.

⸻

Before / After Evidence

Before/after evidence shows whether the workflow improved.

Examples:

* time before vs after
* cost before vs after
* error rate before vs after
* response delay before vs after
* review burden before vs after
* output quality before vs after
* missed follow-ups before vs after
* cleanup burden before vs after

Stackfax checks:

* Did the stack improve the workflow?
* Did it only move work somewhere else?
* Did it reduce burden after cleanup is counted?
* Did it improve the next run?

Core rule:

Agent ROI is not activity. It is verified useful work.

⸻

Evidence Assembly Pattern

A good evidence assembly pattern:

1. Define the claim.
2. Identify what proof is needed.
3. Gather only relevant sources.
4. Label sources clearly.
5. Separate facts from guesses.
6. Record actions taken.
7. Record approvals.
8. Record failures.
9. Record cost.
10. Produce a reviewable conclusion.

The model should not be asked to decide from a pile.

The system should hand it an evidence bundle.

⸻

Claim Before Evidence

Every verdict should know what claim it is making.

Examples:

Claim:

Hardware is not justified yet.

Evidence needed:

* workflow unclear
* no local model requirement
* cloud tools sufficient
* no always-on need
* no privacy isolation requirement

Claim:

Token burn risk is high.

Evidence needed:

* premium model overuse
* large context by default
* repeated tool loops
* no budget caps
* no cost receipts

Claim:

Safe to test with approval.

Evidence needed:

* low-risk workflow
* scoped tools
* human review
* no production access
* receipt exists

A verdict without evidence is just a guess.

⸻

Evidence Bundle

An evidence bundle is the compact set of proof needed for a decision.

Example evidence bundle:

Claim:
Sources used:
Facts:
Assumptions:
Unknowns:
Actions observed:
Approvals:
Failures:
Cost signals:
Risk flags:
Conclusion:
Next evidence needed:

Evidence bundles help with reports, audits, run receipts, and evaluation.

⸻

Evidence And Receipts

Run receipts are a major evidence layer.

A receipt should answer:

* what was attempted
* what input was used
* what model/config ran
* what tools were touched
* what changed
* what failed
* what approval was used
* what cost was created
* what needs review next

Evidence assembly helps receipts avoid vague status labels.

Bad:

Complete.

Better:

Completed pending approval: draft created, no message sent, missing phone number flagged, approval needed before sending.

⸻

Evidence And Evaluation

Evaluation requires evidence.

The evaluation layer should ask:

* What output was expected?
* What output was produced?
* What sources were used?
* What pass/fail criteria applied?
* What failed?
* What did review find?
* What cost was incurred?
* Could the workflow repeat?

Without evidence, evaluation becomes vibes.

Stackfax principle:

Benchmarks rank models. Workflow tests reveal fit.

⸻

Evidence And Business Audits

Business audits need evidence that operators can understand.

Business evidence may include:

* workflow map
* source of truth
* approval policy
* customer-data boundary
* credential boundary
* output examples
* failure examples
* cost records
* review notes
* run receipts
* 30-day action plan

Executives do not need raw logs first.

They need an evidence-backed verdict.

⸻

Evidence And Privacy

Evidence should not expose unnecessary private data.

A good evidence bundle should include enough proof to support the decision without dumping sensitive information.

Avoid including:

* passwords
* API keys
* payment details
* wallet information
* private customer data
* private legal documents
* sensitive personal data
* unnecessary screenshots
* private messages unrelated to the task

Evidence should be scoped.

Customer data is not generic context.

⸻

Evidence Assembly Verdicts

Possible verdicts include:

* Evidence Assembly Needed
* Evidence Before Conclusion
* Run Receipts Required
* Source Evidence Missing
* Approval Evidence Missing
* Cost Evidence Missing
* Failure Evidence Missing
* Output Not Proven
* Agent ROI Unclear
* Safe To Continue With Evidence

⸻

Common Risk Flags

Evidence assembly reviews may include:

* Run Receipts Required
* Evaluation Layer Missing
* Agent ROI Unclear
* Cost Visibility Missing
* Approval Gates Missing
* Workflow Fit Unclear
* Customer Data Risk
* Token Burn Risk
* Production Not Ready
* Version Drift Risk

⸻

What Would Improve The Score

A stack can improve evidence assembly by adding:

* evidence bundle template
* source labels
* claim/evidence mapping
* run receipts
* approval records
* cost records
* failure records
* before/after comparison
* review notes
* pass/fail criteria
* next-evidence-needed field
* privacy-safe evidence handling

The goal is not more paperwork.

The goal is better decisions.

⸻

Example Report Language

Use language like:

This stack needs better evidence assembly.

The agent can produce outputs, but the sources used, approvals, costs, failures, and proof of completion are not yet visible enough to support confident scaling.

Before expanding automation, add run receipts and evidence bundles that show what was used, what changed, what failed, and what needs review.

Short version:

Evidence before conclusion.

⸻

Stackfax Principle

Evidence before conclusion.

Agent output is a claim.

A run receipt is evidence.

⸻

Final Rule

Do not let the agent be the only witness to its own success.

Assemble the evidence before trusting the verdict.
