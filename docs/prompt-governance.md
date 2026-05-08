# Stackfax Prompt Governance

Prompt Governance is the Stackfax doctrine for treating prompts, system instructions, templates, agent roles, routing instructions, and workflow prompts as operational infrastructure.

The goal is to prevent prompt logic from becoming invisible, unversioned, unreviewed, or unsafe.

⸻

Core Idea

A serious Ai stack treats prompts like code.

Prompts can define:

* agent role
* task scope
* tool behavior
* approval rules
* output format
* risk boundaries
* model routing
* customer-facing tone
* business policy
* memory use
* escalation behavior

That means prompts are not just text.

They are part of the operating layer.

Core rule:

A serious Ai stack treats prompts like code: versioned, parameterized, logged, and reviewable.

⸻

Core Question

Can this stack explain which prompt or instruction produced the output, what version it used, what it allowed, and what changed since the last run?

If not, prompt governance is missing.

⸻

Why This Matters

Prompt logic can quietly control important behavior.

A prompt may decide:

* what the agent should do
* what the agent should not do
* which tools it may use
* what tone it should use
* whether it asks for approval
* whether it summarizes or acts
* whether it escalates uncertainty
* whether it saves memory
* whether it contacts a user
* whether it handles private data

If that prompt is invisible, unversioned, or casually edited, the stack becomes hard to trust.

Stackfax verdict:

Prompt logic without metadata becomes invisible infrastructure.

⸻

Prompt Types

Stackfax may review several kinds of prompts.

System Prompts

High-level behavior instructions.

They may define:

* identity
* role
* rules
* boundaries
* forbidden actions
* tool use
* approval requirements

System prompts should be carefully reviewed.

They often act like policy.

⸻

Workflow Prompts

Prompts that run a specific task or process.

Examples:

* summarize customer inquiry
* draft follow-up email
* classify support ticket
* prepare sales report
* review code change
* analyze token burn
* generate Stackfax report

Workflow prompts should have:

* defined inputs
* defined outputs
* success criteria
* failure behavior
* review point
* version notes

⸻

Agent Role Prompts

Prompts that define a specialized agent.

Examples:

* researcher
* reviewer
* drafter
* coder
* evaluator
* scout
* support assistant
* business analyst

Agent role prompts should say:

* what the agent does
* what it cannot do
* what tools it can use
* what needs approval
* what output it should return
* when to stop

Role prompts should not quietly grant authority.

⸻

Template Prompts

Reusable prompt structures with variables.

Examples:

* report template
* customer reply template
* risk review template
* intake summary template
* run receipt template
* evaluation checklist

Template prompts should be parameterized instead of rewritten from scratch every time.

A template is stronger when the variable parts are explicit.

⸻

One-Off Prompts

Ad hoc prompts used for a single task.

One-off prompts are fine for exploration.

They become risky when they are reused repeatedly without being promoted into a reviewed template.

Stackfax check:

Is this still a one-off, or has it become production behavior?

⸻

Prompt Metadata

Useful prompt metadata may include:

* prompt name
* prompt version
* owner
* purpose
* workflow
* model target
* tools allowed
* inputs required
* output format
* approval rules
* memory rules
* risk level
* last updated date
* changelog
* test examples

Metadata makes prompt behavior inspectable.

Without metadata, the prompt becomes harder to audit.

⸻

Prompt Versioning

Prompt versions matter because small wording changes can change behavior.

Versioning helps answer:

* What changed?
* Why did it change?
* Who changed it?
* Which output used which version?
* Did the change improve results?
* Did the change create new risk?
* Should the old version be restored?

Prompt versioning is especially important for:

* customer-facing prompts
* business automation prompts
* agent role prompts
* report-generation prompts
* approval-gate prompts
* routing prompts
* prompts that touch private data

⸻

Prompt Change Receipts

Prompt changes should leave receipts.

A useful prompt change receipt should show:

* prompt name
* old version
* new version
* what changed
* why it changed
* who approved it
* test result
* risk impact
* rollback note

Stackfax principle:

If prompt behavior changed, the receipt should say what changed and why.

⸻

Prompt Drift

Prompt Drift happens when prompts slowly change until the workflow behaves differently than intended.

Warning signs:

* prompt edits are made casually
* no version history exists
* output format changes unexpectedly
* approval language disappears
* customer-facing tone changes
* risk disclaimers become weaker
* tool permissions become broader
* memory instructions become vague
* old examples override current rules

Prompt Drift is a form of Version Drift Risk.

A stack should recheck prompts when the workflow changes.

⸻

Prompt Ownership

Important prompts should have an owner.

An owner answers:

* What is this prompt for?
* Who can change it?
* What workflow does it affect?
* What output should it produce?
* What risks does it control?
* When should it be reviewed?

Business prompts especially need ownership.

If no one owns the prompt, no one owns the behavior.

⸻

Prompt And Tool Permissions

Prompts should not be the only permission layer.

A prompt can say:

Do not send emails without approval.

But the tool layer should also enforce that boundary where possible.

Stackfax checks whether prompt rules are backed by:

* tool permissions
* read-only mode
* scoped credentials
* approval gates
* sandbox environments
* logs
* run receipts

Core rule:

A prompt is not a cage.

Prompts guide behavior.

Permissions limit blast radius.

⸻

Prompt And Approval Gates

Prompts often define when the agent should ask for approval.

Approval should be explicit before:

* sending messages
* posting publicly
* contacting customers
* editing customer records
* changing files
* moving or deleting files
* connecting credentials
* processing payments
* changing inventory
* modifying production systems

Prompt governance checks:

* Does the prompt mention approval?
* Does the workflow enforce approval?
* Does the receipt show approval state?
* Does the prompt define forbidden actions?
* Does the prompt define escalation?

Approval in prompt text is not enough if the system cannot prove it happened.

⸻

Prompt And Memory

Prompts may decide what memory to use or save.

Risk increases when prompts tell agents to:

* remember everything
* load all notes
* summarize private data into memory
* save failed runs
* reuse old history
* infer durable facts from incomplete context
* share memory across projects

Safer prompts should define:

* what memory can be used
* what memory should not be used
* what can be saved
* what needs review before saving
* what should be excluded
* what scope applies

Core rule:

Prompt memory rules should not override memory governance.

⸻

Prompt And Customer-Facing Work

Customer-facing prompts need stronger review.

They may affect:

* brand tone
* promises made
* support quality
* refunds
* sales claims
* regulated statements
* customer trust
* public reputation

Customer-facing prompt checks:

* Is the allowed scope clear?
* Does it avoid unsupported promises?
* Does it require human approval before send?
* Does it escalate uncertainty?
* Does it protect customer data?
* Does it follow business policy?
* Is the output easy to review?

Stackfax verdict:

A customer-facing prompt is operational policy, not just writing help.

⸻

Prompt And Business Policy

Prompts can accidentally become policy.

Examples:

* refund handling
* customer escalation
* compliance notes
* sales promises
* legal disclaimers
* privacy statements
* support boundaries
* public posting tone

If a prompt contains business policy, it should be reviewed like business policy.

Do not hide policy inside a random prompt.

⸻

Prompt And Model Routing

Model routing prompts decide which model handles which task.

They should define:

* cheap model jobs
* strong model jobs
* escalation rules
* fallback rules
* cost caps
* review points
* uncertainty triggers
* when to stop

Weak routing prompts may cause:

* premium model overuse
* silent escalation
* weak model used for risky tasks
* expensive retries
* unclear cost

Stackfax rule:

Routing policy is part of the stack.

⸻

Prompt And Evaluation

Prompts should be tested against workflow outputs.

A prompt evaluation should ask:

* Did it produce the expected format?
* Did it follow approval rules?
* Did it use the right context?
* Did it avoid unsupported claims?
* Did it cite or reference evidence when needed?
* Did it stop safely when uncertain?
* Did it reduce review burden?
* Did it improve the next run?

Benchmarks do not prove prompt fit.

Workflow tests do.

⸻

Prompt Governance Verdicts

Possible verdicts include:

* Prompt Governance Needed
* Prompt Versioning Needed
* Prompt Drift Risk
* Prompt Ownership Missing
* Prompt Change Receipts Needed
* Approval Prompt Weak
* Customer-Facing Prompt Risk
* Prompt Hidden Policy Risk
* Prompt Template Needed
* Safe For Exploration
* Needs Workflow Test

⸻

Common Risk Flags

Prompt governance reviews may include:

* Prompt Governance Risk
* Version Drift Risk
* Approval Gates Missing
* Run Receipts Required
* Evaluation Layer Missing
* Customer Data Risk
* Communication Channel Risk
* Credential Isolation Risk
* Token Burn Risk
* Model Routing Needed
* Production Not Ready

⸻

What Would Improve The Score

A stack can improve prompt governance by adding:

* prompt names
* prompt versions
* owners
* changelog
* prompt metadata
* prompt change receipts
* workflow-specific templates
* approval rules
* memory rules
* test examples
* pass/fail criteria
* rollback notes
* customer-facing review
* 30-day prompt review

The goal is not bureaucracy.

The goal is to make prompt behavior visible and reviewable.

⸻

Example Prompt Metadata

Prompt name:
Version:
Owner:
Workflow:
Purpose:
Model target:
Tools allowed:
Inputs:
Output format:
Approval rules:
Memory rules:
Risk level:
Last updated:
Change note:
Test example:
Rollback note:

⸻

Example Report Language

Use language like:

This stack has Prompt Governance Risk because the prompts appear to control workflow behavior, tool use, and approval rules without versioning, ownership, or change receipts.

Before scaling, name the key prompts, assign owners, add versions, define approval and memory rules, and test the prompt against one repeatable workflow.

Short version:

Prompt logic without metadata becomes invisible infrastructure.

⸻

Stackfax Principle

A serious Ai stack treats prompts like code: versioned, parameterized, logged, and reviewable.

Prompt logic without metadata becomes invisible infrastructure.

Prompts can guide behavior, but they should not be the only safety layer.

⸻

Final Rule

Do not let prompts become invisible policy.

If a prompt controls behavior, permissions, customer-facing output, memory, routing, or approval, it should be named, versioned, reviewed, and testable.
