# Stackfax Model Routing Doctrine

Model Routing Doctrine is the Stackfax doctrine for deciding which model, provider, local model, tool, script, or human review layer should handle each part of an Ai workflow.

The goal is to stop users from sending every task to the strongest, most expensive, or most hyped model by default.

---

## Core Idea

The best stack does not use the best model for everything.

The best stack sends each job to the right layer.

## Core rule:

Route by job, not hype.

---

## Core Question

Is this stack using the right model, tool, code path, or human review layer for each step of the workflow?

If not, the stack may be wasting tokens, increasing risk, or making the workflow harder to trust.

---

## Why This Matters

Ai stacks often start with one model doing everything.

That is simple.

It is also usually inefficient.

One model may be asked to:

* gather data
* clean data
* summarize
* classify
* write
* reason
* review
* call tools
* make decisions
* draft customer-facing messages
* approve actions
* explain results

That creates risk because not every step needs the same intelligence, cost, latency, context window, privacy level, or review standard.

Stackfax verdict:

Spend intelligence where it matters.

⸻

Model Routing Definition

Model routing means deciding which layer handles which job.

A route may send work to:

* deterministic code
* spreadsheet formulas
* search filters
* database queries
* small local model
* cheap cloud model
* mid-tier model
* strong reasoning model
* specialized coding model
* retrieval system
* human reviewer
* approval gate

The model is one layer.

The route is the operating decision.

⸻

Bad Routing Pattern

A weak stack may:

* use the strongest model for every task
* use one model for every workflow
* use premium models for extraction
* send raw logs directly to the model
* ask the model to do math from pasted data
* let fallback chains silently escalate
* use local models for tasks they cannot handle
* use weak models for high-risk customer-facing decisions
* skip human approval on important actions

Stackfax verdict:

Do not spend premium-model money on routine tasks.

⸻

Better Routing Pattern

A stronger stack separates work into layers.

Recommended pattern:

1. Code or tools gather and filter.
2. Retrieval pulls relevant context.
3. Cheap model drafts or summarizes.
4. Mid-tier model organizes or reviews.
5. Strong model handles hard reasoning.
6. Human approves high-consequence actions.
7. Run receipt records what happened.

The expensive model should not carry the entire workflow.

⸻

Model Jobs

Each model or provider should have a job.

Common model jobs include:

* primary daily driver
* drafting model
* summary model
* classification model
* extraction helper
* research helper
* coding helper
* strong reasoning model
* final review model
* local/privacy model
* cheap automation model
* customer-facing writing model
* evaluator model

If a model has no job, it may be stack clutter.

⸻

Code Before Model

Some tasks should use code before Ai.

Good candidates for code:

* counting
* filtering
* sorting
* deduping
* extracting structured fields
* calculating totals
* checking dates
* validating schemas
* reading CSV files
* matching IDs
* applying fixed business rules
* checking required fields

Stackfax rule:

Use code for extraction. Use Ai for judgment.

Do not pay a model to reason through a mess that code could organize first.

⸻

Retrieval Before Reasoning

The model should not search the entire haystack when the system can provide a smaller evidence bundle.

Better pattern:

* search
* filter
* retrieve
* label sources
* assemble evidence
* then ask the model to reason

Stackfax verdict:

Retrieval should reduce reasoning load, not increase it.

⸻

Cheap Model Layer

Cheap models fit routine work.

Good uses:

* first drafts
* summaries
* classification
* tagging
* cleanup
* formatting
* basic extraction
* simple rewrites
* routine checklists
* low-risk internal notes

Cheap models should not make high-consequence decisions without review.

⸻

Local Model Layer

Local models can fit when the workflow benefits from:

* privacy
* isolation
* offline use
* repeated low-risk work
* local experimentation
* lower API usage
* local drafts
* summaries
* tagging
* retrieval cleanup

Local models are not automatically better.

They may be weaker, slower, harder to maintain, or less reliable for complex reasoning.

Stackfax verdict:

Local models reduce cost only when they fit a repeated workload.

⸻

Strong Model Layer

Strong models should be reserved for work that earns the cost.

Good uses:

* hard reasoning
* final review
* complex synthesis
* ambiguous decisions
* difficult debugging
* strategy
* adversarial review
* customer-facing quality checks
* business-critical analysis
* cases where cheaper layers failed

Stackfax rule:

Cloud escalation should happen when the task earns it.

⸻

Human Review Layer

Human review is part of routing.

Some work should route to a human before action.

Human approval should be required before Ai can:

* send messages
* contact customers
* post publicly
* edit customer records
* change inventory
* process payments
* issue refunds
* move or delete files
* access credentials
* modify production systems
* touch wallets or financial accounts

Stackfax principle:

Human approval is a routing decision.

⸻

Routing And Approval Gates

Model routing should include approval gates.

Examples:

* cheap model drafts customer email
* strong model reviews tone and risk
* human approves before send

or:

* code calculates sales totals
* model explains trend
* human approves business decision

or:

* local model summarizes private notes
* strong model receives anonymized evidence bundle
* human reviews before action

The route should show where authority changes.

⸻

Routing And Cost

Routing is cost control.

A token-smart route should define:

* which tasks use cheap models
* which tasks use strong models
* when escalation happens
* when fallback stops
* what budget applies
* what tool-call cap applies
* what context cap applies
* how cost is logged

Without routing, premium models become default workers.

⸻

Routing And Context

Context should be routed too.

Do not pass the same context to every model.

Examples:

* cheap model receives short draft context
* strong model receives evidence bundle
* local model receives private notes
* code receives raw CSV
* human receives summary plus receipt

Stackfax rule:

Pass state, not history.

⸻

Routing And Privacy

Privacy affects routing.

A stack may route private data to:

* local model
* internal tool
* human reviewer
* anonymized summary
* restricted workflow

A stack should avoid routing sensitive data to broad cloud prompts unless the workflow truly requires it and the user approves.

Customer data is not generic context.

⸻

Routing And Fallbacks

Fallback chains need visibility.

Weak fallback:

* cheap model fails
* system silently escalates to premium model
* user sees only final answer
* bill increases
* no receipt exists

Better fallback:

* cheap model fails
* system records failure
* asks whether to escalate
* logs model used
* records cost
* includes fallback in run receipt

Stackfax verdict:

Fallback is not enough. Routing needs policy, priority, logging, and visibility.

⸻

Routing And Version Drift

Model routes age quickly.

A route may need recheck when:

* new model launches
* pricing changes
* limits change
* local model improves
* provider behavior changes
* tool-calling reliability changes
* context window changes
* router defaults change
* fallback behavior changes

Stackfax rule:

A stack verdict should age honestly.

⸻

Routing And Agent ROI

Good routing should improve Agent ROI.

It should reduce:

* cost
* latency
* supervision burden
* cleanup
* risk
* retry loops

It should improve:

* completion
* reliability
* review quality
* repeatability
* useful output
* evidence quality

Agent ROI is not activity.

It is verified useful work after cost, supervision, risk, and cleanup.

⸻

Model Routing Verdicts

Possible verdicts include:

* Model Routing Needed
* Premium Model Overuse
* Cheap Draft Layer Needed
* Strong Review Layer Needed
* Code Before Ai
* Local Model Fit
* Local Model Not Required Yet
* Cloud Escalation Needed
* Fallback Visibility Missing
* Human Review Required
* Route By Job
* Safe To Continue With Routing Rules

⸻

Common Risk Flags

Model routing reviews may include:

* Token Burn Risk
* Premium Model Overuse
* Context Bloat Risk
* Silent Escalation Risk
* Subscription Overlap Risk
* Cost Visibility Missing
* Approval Gates Missing
* Customer Data Risk
* Local Model Quality Gap
* Production Not Ready
* Agent ROI Unclear

⸻

What Would Improve The Score

A stack can improve model routing by adding:

* model job assignments
* cheap draft layer
* strong review layer
* code extraction layer
* retrieval before reasoning
* fallback policy
* escalation approval
* budget caps
* model caps
* context caps
* route logs
* run receipts
* 30-day model review

The goal is not using fewer models.

The goal is using the right layer for the right job.

⸻

## Example Routing Map

Gather data:
Code, search, API, or retrieval

Clean/filter data:
Code or deterministic tool

Draft:
Cheap model or local model

Summarize:
Cheap or mid-tier model

Reason:
Strong model

Review:
Strong model or human

Approve:
Human

Act:
Tool only after approval

Record:
Run receipt

⸻

### Example Report Language

Use language like:

This stack needs model routing.

The strongest model appears to be handling too much routine work, including summaries, drafting, cleanup, and broad context review.

Before scaling, separate the workflow into gather, filter, summarize, reason, review, and approve steps. Use code or tools for extraction, cheaper models for routine work, and strong models only for judgment or final review.

Short version:

Route by job, not hype.

⸻

## Stackfax Principle

Route by job, not hype.

Spend intelligence where it matters.

Use code for extraction. Use Ai for judgment.

⸻

## Final Rule

Do not ask only which model is best.

Ask which layer should handle each part of the workflow, what it costs, what it can touch, what requires approval, and what receipt proves the route worked.
