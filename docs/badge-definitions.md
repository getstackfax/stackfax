# Stackfax Badge Definitions 

Stackfax badges give quick context about what a stack is good for, where it is risky, and what kind of user or workflow it fits.

Stars show overall quality.

Badges show specific traits.

A stack can have strong badges and still need limits.

A badge is a signal, not a guarantee.

⸻

Core Rule

Badges should make the verdict easier to understand.

They should not create false confidence.

Stackfax badges should always be tied to:

* use case
* risk level
* checked date
* workflow context
* approval status
* known limits

⸻

StackChecked

The stack has been reviewed using Stackfax criteria.

This does not mean the stack is perfect.

It means the stack has been inspected for:

* use-case fit
* cost risk
* token burn risk
* safety
* privacy
* hardware needs
* model routing
* approval gates
* permission boundaries

StackChecked should include a checked date.

Example:

StackChecked · Checked May 2026 · Recheck in 30 days

Core meaning:

Core meaning:

This stack was checked for this job, at this time, with these limits.

⸻

Token-Smart

The stack uses model routing or cost controls to avoid wasting premium-model tokens on simple work.

Common signs:

* cheap models handle routine tasks
* strong models are reserved for hard reasoning
* premium models are not used for every draft, summary, or classification
* the stack has a clear cost-control strategy
* context is loaded intentionally
* fallback escalation is visible
* run receipts show model/cost behavior

Stackfax principle:

The leak is not token use. The leak is misrouted intelligence.

⸻

Beginner-Friendly

The stack is understandable and usable by a beginner.

Common signs:

* simple setup
* clear instructions
* limited permissions
* no unnecessary hardware
* human approval before important actions
* low risk of accidental token burn
* clear first workflow
* low blast radius

Public copy should use Beginner-Friendly, not “Noob-Friendly.”

Internal note:

“Noob” can stay internal shorthand, but public badge language should be respectful.

⸻

Cloud-Only

The stack does not require local hosting.

Common signs:

* uses hosted models or APIs
* no local model setup required
* no dedicated machine required
* good fit for business users, writers, researchers, or beginners testing workflows
* setup simplicity matters more than local control

This badge does not mean the stack is weak.

It means local hardware is not required for the job.

⸻

Cloud-First

The stack should begin in the cloud before considering local hardware.

Common signs:

* user is still learning
* workflows are not proven yet
* local hosting is not justified yet
* hardware purchase would be premature
* hosted tools can prove the workflow faster
* model routing matters more than hardware

Verdict meaning:

Prove the workflow before buying local hardware.

⸻

Local-Ready

The stack can benefit from local hosting or local models, but may still need hybrid routing.

Common signs:

* privacy matters
* always-on workflows are useful
* user has or may need a dedicated machine
* local model testing is part of the goal
* hardware may be justified by the workload
* routine tasks may run locally
* cloud models may still handle hard reasoning

Local-ready does not mean local-only.

⸻

Hardware Not Required Yet

The user does not need to buy dedicated hardware yet.

Common signs:

* cloud tools are enough
* workflows are lightweight
* user is still testing
* local privacy needs are not strong
* hardware would be overkill
* no specific local workload exists
* token burn is really a routing problem

Short meaning:

Do not buy the machine before you can name the job.

⸻

Mac Mini Justified

A dedicated Mac mini or similar local machine makes sense.

Common signs:

* user wants isolated Ai experimentation
* user wants local model testing
* always-on agents are useful
* personal machine separation matters
* workload justifies dedicated hardware
* macOS tooling fits the workflow
* approval gates and permission boundaries are understood

Important note:

A Mac mini should be justified as a controlled Ai lab, not as a hype purchase.

⸻

Hardware Justified

A dedicated local machine, GPU rig, Mac mini, or local Ai box is justified by the workload.

Common signs:

* specific workload exists
* local execution solves a real problem
* privacy, control, cost, or always-on needs are real
* repeated usage justifies the cost
* local/cloud tradeoff has been considered
* the user can name what the hardware unlocks

Use this badge when the hardware fit is broader than Mac mini specifically.

⸻

Overkill Warning

The stack is likely more expensive or complex than the job requires.

Common signs:

* premium models used for simple tasks
* hardware purchased too early
* too many tools connected
* no clear workflow
* user copied an expert stack without understanding it
* local-only plan when cloud-first or hybrid would work better
* setup complexity increases faster than useful output

Stackfax line:

Do not build a NASA rig to play FarmSim.

⸻

Human Approval Required

The stack includes workflows that should not run fully autonomously.

Human approval should be required before:

* sending messages
* posting publicly
* editing customer records
* changing inventory
* touching money
* handling credentials
* modifying production systems
* deleting or moving files
* contacting customers
* processing payments
* changing account settings

Approval should be visible in the run receipt.

⸻

Customer Data Risk

The stack may touch customer information, business records, sales data, support messages, CRM data, or private communications.

This badge means the stack needs stronger:

* privacy rules
* approval gates
* credential isolation
* data boundaries
* run receipts
* access limits

Customer data makes the stack higher trust.

It should not be treated like generic context.

⸻

Credential Isolation Risk

The stack may expose too much access through shared credentials, browser sessions, API keys, accounts, or workspaces.

Common signs:

* one agent can access too many tools
* personal and business accounts are mixed
* clients share one browser session
* API keys are reused across workflows
* secrets are visible to agents
* files and memory are not separated

Core rule:

One agent should not get the keys to the whole building.

⸻

Privacy-First

The stack is designed to limit unnecessary exposure of private data.

Common signs:

* minimal access
* clear permissions
* local or isolated workflows where useful
* no unnecessary syncing
* approval before private data is processed or shared
* scoped memory
* private data is not loaded unless needed
* sensitive workflows are separated

Privacy-first does not mean local-only.

It means data exposure is intentionally limited.

⸻

Business Automation Ready

The stack is suitable for controlled business workflows.

Common signs:

* approval gates exist
* customer-facing actions are reviewed
* cost controls exist
* workflows are documented
* private data risks are understood
* permissions are scoped
* run receipts exist
* failure handling exists
* owner accountability is clear

This badge should be used carefully.

Most early stacks should be Safe To Test before they are Business Automation Ready.

⸻

Safe To Test

The stack is appropriate for limited testing with controlled inputs and bounded permissions.

Common signs:

* low-risk workflow
* non-sensitive data
* human review exists
* no production access
* no external messages without approval
* failures can be contained
* logs or receipts exist

Safe To Test does not mean production-ready.

⸻

Production Not Ready

The stack should not be trusted with real operations yet.

Common signs:

* no approval gates
* no run receipts
* unclear permissions
* broad credential access
* no failure plan
* no rollback
* test and production are mixed
* agent can act without review
* customer or business systems are exposed

Short meaning:

It worked once. That does not make it production-ready.

⸻

Run Receipts Required

The stack needs clearer evidence of what agents did.

Common signs:

* agent claims success without proof
* logs are technical but not operator-readable
* tool calls are not summarized
* file changes are unclear
* cost is invisible
* approval state is missing
* failures are hard to review

Stackfax principle:

Agent output is a claim. A run receipt is evidence.

⸻

Communication Channel Risk

The stack can speak through channels where audience, approval state, or workspace boundaries may be unclear.

Common signs:

* agent can send messages
* agent can DM users
* agent can post publicly
* test and production channels are mixed
* agent can reply from a brand account
* customer-facing channels are connected
* communication receipts are missing

Core rule:

The channel is part of the stack.

⸻

Fragile UI Automation Risk

The stack depends on screens, clicks, browser layouts, screenshots, or unstable app interfaces.

Common signs:

* agent clicks through many pages
* workflow depends on a button location
* no API fallback exists
* browser session may expire
* captcha, pop-up, or layout changes can break the workflow
* important actions happen through UI automation

Stackfax principle:

If a workflow breaks because a button moved, it is not production-ready.

⸻

Context Bloat Risk

The stack loads too much context into tasks that do not need it.

Common signs:

* entire histories loaded by default
* every file is included
* memory is always injected
* long documents are dumped into simple tasks
* irrelevant context increases cost and confusion
* sensitive data is loaded unnecessarily

Core rule:

Do not make the model read the haystack. Build the system that hands it the needle bundle.

⸻

Model Routing Needed

The stack does not clearly assign the right model to the right job.

Common signs:

* one model handles everything
* premium model does simple work
* local models are used for tasks they cannot handle well
* fallback escalation is invisible
* no draft/review/decision split exists

Recommended pattern:

* cheap model drafts
* cheap or mid-tier model summarizes
* strong model reasons or reviews
* human approves important actions

⸻

Subscription Overlap Risk

The user may be paying for overlapping Ai access without a clear workflow reason.

Common signs:

* multiple premium subscriptions active
* same task tested across many tools without a decision
* no primary daily model
* no assigned model jobs
* API and chat subscriptions are mixed without a plan
* local models, routers, and premium subscriptions overlap

Core rule:

Every paid tool should have a job.

⸻

API Budget Required

The stack uses APIs, routers, or agent workflows without clear budget controls.

Common signs:

* no monthly budget
* no per-task budget
* no model cap
* no escalation alert
* no cost receipt
* fallback chains may call expensive models
* agents can loop or retry indefinitely

Use when spend can grow faster than the user realizes.

⸻

Version Drift Risk

The stack may become outdated because models, prices, limits, tooling, OpenClaw versions, or provider policies changed.

Common signs:

* recommendation depends on a specific tool version
* model/pricing assumptions may be stale
* OpenClaw or local runner changed
* provider rate limits changed
* creator guide may be outdated
* stack needs recheck after a major update

Core rule:

Ai stacks expire. Stackfax keeps them checked.

⸻

Migration Risk

The user may be switching stacks, tools, models, hardware, or providers without a proven reason.

Common signs:

* switching because of hype
* no defined bottleneck
* no rollback plan
* no current-stack inventory
* no cost comparison
* no output comparison
* migration may break memory, tools, or credentials

Stackfax principle:

Migration is not progress unless the workflow gets better.

⸻

Agent ROI Unclear

The stack appears active, but useful outcome is not yet proven.

Common signs:

* agent does lots of work with unclear value
* supervision cost is high
* cleanup cost is high
* no success metric exists
* no repeatable output exists
* no evidence of time, cost, risk, or quality improvement

Core rule:

Agent ROI is not activity. It is verified useful work.

⸻

Evaluation Layer Missing

The stack lacks a way to test whether outputs are good enough for the workflow.

Common signs:

* model choice based only on benchmarks
* no workflow-specific tests
* no review rubric
* no failure examples
* no comparison against expected output
* no quality gate before automation

Stackfax principle:

Benchmarks rank models. Workflow tests reveal fit.

⸻

Degen Mode Warning

The stack is being used around trading, speculation, crypto, prediction markets, or other high-risk financial contexts.

This badge means the stack should be research-only unless strong human controls exist.

Stackfax does not treat financial automation casually.

Human approval is required before any action involving:

* money
* trading
* wallets
* exchanges
* financial accounts
* payments
* leverage
* automated orders

Use this badge to slow the system down.

⸻

Badge Trust Rule

Do not use badges as fake certification.

Badges do not guarantee:

* security
* compliance
* legal approval
* financial outcomes
* trading results
* business results
* future safety
* permanent correctness

Badges help explain the stack.

They do not replace judgment.

⸻

Final Rule

Stars show the overall verdict.

Badges show why.

A good Stackfax badge makes the stack easier to understand without making it sound safer than it is.

