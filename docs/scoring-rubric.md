# Stackfax Scoring Rubric

The Stackfax scoring rubric defines how Ai stacks are reviewed, scored, and explained.

The goal is not to reward the biggest stack, the most expensive tools, or the newest hardware.

The goal is to measure whether the stack fits the task.

⸻

Core Question

Does this stack match the user’s workload, budget, skill level, risk tolerance, privacy needs, permission boundaries, and scaling goals?

A higher score does not mean the stack is bigger.

A higher score means the stack is better matched to the job.

⸻

Score Range

Stackfax uses a 0–100 Stack Score.

Suggested rating bands:

* 0–39: Poor fit
* 40–59: Risky or unclear fit
* 60–74: Usable starter stack
* 75–89: Strong stack
* 90–100: Excellent stack

The score should reflect fit, not flash.

⸻

Star Rating

Stackfax also uses a 1–5 star rating.

Suggested star bands:

* ⭐: 0–24
* ⭐⭐: 25–49
* ⭐⭐⭐: 50–69
* ⭐⭐⭐⭐: 70–84
* ⭐⭐⭐⭐⭐: 85–100

A 5-star stack is not always the most expensive stack.

A 5-star stack is the stack that best fits the task.

⸻

Main Categories

1. Use-Case Fit

Checks whether the stack matches what the user is actually trying to do.

Signals of good fit:

* clear primary use case
* tools match the task
* models are assigned to the right jobs
* hardware is justified by the workload
* workflow is understandable
* first useful workflow is defined

Signals of weak fit:

* no clear task
* too many tools
* copying a creator or vendor stack without context
* buying hardware before proving the workflow
* using one powerful model for everything
* optimizing the setup before defining the job

⸻

2. Cost And Token Discipline

Checks whether the stack avoids unnecessary spending and misrouted intelligence.

Signals of good fit:

* cheap models handle simple work
* strong models are reserved for judgment or final review
* token use is bounded
* session budget caps exist
* context is kept relevant
* subscriptions do not heavily overlap
* cost visibility exists

Signals of weak fit:

* premium models used for routine tasks
* large context loaded by default
* silent fallback escalation
* multiple overlapping subscriptions
* no cost visibility
* no budget caps
* no run receipts showing where tokens went

Core rule:

The leak is not token use. The leak is misrouted intelligence.

⸻

3. Model Routing

Checks whether the stack uses the right model for each layer of work.

Recommended pattern:

* cheap model drafts
* cheap or mid-tier model summarizes
* strong model reasons or decides
* human approves important actions

Signals of good fit:

* task types are separated
* routine work has cheaper routes
* escalation is visible
* premium models are used when the task earns them
* model fallback behavior is logged

Signals of weak fit:

* one model handles every task
* expensive model does extraction work
* no fallback visibility
* no model cap
* no separation between draft, review, and decision layers
* fallback chains silently escalate cost

⸻

4. Hardware Fit

Checks whether local hardware is actually needed.

Signals of good fit:

* hardware is tied to a specific workflow
* local model testing is justified
* privacy or isolation requirements are real
* always-on local workflows are proven
* dedicated workspace has a clear purpose
* existing hardware limits are understood

Signals of weak fit:

* buying a Mac mini because of hype
* buying local hardware before defining the workflow
* running cloud-friendly tasks locally for no clear reason
* overbuying RAM, VRAM, or storage without a workload
* treating hardware as the solution before stack design
* no comparison against cloud-first or hybrid options

⸻

5. Local Vs Cloud Fit

Checks whether the stack should be cloud-first, local-first, or hybrid.

Cloud-first fits when:

* tasks are mostly research, summaries, drafts, or reports
* local models are not required
* frontier reasoning matters more than local control
* uptime can be handled by hosted tools
* the user is still proving the workflow

Local-first fits when:

* privacy isolation matters
* local model testing matters
* the user needs a dedicated Ai lab
* repeated low-risk workloads can run locally
* the workload benefits from local runtime control

Hybrid fits when:

* cloud models handle heavy reasoning
* local tools handle safe, bounded workflows
* private or sensitive data stays isolated
* the workflow is proven enough to split cleanly
* cost can be reduced without losing quality

⸻

6. Permission And Approval Gates

Checks whether the stack has safe boundaries.

Human approval should usually be required before:

* sending messages
* posting publicly
* contacting customers
* changing files
* moving or deleting files
* connecting credentials
* accessing wallets
* touching financial accounts
* editing customer records
* changing inventory
* processing payments
* modifying production systems

Signals of good fit:

* approval gates are written down
* risky actions are draft-only first
* read-only access comes before write access
* agent permissions are narrow
* forbidden actions are clear

Signals of weak fit:

* agents can act without review
* credentials are broadly shared
* customer-facing actions are automated too early
* no written approval rules
* no list of forbidden actions
* permission expands faster than trust

Core rule:

The model can request an action. The system decides whether that action is allowed.

⸻

7. Privacy And Credential Isolation

Checks whether sensitive data is separated properly.

Signals of good fit:

* personal files are isolated
* client data is separated
* credentials are scoped
* browser sessions are not shared across clients
* agents have limited access
* private data is not loaded unless needed
* real customer data stays outside the public repo

Signals of weak fit:

* one agent has access to everything
* multiple clients share the same browser, session, or context
* credentials are stored loosely
* personal and business data are mixed
* private data is loaded into unnecessary model calls
* sensitive data is submitted before it is needed

⸻

8. Workflow Design

Checks whether the task is structured well.

Good workflow structure:

* define task
* gather data
* filter or extract with code/tools where possible
* summarize
* reason
* draft
* review
* human approves
* save/send only after approval
* log what happened

Weak workflow structure:

* one broad agent prompt does everything
* Ai performs deterministic work that code could do
* no clear inputs or outputs
* no checkpoint before action
* no separation between research, judgment, and execution
* no done-state
* no failure path

Stackfax principle:

Use code for extraction. Use Ai for judgment.

⸻

9. Reliability And Uptime

Checks whether the stack is ready for real use.

Signals of good fit:

* failures are expected
* restart behavior is understood
* logs exist
* important tasks have human review
* production workflows are not run from fragile setups
* uptime needs match hosting choice
* fallback plan exists

Signals of weak fit:

* always-on workflows run on a machine not designed for them
* updates or restarts can break work
* no fallback plan
* no monitoring
* no run receipts
* real customer workflows rely on experimental setups
* production behavior is not tested

⸻

10. Run Receipts And Observability

Checks whether the user can see what the stack did.

A useful run receipt should show:

* what task was requested
* what model was used
* why that model was selected
* what tools were used
* what data/files/accounts were touched
* what changed
* what failed
* what it cost
* what needs human review next

Signals of weak fit:

* no logs
* no cost receipt
* no model trace
* no tool trace
* no approval record
* no way to review failed runs
* no evidence behind agent claims

Core rule:

Agent output is a claim. A run receipt is evidence.

⸻

11. Memory And Context Governance

Checks whether memory/context is useful, safe, and inspectable.

Signals of good fit:

* memory is inspectable
* memory is searchable
* memory is scoped by project or workflow
* users can edit or delete memory
* memory injection is controlled
* durable state is separated from raw history
* sensitive memory is not saved by default

Signals of weak fit:

* invisible memory
* everything is remembered by default
* bad runs are saved as durable truth
* failed tool loops enter memory without validation
* private data is mixed across contexts
* memory is used without the user knowing why

Core rule:

Pass state, not history.

⸻

12. Scaling Path

Checks whether the stack can grow without breaking cost, safety, or control.

Signals of good fit:

* first workflow is clear
* future upgrades are staged
* more tools are added only after need is proven
* costs can be tracked
* permissions can be tightened
* new users or clients can be isolated
* 30-day recheck plan exists

Signals of weak fit:

* scaling plan depends only on buying bigger hardware
* costs are unknown
* more agents are added before the first workflow is proven
* client/customer boundaries are unclear
* no 30-day recheck plan
* version drift is ignored

⸻

Common Risk Badges

Stackfax may apply badges such as:

* StackChecked
* Token-Smart
* Cloud-First
* Local-Ready
* Hardware Justified
* Hardware Not Required Yet
* Overbuild Risk
* Human Approval Required
* Customer Data Risk
* Credential Isolation Risk
* Context Bloat Risk
* Silent Escalation Risk
* Fragile UI Automation Risk
* Vendor Stack Overkill Risk
* Version Drift Risk
* Migration Risk
* Cost Visibility Missing
* Run Receipts Required
* Uptime Risk
* Production Not Ready

⸻

Scoring Guidance

A sample scoring split:

* Use-case fit: 15 points
* Cost and token discipline: 15 points
* Model routing: 10 points
* Hardware fit: 10 points
* Local vs cloud fit: 10 points
* Permission and approval gates: 15 points
* Privacy and credential isolation: 10 points
* Workflow design: 10 points
* Reliability and uptime: 5 points

Total:

100 points

This base weighting can change by report type.

⸻

Report-Type Weighting Notes

A Hardware Verdict may weigh more heavily:

* hardware fit
* local vs cloud fit
* workload clarity
* cost discipline
* upgrade path

A Token Burn Audit may weigh more heavily:

* cost and token discipline
* model routing
* context bloat
* tool-loop burn
* cost visibility

A Business Automation Safety Check may weigh more heavily:

* approval gates
* credential isolation
* customer data risk
* workflow design
* production readiness

A Vendor Stack Verdict may weigh more heavily:

* use-case fit
* setup complexity
* overbuild risk
* vendor lock-in risk
* hidden cost risk

A Stackfax Recheck may weigh more heavily:

* version drift
* migration fit
* current stack changes
* new bottlenecks
* whether the original verdict still fits

⸻

Score Interpretation

The score should be explained in plain language.

Do not give a number without a reason.

A useful score explanation should include:

* why the stack scored well
* what pulled the score down
* which risk flags matter most
* what one change would improve the score most
* whether the user should build, buy, wait, simplify, test, or recheck

⸻

What Should Improve A Score

Reward:

* clear workflow
* good tool-task fit
* cost discipline
* model routing
* approval gates
* limited permissions
* credential isolation
* private-data boundaries
* run receipts
* realistic hardware choice
* local/cloud fit
* rollback plan
* recheck plan

⸻

What Should Lower A Score

Penalize:

* unclear use case
* tool pile without workflow
* premium model overuse
* hidden token burn
* missing approval gates
* broad credential access
* customer data risk
* no cost visibility
* fragile UI automation
* no run receipts
* overbuilt hardware
* no fallback or rollback
* production use without testing
* version drift ignored

⸻

Final Rule

Do not reward complexity by default.

Reward fit, clarity, safety, cost discipline, and upgrade path.

A small stack that does the job safely can score higher than a huge stack that is expensive, risky, or unclear.
