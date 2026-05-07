Token Burn Risk

Token burn is not automatically bad.

Misrouted token burn is the leak.

Stackfax treats token cost as a workflow design issue, not just a pricing issue.

Two users can be on the same subscription page and have completely different burn rates.

One person asks for summaries and recipe ideas.

Another person spins up agent workflows, generates code all day, runs giant context windows, retries everything repeatedly, and treats the model like a full-time employee with no lunch break.

Same subscription page.

Completely different burn rate.

⸻

Core Question

Stackfax asks:

Is this stack spending intelligence where it actually matters?

A stack has Token Burn Risk when it uses expensive model capacity for work that could be handled by:

* a smaller model
* a local model
* retrieval
* caching
* structured data
* deterministic code
* search filters
* templates
* rules
* human approval
* better workflow design

The goal is not to spend zero tokens.

The goal is to route tokens correctly.

⸻

Why This Matters

Token burn can hide inside normal-looking usage.

A user may think the problem is:

* the model is too expensive
* the subscription is not enough
* the API is overpriced
* the context window is too small
* the hardware is not strong enough

But the real issue may be:

* every task uses the strongest model
* too much context is loaded
* retrieval is sloppy
* agents retry without limits
* tools fail silently
* workflows are too broad
* no one tracks cost per run
* no one knows which model did what

Stackfax treats token burn as a routing and workflow problem first.

⸻

Common Token Burn Leaks

1. Premium Model By Default

Using the strongest model for every task is simple, but often wasteful.

Common examples:

* summaries
* classification
* tagging
* formatting
* rewriting
* simple research
* basic extraction
* routine drafts
* checklist generation

Stackfax verdict:

Do not use a frontier model as the default worker for routine tasks.

⸻

2. Raw Context Dumping

Many stacks burn tokens because they dump everything into the prompt.

Common examples:

* full logs
* entire repos
* giant chat histories
* long documents
* raw exports
* repeated screenshots
* unfiltered browser pages
* unchanged background context

Stackfax verdict:

Do not make the model read the haystack. Build the system that hands it the needle bundle.

⸻

3. Bad Retrieval

Poor retrieval can be more expensive than no retrieval.

A stack has retrieval burn risk when it:

* retrieves too much
* retrieves irrelevant chunks
* misses the key source
* repeats the same retrieval
* gives the model conflicting context without labels
* fails to separate facts, notes, guesses, and logs

Stackfax verdict:

Retrieval should reduce reasoning load, not increase it.

⸻

4. Agent Retry Loops

Agents can burn tokens quickly when they fail silently and keep trying.

Common signs:

* repeated tool calls
* repeated file reads
* repeated failed commands
* repeated planning loops
* no clear stop condition
* no retry limit
* no human escalation
* no run receipt

Stackfax verdict:

Retry rules are cost controls.

⸻

5. Thinking When Routing Would Work

Some tasks do not need more reasoning.

They need better routing.

Examples:

* Which document matters?
* Which logs are relevant?
* Which customer record should be updated?
* Which model should handle this?
* Does this action need approval?

These should often be handled by routing, filters, schemas, or rules before a premium model is called.

Stackfax verdict:

Do not pay a model to reason through a mess the system could have organized first.

⸻

6. Long History By Default

Some stacks pass too much past conversation into every new task.

This can create:

* higher cost
* slower responses
* stale assumptions
* irrelevant context
* worse reasoning
* accidental leakage across tasks

A better pattern is:

Pass state, not history.

The next step usually needs the current state, constraints, decision, and relevant evidence.

It does not need the whole story every time.

Stackfax verdict:

Long memory is not the same as useful state.

⸻

7. Silent Escalation

Some stacks quietly escalate to stronger models when cheaper models fail.

This can be useful if controlled.

It becomes risky when:

* the user does not know escalation happened
* no budget cap exists
* fallback chains are too aggressive
* the same task retries across multiple premium models
* there is no cost receipt
* there is no quality improvement from the escalation

Stackfax verdict:

Escalation should be visible, bounded, and earned.

⸻

Better Routing Pattern

A healthier stack uses layers.

Example:

1. Cheap/simple layer receives the task.
2. Workflow identifies the task type.
3. Retrieval pulls only relevant context.
4. Small/local model handles routine work.
5. Premium model handles hard reasoning only when needed.
6. Human reviews risky outputs.
7. Run receipt records cost, tools, outcome, and failure state.

This turns token usage into an intentional decision.

⸻

Log Intelligence Example

A user may think they need a bigger GPU or larger context window because they have many logs.

But the real problem may be workflow architecture.

For log intelligence, do not dump raw logs into a model.

First:

* normalize events
* filter by IP, user, device, source, and time window
* query each log source separately
* return only matching events and nearby context
* group by timestamp, source, and device
* flag likely causes
* show evidence before conclusion

Then the model reasons over a compact incident bundle.

Stackfax verdict:

Log intelligence needs retrieval quality before model size.

⸻

Local Model Use

Local models can reduce token burn, but only if the workflow is shaped correctly.

A small local model can be useful for:

* summaries
* tagging
* classification
* draft cleanup
* retrieval cleanup
* simple extraction
* log/event explanation
* routine code review
* structured transformations

But local is not free if it creates:

* setup time
* maintenance burden
* slower iteration
* worse reliability
* hidden debugging cost
* hardware overbuild
* weaker output quality

Stackfax verdict:

Local models reduce cost only when they fit a repeated workload.

⸻

Premium Model Use

Premium models are valuable.

The problem is using them without discrimination.

Premium models should be reserved for:

* ambiguous reasoning
* high-value decisions
* complex planning
* difficult debugging
* final synthesis
* adversarial review
* customer-facing quality checks
* sensitive business decisions
* cases where a cheaper layer failed

Stackfax verdict:

Cloud escalation should happen when the task earns it.

⸻

Cost Controls

A stack should define cost controls before agents run unattended.

Useful controls include:

* model routing rules
* max context limits
* retry limits
* tool-call limits
* per-task budgets
* daily budgets
* approval before expensive runs
* fallback models
* summarization checkpoints
* caching rules
* run receipts
* exception alerts

Without cost controls, an agent stack can look productive while silently burning money.

⸻

Run Receipts

Token burn should be visible.

A useful run receipt should show:

* selected model
* why that model was selected
* prompt/config version
* context size
* tools used
* retries
* fallback events
* cost estimate
* outcome status
* approval needed
* next action

Stackfax verdict:

If you cannot see where the tokens went, you cannot manage the stack.

⸻

Warning Signs

A stack has high Token Burn Risk when:

* every task uses the same premium model
* agents reread the same files repeatedly
* raw logs are pasted directly into prompts
* context grows every turn without compression
* retrieval returns too much
* tool failures trigger repeated retries
* there is no stop condition
* no one knows which model did what
* fallback behavior is invisible
* budget caps are missing
* cost is reviewed only after the bill arrives

⸻

What Would Improve The Score

A stack can reduce Token Burn Risk by adding:

* model routing rules
* cheaper draft layer
* premium review layer
* retrieval filters
* context limits
* caching
* deterministic preprocessing
* retry limits
* budget caps
* cost receipts
* workflow scoping
* human approval for expensive runs
* local models for repeated low-risk work
* monthly or 30-day cost recheck

The goal is not cheapness.

The goal is useful work per dollar.

⸻

Possible Verdicts

Possible Token Burn Risk verdicts include:

* Low Token Burn Risk
* Token Burn Risk
* High Token Burn Risk
* Model Routing Needed
* Context Bloat Risk
* Retrieval Burn Risk
* Tool Loop Burn
* Silent Escalation Risk
* Budget Caps Missing
* Cost Visibility Missing
* Local Model May Help
* Premium Model Overuse
* Recheck After Routing

⸻

Report Language

Use language like:

This stack is not necessarily spending too much.

The issue is that expensive model capacity may be used before routing, retrieval, filtering, caching, or smaller-model layers have done their job.

Short version:

The leak is not token use. The leak is misrouted intelligence.

Final Rule

Do not ask only:

How do I spend fewer tokens?

Ask:

Which work deserves expensive reasoning, and which work should be routed, retrieved, cached, local, scripted, or reviewed?

The best stack is not the one with the lowest token use.

The best stack spends tokens where they create verified useful work.
