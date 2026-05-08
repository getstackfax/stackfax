# Agent ROI

Agent ROI is the Stackfax dimension for measuring whether an agent creates real operational value.

It does not ask whether the agent looked busy.

It asks whether the agent turned intent into a verified outcome.

Core rule:

Agent ROI is not activity. It is verified useful work.

⸻

## Core Formula

Agent ROI = completed useful work - supervision cost - model/tool cost - risk - cleanup
An agent that completes a task but creates hidden cleanup, review burden, cost overruns, or safety risk may have low ROI even if it appears productive.

A useful agent should make the workflow better after the full cost is counted.

⸻

## Core Question

Did the agent produce a useful, verifiable outcome that was worth the supervision, cost, risk, and cleanup?

If the answer is unclear, Agent ROI is unclear.

⸻

## What Agent ROI Measures

1. Execution

Did the agent actually complete the job?

A useful agent should produce an outcome that can be:

* checked
* used
* shipped
* filed
* sent
* reviewed
* acted on
* reused

Weak execution signs:

* output is vague
* task status is unclear
* agent claims success without evidence
* output cannot be used without major rewrite
* no one can tell what actually changed

Stackfax rule:

Agent output is a claim. A run receipt is evidence.

⸻

2. Reliability

Can the agent complete the job again?

One lucky run is not a system.

Repeatability matters more than demo quality.

Strong reliability signs:

* same workflow can run again
* inputs and outputs are clear
* failures are understandable
* retry rules exist
* results can be checked
* receipts exist
* human review points are defined

Weak reliability signs:

* works once, fails randomly
* depends on fragile UI paths
* no stop condition
* no fallback plan
* no rollback
* no clear owner for failures

⸻

3. Supervision Cost

How much human babysitting did the agent require?

If a human has to constantly monitor, rescue, rewrite, or verify every step, the agent may not be creating much leverage.

Supervision cost includes:

* watching the run
* correcting errors
* rewriting outputs
* checking sources
* rerunning failed steps
* cleaning files
* reviewing unsafe actions
* explaining what the agent did
* undoing side effects

A useful agent reduces net operator burden.

It does not just move work from doing to babysitting.

⸻

4. Cost Discipline

Did the agent spend tokens, API calls, subscriptions, tools, or hardware time wisely?

Agent ROI drops when the agent:

* uses premium models for simple work
* loads unnecessary context
* retries too much
* calls tools repeatedly
* silently escalates to expensive models
* requires overlapping subscriptions
* needs hardware that the workflow does not justify
* creates cost that cannot be traced to useful output

Stackfax rule:

The leak is not token use. The leak is misrouted intelligence.

⸻

5. Risk Control

Did the agent stay inside permissions and approval gates?

Agent ROI is reduced when the system creates:

* privacy risk
* customer data risk
* credential risk
* compliance risk
* financial risk
* security risk
* reputation risk
* production risk
* public posting risk

### A high-ROI agent should not create hidden blast radius.

### If the agent can touch customers, money, inventory, credentials, files, or production systems, approval gates and receipts matter.

⸻

6. Cleanup Burden

Did the agent leave behind a mess?

Cleanup burden includes:

* broken files
* half-finished tasks
* duplicate notes
* bad records
* unclear logs
* wrong summaries
* stale memory
* unreviewed drafts
* noisy outputs
* confusing tool changes

An agent that creates cleanup debt may have negative ROI even when it appears productive.

⸻

7. Compounding Value

Did the agent leave behind reusable value?

Examples include:

* better workflow
* reusable scripts
* documentation
* structured data
* review checklists
* cleaner handoffs
* improved prompts
* reusable reports
* run receipts
* lessons that improve the next run
* reduced future supervision
* better routing rules

The best agents do not just save time once.

They improve the next run.

⸻

Agent ROI Score Bands

Score

Meaning

0–20

Toy or demo only

21–40

Helpful assistant, not reliable worker

41–60

Useful with heavy supervision

61–80

Real workflow value with approval gates

81–100

Repeatable operating leverage
The score should explain what would improve the next run.

Do not give a high Agent ROI score just because the agent produced a lot of output.

⸻

# Common Failure Modes

## Activity Without Outcome

The agent produced text, logs, or actions, but nothing useful changed.

Warning signs:

* long transcript
* many tool calls
* no usable deliverable
* unclear status
* no evidence of completion

Verdict:

Busy is not the same as useful.

⸻

## Hidden Cleanup

The agent saved time up front but created more review, correction, or repair work later.

Warning signs:

* output needs heavy rewriting
* source claims need checking
* files are messy
* agent made partial changes
* operator must reconstruct what happened

Verdict:

Saved time does not count until cleanup is counted.

⸻

Unpriced Risk

The agent created risk that was not included in the ROI calculation.

Warning signs:

* customer data touched without review
* credentials exposed
* messages drafted or sent incorrectly
* public posting risk
* production systems changed
* payment or account risk

Verdict:

Risk is part of ROI.

⸻

## One-Off Win

The agent worked once, but the process cannot be repeated reliably.

Warning signs:

* no template
* no receipt
* no defined inputs
* no repeatable workflow
* no failure handling
* no recheck plan

Verdict:

One lucky run is not a system.

⸻

## No Compounding Asset

The agent completed a task but left nothing reusable behind.

Warning signs:

* no improved prompt
* no reusable workflow
* no saved checklist
* no clean handoff
* no structured output
* no lesson for next time

Verdict:

The best agent runs improve future agent runs.

⸻

## Negative Agent ROI

An agent can have negative ROI when it creates more burden than value.

Examples:

* output requires more cleanup than manual work
* agent loops and burns tokens
* agent touches risky systems without approval
* agent produces unverifiable claims
* agent creates noisy memory
* agent breaks workflows
* agent requires constant supervision
* agent adds complexity without improving output

Stackfax should flag this clearly.

Possible verdict:

Agent activity is high, but Agent ROI is low.

⸻

## Agent ROI Inputs

A Stackfax report may ask:

* What task did the agent attempt?
* What output was produced?
* Who reviewed it?
* What changed?
* What did it cost?
* What tools were touched?
* What approval was required?
* What failed?
* What cleanup was needed?
* Could the workflow run again?
* What reusable asset was created?
* What should improve next time?

⸻

## Agent ROI And Run Receipts

Agent ROI depends on evidence.

A useful run receipt should show:

* task requested
* model used
* tools touched
* files or systems accessed
* output produced
* changes made
* failures
* cost estimate
* approval state
* next action

Without receipts, Agent ROI becomes a guess.

# Stackfax rule:

The agent should not be the only witness to its own success.

⸻

## Agent ROI And Business Workflows

For business use, Agent ROI should include operational value, not just time saved.

Business Agent ROI may include:

* faster lead response
* fewer missed follow-ups
* cleaner intake
* better support drafts
* fewer handoff errors
* clearer reports
* reduced manual cleanup
* better review quality
* lower token/API waste
* more visible failure handling

But it should also subtract:

* review time
* cleanup time
* customer data risk
* credential risk
* brand risk
* compliance risk
* tool cost
* subscription cost

Agent ROI is verified outcome, not automation theater.

⸻

## Agent ROI And Evaluation

Agent ROI should be connected to workflow tests.

Good evaluation asks:

* Did the output match the expected result?
* Was the result useful?
* Was the result safe?
* Was the result cheaper than the alternative?
* Was review effort reasonable?
* Did the workflow repeat?
* Did receipts prove what happened?
* Did the next run improve?

Benchmarks rank models.

Workflow tests reveal fit.

⸻

What Would Improve The Score

An agent can improve ROI by adding:

* clear workflow
* definition of done
* bounded permissions
* approval gates
* model routing
* cost visibility
* run receipts
* failure handling
* rollback plan
* reusable templates
* structured outputs
* reduced cleanup burden
* better evaluation checks
* 30-day recheck

The goal is not more agent activity.

The goal is more verified useful work.

⸻

Example Report Language

Use language like:

This stack has unclear Agent ROI.

The agent appears active, but the useful outcome, review cost, token cost, cleanup burden, and risk are not yet visible.

Before expanding automation, define one repeatable workflow, require a run receipt, and measure whether the agent produces a usable result with less supervision than the manual process.

Short version:

Agent ROI is not activity. It is verified useful work.

⸻

Common Badges And Verdicts

Agent ROI reviews may use:

* Agent ROI Unclear
* Agent ROI Verified
* Activity Without Outcome
* Heavy Supervision Required
* Run Receipts Required
* Evaluation Layer Missing
* Cost Visibility Missing
* Approval Gates Missing
* Useful With Review
* Repeatable Operating Leverage

⸻

Stackfax Principle

A useful agent should get real work done safely, repeatedly, and measurably.

The best agents do not just save time once.

They improve the next run.

⸻

Final Rule

Do not measure the agent by how busy it looked.

Measure it by the useful work completed, the evidence left behind, and the burden it removed after cost, risk, supervision, and cleanup are counted.
