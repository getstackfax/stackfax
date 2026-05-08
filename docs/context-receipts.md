# Stackfax Context Receipts

Context Receipts are the Stackfax doctrine for showing what information was loaded, retrieved, passed, summarized, injected, or excluded during an Ai run.

The goal is to make context visible enough that a user, operator, reviewer, or future agent can understand why the output happened.

⸻

Core Idea

If context influenced the run, the receipt should show what context was used.

An Ai system should not silently load memory, files, history, RAG chunks, screenshots, notes, or tool outputs without leaving a record.

Core rule:

Context used should be context accounted for.

⸻

Core Question

Can the stack explain what context the agent saw before it produced the output?

If not, the output may be hard to trust, debug, repeat, or improve.

⸻

Why This Matters

Ai output depends heavily on context.

The model may be affected by:

* files
* memory
* chat history
* retrieval results
* screenshots
* browser pages
* logs
* prompts
* tool outputs
* prior summaries
* stale notes
* hidden system instructions
* project assumptions

If the user cannot see what context was used, they cannot know whether the answer came from the right information.

Stackfax verdict:

Hidden context creates hidden risk.

⸻

Context Receipt Definition

A context receipt is a short record of what information was available to the model, agent, workflow, or report generator during a run.

It should show:

* what was loaded
* what was retrieved
* what was summarized
* what was excluded
* what was stale
* what was private
* what was missing
* what influenced the output

A context receipt does not need to include every raw token.

It should explain the context boundary.

⸻

What A Context Receipt Should Include

A useful context receipt may include:

* task name
* run ID or date
* agent/workflow name
* model/provider used
* prompt/config version
* memory used
* files used
* sources retrieved
* search query used
* tools used for context gathering
* excluded sources
* stale sources
* private/sensitive context warning
* context size estimate
* assumptions carried forward
* open questions
* confidence or completeness note

⸻

Basic Context Receipt Template

Task:
Run date:
Agent/workflow:
Model/provider:
Prompt/config version:

Context used:
Memory used:
Files used:
Sources retrieved:
Tool outputs used:
Context excluded:
Stale or uncertain context:
Private/sensitive context included:
Missing context:
Assumptions carried forward:

Context completeness:
Next context needed:

⸻

Context Used

The receipt should list the main context used.

Examples:

* docs/token-burn-risk.md
* customer intake form response
* public Reddit thread
* pricing page
* previous report
* meeting transcript
* CSV summary
* browser page summary
* current project state packet
* memory note
* prior run receipt

This helps the user know what the agent relied on.

⸻

Memory Used

If memory influenced the run, the receipt should say so.

Examples:

* user preference memory
* project doctrine
* prior decision
* client-specific note
* workflow rule
* past report result
* previous approval state

Stackfax principle:

If memory influenced the run, the receipt should say what memory was used.

Memory should not act like invisible authority.

⸻

Files Used

If files were read or injected, the receipt should list them.

For each file, useful fields include:

* file name
* file path
* source
* date or version
* read-only or editable
* reason used
* whether sensitive data was present

This matters most when files contain business, customer, financial, legal, or private information.

⸻

Sources Retrieved

For RAG, search, or knowledge systems, the receipt should show what sources were retrieved.

Useful fields include:

* search query
* top sources
* source labels
* date labels
* relevance note
* whether stale sources were present
* whether conflicting sources were present

Stackfax verdict:

Retrieval should reduce reasoning load, not hide source selection.

⸻

Tool Outputs Used

If tools gathered context, the receipt should show the tool outputs that mattered.

Examples:

* web search result
* file search result
* database query
* spreadsheet filter
* API response
* terminal command output
* browser inspection
* screenshot analysis
* log scan

The receipt should not just say “used tools.”

It should say what the tools contributed.

⸻

Context Excluded

A strong context receipt should also show what was deliberately excluded.

Examples:

* full chat history excluded
* unrelated project notes excluded
* private customer data excluded
* old version docs excluded
* credentials excluded
* failed run notes excluded
* stale assumptions excluded
* raw logs excluded after summary

This helps prove that the stack is not blindly dumping everything into the model.

Stackfax rule:

Exclusion is part of context control.

⸻

Stale Or Uncertain Context

The receipt should mark stale or uncertain context.

Examples:

* pricing may have changed
* tool version may be old
* user report may be incomplete
* source is a forum comment
* memory note is unverified
* old workflow assumption
* outdated model benchmark
* prior report older than recheck window

Stackfax principle:

A stack verdict should age honestly.

⸻

Private Or Sensitive Context

The receipt should mark whether sensitive context was included.

Sensitive context may include:

* customer data
* business records
* emails
* private files
* financial records
* legal documents
* payment information
* credentials
* personal data
* medical or regulated information

The receipt should not expose the sensitive details unnecessarily.

It should show that sensitive context was present and handled intentionally.

⸻

Missing Context

A context receipt should identify missing context.

Examples:

* no workflow provided
* no pricing data available
* no tool version known
* no cost history
* no approval policy
* no source of truth
* no examples of failed runs
* no customer-data boundary
* no current stack inventory

Missing context is not a failure.

It is a review signal.

⸻

Assumptions Carried Forward

The receipt should show assumptions that influenced the output.

Examples:

* assumed cloud-first because no local workload was named
* assumed draft-only because customer contact was involved
* assumed human approval required because money/customer data appeared
* assumed current tool version based on user-provided screenshot
* assumed workflow is early-stage because no production evidence was provided

Assumptions should be visible so they can be corrected.

⸻

Context Completeness

The receipt can include a simple completeness label.

Possible labels:

* Complete enough for first verdict
* Partial context
* Missing key context
* Stale context risk
* Private context excluded
* Needs recheck
* Needs source verification
* Needs user confirmation

This helps the user understand how strong the output is.

⸻

Context Receipts And Run Receipts

Context receipts are part of run receipts.

A run receipt answers:

* what happened
* what changed
* what failed
* what cost
* what needs approval

A context receipt answers:

* what information the run used
* what information it excluded
* what assumptions shaped the result

Together, they make the run inspectable.

⸻

Context Receipts And Decision Receipts

Context receipts also support decision receipts.

A decision receipt should show why a verdict was made.

The context receipt shows what information fed that decision.

Example:

Decision:

Cloud-First

Context receipt shows:

* no local model requirement provided
* no always-on workflow provided
* user mainly described research and drafts
* no customer data isolation need stated
* hardware purchase not tied to workload

The decision becomes easier to trust.

⸻

Context Receipts And Memory Governance

Context receipts help keep memory honest.

They can show:

* which memories were injected
* which memories were ignored
* which memories were stale
* which memories should be deleted
* which memories need review
* which memory scope applied

Stackfax rule:

Inspectable memory is safer than invisible memory.

⸻

Context Receipts And Token Burn

Context receipts help identify token waste.

Warning signs:

* too many files loaded
* full history included
* irrelevant memory injected
* raw logs passed directly
* old context repeated
* RAG returned too many chunks
* premium model used to sort context mess

Stackfax verdict:

Do not make the model read the haystack. Build the system that hands it the needle bundle.

⸻

Context Receipts And Privacy

Context receipts help reduce privacy risk.

They show whether the system used only the context needed.

Privacy-safe context behavior includes:

* excluding private data unless required
* labeling sensitive context
* scoping memory by workflow
* using summaries instead of raw data
* avoiding unnecessary customer data
* keeping credentials out of prompts
* showing what was included

Customer data is not generic context.

⸻

Context Receipt Verdicts

Possible verdicts include:

* Context Receipt Needed
* Context Boundary Unclear
* Hidden Context Risk
* Context Bloat Risk
* Private Context Included
* Stale Context Risk
* Missing Context
* Context Scope Good
* Safe To Continue With Partial Context
* Recheck Needed

⸻

Common Risk Flags

Context receipt reviews may include:

* Context Bloat Risk
* Memory Scope Risk
* Private Memory Risk
* Retrieval Quality Risk
* Customer Data Risk
* Token Burn Risk
* Run Receipts Required
* Evidence Assembly Needed
* Decision Receipt Needed
* Version Drift Risk

⸻

What Would Improve The Score

A stack can improve context control by adding:

* context receipt template
* source labels
* memory-use record
* file-use record
* RAG result labels
* stale context labels
* sensitive context labels
* excluded context notes
* missing context notes
* assumption notes
* context completeness label
* 30-day context review

The goal is not more documentation for its own sake.

The goal is to make context visible enough to trust the output.

⸻

## Example Report Language

### Use language like:

This stack needs context receipts.

The output may be useful, but it is not clear which files, memories, retrieved sources, assumptions, or stale notes influenced the answer.

Before scaling, add a context receipt showing what was loaded, what was excluded, what was stale, and what context is still missing.

### Short version:

Context used should be context accounted for.

⸻

## Stackfax Principle

Context used should be context accounted for.

Hidden context creates hidden risk.

Inspectable memory is safer than invisible memory.

⸻

# Final Rule

Do not let context become invisible infrastructure.

If context shaped the answer, the stack should be able to show what context was used, what was excluded, what was stale, and what still needs review.
