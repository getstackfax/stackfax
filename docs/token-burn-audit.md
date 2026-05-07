Token Burn Audit

The Token Burn Audit is a Stackfax report type for users who are spending too much on premium-model tokens, API calls, agent runs, or overlapping Ai subscriptions.

The goal is to find where the stack is wasting tokens, using expensive models for simple work, loading too much context, silently escalating to higher-cost models, or letting agents loop without cost controls.

⸻

Core Question

Is this stack using the right model, context, tool, and workflow for the task, or is it burning tokens because the workflow is poorly structured?

Short version:

The leak is not token use. The leak is misrouted intelligence.

⸻

Who This Is For

The Token Burn Audit is for:

* users surprised by high API bills
* OpenClaw users who burned too many tokens on one task
* builders using premium models for routine work
* businesses running Ai automations without cost controls
* users with overlapping model subscriptions
* users using large context windows without understanding the cost
* users relying on fallback chains that may silently escalate
* users whose agents repeatedly search, browse, retry, or reread files
* users who do not know which model handled which step

⸻

What The Audit Reviews

A Token Burn Audit reviews:

* premium model overuse
* model routing
* model subscription overlap
* API/token costs
* context bloat
* memory loading
* knowledge file loading
* fallback escalation
* repeated tool loops
* workflow design
* deterministic tasks that should use code instead of Ai
* retrieval quality
* budget caps
* model caps
* tool-call caps
* logging and visibility
* run receipts

⸻

Common Token Burn Patterns

Premium Model Overuse

This happens when the strongest or most expensive model handles too much routine work.

Warning signs:

* premium model drafts everything
* premium model summarizes simple text
* premium model does basic classification
* premium model performs extraction work that code could handle
* no cheaper draft/review layers exist
* no model routing rules exist

Stackfax recommendation:

Use cheaper models for routine work and reserve strong models for judgment, reasoning, difficult debugging, and final review.

⸻

Context Bloat

This happens when the stack loads too much information into tasks that do not need it.

Warning signs:

* large context loaded by default
* knowledge files loaded into every call
* long histories always included
* irrelevant files attached to simple tasks
* memory is always on
* sensitive data is loaded unnecessarily
* unchanged background context is resent repeatedly

Stackfax recommendation:

Load only the context needed for the task.

Use state, not full history.

⸻

Silent Escalation

This happens when a fallback chain moves from cheaper models to expensive models without the user clearly noticing.

Warning signs:

* fallback chain includes premium models
* no session budget cap
* no model cap
* no escalation alert
* no log showing which model handled which step
* no cost receipt
* user only notices after the bill arrives

Stackfax recommendation:

Add model caps, session budget caps, escalation visibility, and cost receipts.

Escalation should be visible, bounded, and earned.

⸻

Tool Loop Burn

This happens when an agent repeatedly calls tools, searches, browsers, files, APIs, or commands without clear stopping rules.

Warning signs:

* repeated web searches
* repeated browser actions
* repeated file reads
* repeated failed commands
* long tool loops
* no max step count
* no clear stop condition
* no failure path
* broad task prompt with unclear output

Stackfax recommendation:

Set tool-call limits, task boundaries, retry limits, stop conditions, and approval checkpoints.

Retry rules are cost controls.

⸻

Ai Doing Code Work

This happens when Ai is used for deterministic work that code, filters, spreadsheets, schemas, or simple scripts could handle better.

Warning signs:

* Ai extracts simple structured fields
* Ai filters data that code could filter
* Ai repeatedly searches instead of using a structured source
* Ai compares raw data before it is cleaned
* Ai handles tasks that could be preprocessed cheaply
* Ai reasons over messy data before tools organize it

Stackfax principle:

Use code for extraction. Use Ai for judgment.

⸻

Bad Retrieval

This happens when retrieval adds more confusion and cost instead of reducing context.

Warning signs:

* too many chunks retrieved
* irrelevant context retrieved
* same sources retrieved repeatedly
* important source missed
* conflicting context passed without labels
* facts, guesses, notes, and logs mixed together

Stackfax recommendation:

Retrieval should reduce reasoning load, not increase it.

The model should receive a useful evidence bundle, not a junk drawer.

⸻

Model Routing Pattern

A token-smart stack should separate work into layers.

Recommended pattern:

* code or tools gather and filter
* retrieval pulls relevant context only
* cheap model drafts
* cheap or mid-tier model summarizes
* strong model reasons or reviews
* human approves important actions
* run receipt records cost, tools, outcome, and failure state

The expensive model should not be doing every step.

⸻

Budget Controls

A strong stack should include budget controls.

Recommended controls:

* session budget cap
* daily budget cap
* model cap
* context cap
* tool-call cap
* retry cap
* escalation alert
* fallback rules
* logging by model
* logging by workflow
* cost review after testing
* approval before expensive runs

Without cost controls, an agent stack can look productive while silently burning money.

⸻

Subscription Fit

Token burn is not only API cost.

Users can also waste money by paying for overlapping subscriptions.

Stackfax checks whether the user really needs multiple paid tools such as:

* ChatGPT
* Claude
* Gemini
* OpenRouter
* local models
* API credits
* business Ai tools
* agent platforms
* automation platforms

The question is not which tool is best.

The question is which paid access actually fits the workflow.

Every paid tool should have a job.

⸻

Run Receipts

A Token Burn Audit should look for run receipts or cost visibility.

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

Example Token Burn Verdict

Verdict:

Model Routing Needed

Risk flags:

* Premium Model Overuse
* Context Bloat Risk
* Silent Escalation Risk
* Tool Loop Burn
* Budget Cap Missing
* Cost Visibility Missing

Best next move:

Split the workflow into gather, filter, summarize, reason, and review steps.

Use code or tools for extraction, cheaper models for routine work, and strong models only for judgment or final review.

⸻

What Would Improve The Score

A stack can improve its Token Burn Audit score by adding:

* clear task boundaries
* cheaper draft layer
* strong model only for review or judgment
* session budget cap
* daily budget cap
* model cap
* context cap
* tool-call cap
* retry cap
* smaller task-specific context
* fallback visibility
* cost logging
* run receipts
* 30-day recheck

The goal is not cheapness.

The goal is useful work per dollar.

⸻

Common Badges

Token Burn Audits may use badges such as:

* Token-Smart
* Token Burn Risk
* Context Bloat Risk
* Silent Escalation Risk
* Model Routing Needed
* Budget Cap Required
* Cost Visibility Missing
* Subscription Overlap Risk
* Tool Loop Burn
* Human Approval Required
* Recheck Needed

⸻

Possible Verdicts

Possible Token Burn Audit verdicts include:

* Token-Smart
* Low Token Burn Risk
* Model Routing Needed
* Premium Model Overuse
* Context Bloat Risk
* Silent Escalation Risk
* Tool Loop Burn
* Budget Caps Missing
* Cost Visibility Missing
* Subscription Overlap Risk
* Local Model May Help
* Recheck After Routing

⸻

Final Rule

Do not spend premium-model money on intern tasks.

Stackfax helps users find where tokens are draining before the bill teaches the lesson.
