# Stackfax Workflow Before Agent

Workflow Before Agent is the Stackfax doctrine for defining the job before adding agents, tools, memory, automations, local hardware, or model routing.

The goal is to prevent users from building powerful agent stacks around unclear work.

⸻

Core Idea

Do not start with the agent.

Start with the workflow.

An agent is only useful when the work it supports is clear enough to inspect, repeat, improve, and safely review.

Core rule:

Workflow first. Agent second.

⸻

Core Question

What job is this agent supposed to make simpler, cheaper, safer, faster, more reliable, or easier to review?

If the job is unclear, the agent stack is probably premature.

⸻

Why This Matters

Agents feel like leverage.

They can also hide workflow confusion.

A user may add:

* more models
* more tools
* more memory
* more prompts
* more agents
* more routing
* more dashboards
* more automations
* more hardware

But if the workflow is unclear, more stack usually creates more confusion.

Stackfax verdict:

Ai does not fix chaos. It scales chaos.

⸻

What A Workflow Includes

A workflow should define:

* trigger
* owner
* input
* source of truth
* task steps
* tools involved
* output
* definition of done
* approval point
* failure path
* receipt or log
* next action

If these are missing, the agent does not have a job.

It has a vague mission.

⸻

Workflow Questions

Before adding an agent, ask:

* What starts the work?
* Who owns the work?
* What input is required?
* Where does the input come from?
* What output should be produced?
* Who reviews the output?
* What should require approval?
* What should never happen?
* What can fail?
* What happens when it fails?
* What evidence proves the job was done?
* What should improve after 30 days?

These questions matter more than tool choice.

⸻

Bad Starting Point

A weak starting point sounds like:

* I want an agent for my business.
* I want to automate everything.
* I want OpenClaw set up.
* I want a local Ai box.
* I want a multi-agent system.
* I want Ai to handle customers.
* I want Ai to manage operations.
* I want a dashboard.

These may become useful later.

But first, define the workflow.

⸻

Better Starting Point

A better starting point sounds like:

* I want to summarize incoming customer inquiries every morning.
* I want to draft follow-up emails, but not send them.
* I want to flag missing intake information.
* I want to compare sales reports and explain changes.
* I want to prepare weekly content drafts for review.
* I want to classify support tickets and route them to a human.
* I want to create run receipts for each agent task.

These are workflows.

They can be tested.

⸻

The First Workflow Test

A safe first workflow should be small.

Recommended pattern:

1. Pick one repeated task.
2. Define the input.
3. Define the output.
4. Use low-risk or public data.
5. Let Ai summarize or draft.
6. Require human review.
7. Leave a receipt.
8. Repeat before expanding access.

The first goal is not autonomy.

The first goal is proving the workflow.

⸻

Workflow Fit

A workflow has stronger fit when:

* the task repeats
* the input is available
* the output is clear
* review is possible
* mistakes are containable
* value is visible
* approval points are obvious
* cost can be tracked
* the result can be compared to manual work

A workflow has weak fit when:

* the task is vague
* the input is messy
* ownership is unclear
* output is subjective
* mistakes are expensive
* no one reviews the result
* no approval gates exist
* no receipt exists
* the user cannot say what improved

⸻

Agent Fit

An agent may be useful when the workflow requires:

* repeated reasoning
* multi-step drafting
* structured review
* source gathering
* tool coordination
* status reporting
* missing-information detection
* safe preparation for human approval
* receipt generation

An agent may be premature when the workflow mostly needs:

* process cleanup
* better handoff
* clearer ownership
* simple checklist
* spreadsheet cleanup
* deterministic script
* better data source
* human decision
* stable business rule

Stackfax principle:

Do not use an agent where a checklist, rule, script, or cleaner handoff would solve the problem.

⸻

Tools After Workflow

Tools should be added after the workflow is defined.

Ask:

* What tool does the workflow need?
* Is the tool read-only or write-capable?
* What can the tool touch?
* What approval is required?
* What happens if the tool fails?
* Does the tool leave evidence?

A tool without a workflow is just another risk surface.

⸻

Memory After Workflow

Memory should support the workflow, not replace workflow clarity.

Ask:

* What should the agent remember?
* What should stay temporary?
* What should be retrieved only when needed?
* What should never enter memory?
* What memory scope applies?
* What stale memory could mislead the run?

Stackfax rule:

Pass state, not history.

⸻

Model Routing After Workflow

Model routing should follow the job.

Ask:

* Which step needs cheap drafting?
* Which step needs summarization?
* Which step needs strong reasoning?
* Which step needs final review?
* Which step should use code instead of Ai?
* Which step needs human approval?

The model route should match the workflow.

Not the hype cycle.

⸻

Hardware After Workflow

Hardware should be considered after the workload is clear.

Ask:

* What workload would hardware unlock?
* Does the task require local models?
* Does privacy isolation matter?
* Does always-on local runtime matter?
* Does an existing machine work?
* Would cloud-first prove the workflow faster?
* Would hardware solve the actual bottleneck?

Stackfax rule:

Do not buy the machine before you can name the job.

⸻

Approval Gates

Workflow design should identify approval gates before automation expands.

Human approval should be required before Ai can:

* send messages
* contact customers
* post publicly
* edit customer records
* move or delete files
* connect credentials
* process payments
* issue refunds
* change inventory
* modify production systems
* trigger external actions

Approval should be built into the workflow, not added after something goes wrong.

⸻

Run Receipts

Every serious workflow should leave a receipt.

A useful workflow receipt should show:

* what task was requested
* what input was used
* what model or tool ran
* what output was produced
* what changed
* what failed
* what approval was requested
* what needs review next

Stackfax rule:

Agent output is a claim. A run receipt is evidence.

⸻

Business Workflow Pattern

For business workflows, the safest path is:

1. Map the current manual process.
2. Identify where delay, cost, or errors happen.
3. Pick one low-risk repeated task.
4. Add Ai for summary, draft, or review support.
5. Require human approval before action.
6. Track the result.
7. Improve the workflow before expanding automation.

Business automation should start with trust, not speed.

⸻

Common Workflow-First Verdicts

Possible verdicts include:

* Workflow Not Defined
* Workflow Fit Unclear
* Process Before Automation
* Start With One Safe Workflow
* Draft With Approval
* Observe Only
* Human Approval Required
* Run Receipts Required
* Safe To Test
* Agent Not Needed Yet
* Agent Ready For First Workflow
* Stack Ready For Next Test

⸻

Common Risk Flags

Workflow Before Agent reviews may include:

* Workflow Fit Unclear
* Agentic Trap Risk
* Process Before Automation
* Approval Gates Missing
* Run Receipts Required
* Agent ROI Unclear
* Evaluation Layer Missing
* Token Burn Risk
* Context Bloat Risk
* Hardware Overbuild Risk
* Production Not Ready
* Credential Isolation Risk

⸻

What Would Improve The Score

A workflow can improve by adding:

* clear trigger
* clear owner
* defined input
* source of truth
* expected output
* definition of done
* approval gates
* forbidden actions
* failure path
* run receipt
* review checklist
* cost boundary
* repeat test
* 30-day recheck

The goal is not to make the stack bigger.

The goal is to make the work clearer.

⸻

Example Report Language

Use language like:

This stack is not ready for more agents yet.

The workflow needs to be defined first: what starts the task, what input is used, what output counts as done, what requires approval, and what receipt proves the work happened.

Start with one low-risk workflow, run it manually or draft-only, then add agent permissions after the result is proven.

Short version:

Workflow first. Agent second.
⸻

Stackfax Principle

Workflow first.

Agent second.

Do not automate chaos.

Do not add agent power before the job is clear.

⸻

Final Rule

Before asking what agent to use, ask what workflow needs to improve.

The right agent stack starts with a clear job, a safe first test, and evidence that the workflow actually got better.
