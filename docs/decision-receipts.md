# Stackfax Decision Receipts

Decision Receipts are the Stackfax doctrine for explaining why a stack verdict, model route, approval requirement, hardware recommendation, risk flag, or automation decision was made.

The goal is to make Ai-stack decisions inspectable instead of mysterious.

⸻

Core Idea

A decision should not only say what to do.

It should explain why that decision fits the evidence.

Core rule:

A verdict should leave a receipt.

⸻

Core Question

Can the stack explain why this recommendation, verdict, risk flag, approval gate, or next action was chosen?

If not, the user may not know whether to trust it, challenge it, or improve it.

⸻

Why This Matters

Stackfax gives verdicts.

Examples:

* Cloud-First
* Hardware Justified
* Overkill Warning
* Model Routing Needed
* Token Burn Risk
* Approval Gates Missing
* Production Not Ready
* Safe To Test
* Recheck Needed
* Draft With Approval
* Process Before Automation

Those verdicts are only useful if the user can see what caused them.

A decision receipt turns a verdict into an explainable recommendation.

⸻

Decision Receipt Definition

A decision receipt is a short explanation of:

* what decision was made
* what evidence supported it
* what assumptions were used
* what risks mattered
* what alternatives were considered
* what would change the verdict
* what the next action should be

The goal is not to write a legal brief.

The goal is to make the recommendation reviewable.

⸻

## Basic Decision Receipt Template

Decision:
Verdict:
Evidence used:
Main reasons:
Assumptions:
Risks considered:
Alternatives considered:
What would change this decision:
Next action:
Recheck trigger:

## ⸻

Decision Types

Stackfax may need decision receipts for:

* hardware verdicts
* model routing choices
* subscription fit decisions
* automation level decisions
* approval gate decisions
* production readiness decisions
* risk flag assignments
* badge assignments
* recheck recommendations
* migration recommendations
* business automation safety decisions
* agent permission decisions

Any decision that affects cost, safety, trust, or action should be explainable.

⸻

Hardware Decision Receipts

A hardware decision receipt should explain why the user should buy, wait, stay cloud-first, or consider local later.

### Example decision:

Verdict: Cloud-First

Possible evidence:

* no proven local workload
* no privacy isolation requirement
* no always-on local need
* workflow is mostly research and drafts
* current cloud tools are enough
* hardware would not solve the main bottleneck

What would change the verdict:

* repeated local workload appears
* token cost becomes material
* privacy isolation becomes necessary
* always-on local workflow is proven
* user needs dedicated Ai lab separation

Stackfax rule:

Hardware should match the job, not the hype.

⸻

Model Routing Decision Receipts

A model routing decision receipt should explain why a task should go to a cheap model, strong model, local model, cloud model, code, or human review.

### Example decision:

Verdict: Model Routing Needed


Possible evidence:

* premium model used for routine work
* classification/summarization does not need strongest model
* no budget cap
* no fallback visibility
* strong reasoning only needed for final review
* code could handle extraction first

What would change the verdict:

* model jobs are assigned
* cheap draft layer exists
* strong model only reviews
* cost visibility exists
* fallback escalation is logged

Stackfax rule:

Spend intelligence where it matters.

⸻

## Subscription Decision Receipts

A subscription decision receipt should explain what to keep, pause, cancel, test, or route differently.

### Example decision:

Verdict: Simplify Subscriptions

## Possible evidence:

* multiple premium tools with overlapping jobs
* no usage log
* no assigned model roles
* API and chat subscriptions overlap
* local models are being tested without a proven local workflow

## What would change the verdict:

* each paid tool gets a job
* 30-day usage log proves value
* API budget cap exists
* routine tasks are routed cheaper
* business plan need is proven

## Stackfax rule:

Every paid tool should have a job.

⸻

## Approval Gate Decision Receipts

An approval gate decision receipt should explain why a human must approve an action.

### Example decision:

Verdict: Human Approval Required

Possible evidence:

* customer-facing message
* public posting
* money/payment involved
* credentials involved
* production system involved
* customer record could change
* business reputation risk
* irreversible action risk

What would change the verdict:

* action becomes read-only
* action becomes draft-only
* permissions are scoped
* output is reviewed
* approval is recorded
* rollback exists

Stackfax rule:

Human approval is only real if the receipt shows what was approved.

⸻

Automation Level Decision Receipts

A decision receipt should explain why the workflow belongs at a specific automation level.

Possible levels:

* Observe Only
* Draft With Approval
* Limited Approved Actions
* Production Automation

Example decision:

Verdict: Draft With Approval

Possible evidence:

* workflow involves customers
* tone and context matter
* source data may be incomplete
* mistakes could damage trust
* approval path is easy
* full automation is not needed yet

What would change the verdict:

* workflow repeats reliably
* review burden drops
* approval history is clean
* receipts exist
* failure handling is tested

Stackfax rule:

Drafting is not execution.

⸻

Production Readiness Decision Receipts

A production readiness decision receipt should explain why a workflow is or is not ready for real operations.

Example decision:

Verdict: Production Not Ready

Possible evidence:

* no run receipts
* no rollback plan
* no approval gates
* no failure owner
* no cost visibility
* no monitoring
* broad credentials
* customer data involved
* workflow only worked once

What would change the verdict:

* repeat test passes
* run receipts exist
* approval gates work
* errors fail safely
* rollback is tested
* cost and tool use are visible

Stackfax rule:

One lucky run is not a system.

⸻

Risk Flag Decision Receipts

Risk flags should not be random labels.

A decision receipt should explain why the flag was assigned.

Example:

Risk flag: Context Bloat Risk

Evidence:

* full history included
* unrelated notes loaded
* long documents attached
* no context receipt
* premium model used to sort context

What would remove the flag:

* state packet used
* context receipt exists
* retrieval scoped
* irrelevant files excluded
* stale context labeled

Stackfax rule:

Context used should be context accounted for.

⸻

Badge Decision Receipts

Badges should also be explainable.

Example:

Badge: StackChecked

Evidence:

* use case reviewed
* score assigned
* verdict assigned
* risk flags listed
* checked date recorded
* recheck window defined

Badge limitation:

StackChecked does not mean certified, perfect, safe forever, compliant, profitable, or future-proof.

Stackfax rule:

This stack was checked for this job, at this time, with these limits.

⸻

Migration Decision Receipts

A migration decision receipt should explain whether a stack should switch, test, wait, or stay put.

Example decision:

Verdict: Test Before Switching

Possible evidence:

* new model/tool update exists
* current stack still works
* migration could break workflows
* rollback path unclear
* cost/quality improvement not proven
* production workflow involved

What would change the verdict:

* sandbox test passes
* cost improves
* output improves
* workflow survives migration
* rollback exists
* recheck confirms fit

## Stackfax rule:

Migration is not progress unless the workflow gets better.

⸻

## Decision Receipts And Context Receipts

A decision receipt explains why the verdict happened.

A context receipt explains what information fed the verdict.

## Together they answer:

What did the system know?
Why did it recommend this?
What would change the answer?

Without context receipts, decision receipts may be weak.

Without decision receipts, context may not turn into an explainable verdict.

⸻

## Decision Receipts And Evidence Assembly

### Decision receipts should be grounded in evidence.

Weak decision:

You should stay cloud-first.

Better decision:

Verdict: Cloud-First.

Reason: The workflow is mostly research, drafts, and reports; no local model requirement was named; no always-on local runtime is needed; and hardware would not solve the current bottleneck.

What would change this: repeated private local workloads, material token cost, or a proven always-on agent workflow.

Stackfax rule:

Evidence before conclusion.

⸻

Decision Receipts And User Trust

Decision receipts help users trust the report without blindly obeying it.

A good receipt lets the user say:

* that makes sense
* that assumption is wrong
* this evidence is missing
* I can improve the score
* I know what to test next
* I know when to recheck

The best decision receipts make the next move obvious.

⸻

Decision Receipts And Rechecks

Decision receipts should include recheck triggers.

Examples:

* new model launches
* pricing changes
* usage limits change
* workflow changes
* agent gets new tools
* customer data is added
* hardware is added
* OpenClaw updates
* local model improves
* business workflow moves to production

Stackfax rule:

A stack verdict should age honestly.

⸻

Decision Receipt Verdicts

Possible verdicts include:

* Decision Receipt Needed
* Verdict Needs Evidence
* Risk Flag Needs Explanation
* Badge Needs Limits
* Recheck Trigger Needed
* Decision Explainability Good
* Safe To Continue With Decision Receipt

⸻

Common Risk Flags

Decision receipt reviews may include:

* Evidence Assembly Needed
* Context Receipt Needed
* Run Receipts Required
* Approval Gates Missing
* Cost Visibility Missing
* Evaluation Layer Missing
* Version Drift Risk
* Production Not Ready
* Agent ROI Unclear

⸻

What Would Improve The Score

A stack can improve decision quality by adding:

* decision receipt template
* evidence mapping
* context receipt
* alternatives considered
* assumptions listed
* what-would-change field
* recheck trigger
* score improvement notes
* risk flag explanation
* badge limitation notes
* next action

The goal is not to make every decision long.

The goal is to make important decisions inspectable.

⸻

## Example Report Language

### Use language like:

This report needs stronger decision receipts.

The verdict may be reasonable, but the user should be able to see why the system recommended Cloud-First, why Human Approval Required was assigned, and what evidence would change those decisions.

Add short decision receipts for major verdicts, risk flags, and next actions.

Short version:

A verdict should leave a receipt.

⸻

## Stackfax Principle

A verdict should leave a receipt.

Evidence before conclusion.

This stack was checked for this job, at this time, with these limits.

⸻

## Final Rule

Do not give users unexplained verdicts.

For every important Stackfax decision, show the evidence, assumptions, risks, alternatives, what would change the answer, and the next action.
