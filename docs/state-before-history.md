# Stackfax State Before History

State Before History is the Stackfax doctrine for passing only the information needed for the next decision instead of dumping full transcripts, logs, memories, notes, or histories into every agent run.

The goal is to reduce context bloat, token burn, stale assumptions, privacy risk, and decision confusion.

⸻

Core Idea

Agents do not need the whole story every time.

They need the current state.

Core rule:

Pass state, not history.

History explains how the system got here.

State tells the system what matters now.

⸻

Core Question

Does this stack pass the current task state clearly, or does it force the model to reread the full history and figure it out?

If the stack passes too much history, it may be wasting tokens and increasing risk.

⸻

Why This Matters

Long histories feel safe because nothing gets lost.

But full history can create problems:

* token burn
* context bloat
* stale assumptions
* private data exposure
* irrelevant details
* conflicting instructions
* slower runs
* weaker retrieval
* harder review
* old mistakes reappearing
* failed outputs becoming durable truth

A bigger prompt is not always a better prompt.

Stackfax verdict:

Bigger context is not the same as better state.

⸻

History

History is the full record of what happened.

Examples:

* full chat transcript
* full tool log
* full meeting notes
* entire project archive
* all prior drafts
* old decisions
* failed attempts
* full repo context
* every memory note
* previous screenshots
* raw research dumps

History is useful for audit, review, and recovery.

But it should not always be passed directly into the next run.

⸻

State

State is the current information needed to make the next decision.

Examples:

* current goal
* current task
* known constraints
* approved decisions
* active files
* current blockers
* unresolved questions
* forbidden actions
* approval status
* relevant source notes
* next action
* current risk flags
* latest checked date

State is compact, current, and decision-ready.

A good state packet helps the agent act without rereading the entire story.

⸻

Bad Pattern

A weak stack may:

* paste the whole transcript
* load all memory
* include every note
* attach entire documents
* pass all logs
* keep every turn active
* use long context as the default solution
* trust the model to sort the mess

Stackfax verdict:

Do not make the model read the haystack. Build the system that hands it the needle bundle.

⸻

Better Pattern

A stronger stack should:

* summarize the current goal
* identify the next decision
* pass relevant constraints
* include only needed evidence
* label source material
* separate facts from guesses
* mark stale assumptions
* preserve approval state
* leave full history in storage
* retrieve history only when needed

The model should receive the working state, not the whole attic.

⸻

State Packet

A state packet is a compact handoff for the next run or agent.

A useful state packet may include:

Current goal:
Current task:
Relevant facts:
Current constraints:
Approved decisions:
Open questions:
Files/sources needed:
Tools allowed:
Forbidden actions:
Approval status:
Risk flags:
Next action:
Receipt needed:

A state packet should be short enough to inspect and specific enough to act on.

⸻

Agent Handoffs

Multi-agent systems especially need state discipline.

Bad handoff:

Here is the whole transcript. Figure it out.

Better handoff:

Here is the current state, the task, the constraints, the allowed tools, and what output is needed.

Stackfax principle:

Agents do not become a team until responsibility moves through a durable handoff.

A handoff should transfer responsibility, not confusion.

⸻

Memory Handoffs

Memory should pass relevant state, not all remembered history.

Risky memory handoff:

* global memory injected into every run
* client notes mixed across workflows
* old assumptions reused
* private data included unnecessarily
* failed outputs treated as facts

Safer memory handoff:

* scoped retrieval
* current state summary
* source labels
* stale labels
* sensitivity labels
* approval notes
* memory receipt

Core rule:

Agent memory is not agent permission.

⸻

Context Compression

Context compression is useful, but compression is not the same as state design.

A summary of everything may still be too broad.

Ask:

* What does the next agent need to decide?
* What can be archived?
* What is stale?
* What is unresolved?
* What requires approval?
* What should be excluded?
* What evidence is needed?

Stackfax verdict:

Compacting history is not the same as designing state.

⸻

State And Token Burn

Passing history can burn tokens without improving output.

Warning signs:

* every run includes long prior context
* agents reread unchanged files
* logs are pasted repeatedly
* full memory is always active
* premium models are used to sort irrelevant context
* cost rises but quality does not improve

Stackfax rule:

The leak is not token use. The leak is misrouted intelligence.

State-first design helps the stack spend tokens where they matter.

⸻

State And Privacy

Passing full history can expose private information unnecessarily.

Risk increases when history contains:

* customer data
* client data
* emails
* private files
* credentials
* payment details
* financial records
* sensitive personal information
* old screenshots
* internal strategy

State packets should exclude private data unless the task truly needs it.

Customer data is not generic context.

⸻

State And Approval

Approval state should be explicit.

A good state packet should say whether the next action is:

* allowed
* blocked
* waiting for approval
* approved
* denied
* draft-only
* observe-only
* forbidden

Approval should not be buried in old chat history.

Stackfax rule:

Human approval is only real if the receipt shows what was approved.

⸻

State And Receipts

State packets and run receipts work together.

State packet before the run:

* what the agent needs to know
* what it is allowed to do
* what result is expected

Run receipt after the run:

* what happened
* what changed
* what failed
* what approval was used
* what state should carry forward

A strong stack updates state after each meaningful run.

⸻

Evidence Before State

State should be grounded in evidence.

Avoid state summaries that hide uncertainty.

Weak state:

Customer is ready to buy.

Better state:

Customer asked for pricing and availability. No purchase approval yet. Next action: draft follow-up for review.

Weak state:

Task complete.

Better state:

Draft created. No message sent. Approval pending.

Stackfax verdict:

Status should describe operational reality, not agent confidence.

⸻

State Drift

State Drift happens when the current state becomes outdated or wrong.

Warning signs:

* old decisions remain active
* stale tool versions are referenced
* old pricing assumptions remain
* old customer status is reused
* completed tasks remain open
* rejected drafts return later
* failed runs are summarized as success

State should be refreshed after important changes.

⸻

State Before History Verdicts

Possible verdicts include:

* Pass State, Not History
* Context Bloat Risk
* State Packet Needed
* Handoff Too Broad
* Memory Scope Risk
* Stale State Risk
* Approval State Missing
* Receipt Needed
* Safe To Continue With Scoped State

⸻

Common Risk Flags

State reviews may include:

* Context Bloat Risk
* Token Burn Risk
* Memory Scope Risk
* Stale Memory Risk
* Customer Data Risk
* Approval Gates Missing
* Run Receipts Required
* Agent ROI Unclear
* Evaluation Layer Missing
* Version Drift Risk

⸻

What Would Improve The Score

A stack can improve state discipline by adding:

* state packet template
* scoped memory retrieval
* current-task summary
* approval status
* risk flags
* source labels
* stale labels
* open question list
* forbidden action list
* next action
* receipt update after run
* archived history
* 30-day state review

The goal is not less information.

The goal is better information at the point of decision.

⸻

Example Report Language

Use language like:

This stack has Context Bloat Risk because it appears to pass full history into each run instead of a compact current-state packet.

Before scaling, separate archived history from active state. Pass the current goal, constraints, approval status, relevant sources, risk flags, and next action instead of loading everything by default.

Short version:

Pass state, not history.

⸻

Stackfax Principle

Pass state, not history.

Compacting history is not the same as designing state.

Bigger context is not the same as better state.

⸻

Final Rule

Do not make every agent reread the whole story.

Give it the current state, the allowed action, the evidence needed, and the next decision.
