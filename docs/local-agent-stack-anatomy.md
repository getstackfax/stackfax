# Stackfax Local Agent Stack Anatomy

The Local Agent Stack Anatomy explains the major layers of a local or hybrid Ai agent setup.

The goal is to help users understand that a local agent stack is not just a model.

It is a system made of hardware, runtime, model routing, memory, tools, communication channels, schedules, permissions, receipts, and human approval.

⸻

Core Idea

Local agents are not just “run a model.”

A local agent stack includes:

* host machine
* operating system
* local runtime
* model runner
* model
* agent framework
* memory
* tools
* communication channel
* schedule or heartbeat
* file access
* browser access
* approval gates
* run receipts
* safety boundaries

A model is one layer.

The stack is the whole system around it.

⸻

Simple Stack Layers

A local agent stack may include:

1. Host machine
2. Local runtime
3. Model runner
4. Model layer
5. Agent framework
6. Memory layer
7. Tool layer
8. Communication channel
9. Schedule or heartbeat
10. Run receipt layer
11. Safety layer

The more layers the agent can touch, the more boundaries it needs.

⸻

Host Machine

The host machine is where the local agent runs.

Examples:

* existing laptop
* old laptop
* desktop
* Mac mini
* local Ai box
* GPU rig
* home server
* VPS or cloud machine

Stackfax checks:

* Is this a personal daily machine?
* Is this a dedicated agent machine?
* Can the agent access personal files?
* Is the machine isolated enough?
* Does the hardware match the workload?
* Can mistakes be contained?
* Is the machine reliable enough for the workflow?

A dedicated machine can lower blast radius, but it does not automatically make the setup safe.

⸻

Local Runtime

The local runtime is the environment that runs the agent stack.

It may include:

* macOS
* Linux
* Windows
* Docker
* Python
* Node.js
* Homebrew
* local services
* command-line tools
* background jobs
* launch agents or cron jobs

Stackfax checks:

* Is the setup repeatable?
* Is it fragile?
* Does it depend on many manual steps?
* Can the user troubleshoot it?
* Is the environment separate from sensitive personal use?
* Are secrets stored safely?
* Can the setup be restored after failure?

⸻

Model Runner

The model runner manages local models.

Examples:

* Ollama
* LM Studio
* llama.cpp
* vLLM
* other local inference tools

Stackfax checks:

* What models can it run?
* Is setup simple?
* Is speed acceptable?
* Is quality good enough for the task?
* Does it reduce API cost for the right jobs?
* Is it being used where local models actually fit?
* Is the user expecting local models to replace frontier reasoning too early?

Local models reduce cost only when they fit a repeated workload.

⸻

Model Layer

The model is the brain used for reasoning, drafting, summarizing, coding, classification, extraction, or review.

A stack may use:

* local models
* cloud models
* hybrid routing
* cheap draft models
* strong review models
* specialized coding models
* model routers

Stackfax checks:

* Which model handles which job?
* Is the strongest model doing everything?
* Are local models being asked to do work they are not good at?
* Are cloud models being overused?
* Is model routing clear?
* Is escalation visible?
* Are cost and quality tracked by task?

Core rule:

The expensive model should not be doing every step.

⸻

Agent Framework

The agent framework coordinates tasks, tools, memory, prompts, and actions.

Examples:

* OpenClaw
* Claude Code-style workflows
* custom scripts
* agent platforms
* local automation tools

Stackfax checks:

* What can the agent do?
* What tools can it call?
* What files can it access?
* What workflows are defined?
* What requires approval?
* What should be forbidden?
* What happens when the agent fails?
* Does the agent leave a receipt?

The framework is not just the worker.

It is the coordination layer.

⸻

Memory Layer

Memory stores context for the agent.

It may include:

* markdown files
* notes
* project docs
* vector databases
* chat history
* local folders
* database records
* long-term memory stores
* session summaries
* knowledge vaults

Stackfax checks:

* What memory does the agent load?
* Is memory scoped to the task?
* Is private data exposed?
* Is history getting bloated?
* Is memory shared across unrelated workflows?
* Can memory create context bloat?
* Can the user inspect, edit, or delete memory?
* Are failed runs saved as durable truth?

Strong memory is inspectable.

Weak memory is invisible.

Core rule:

Pass state, not history.

⸻

Tool Layer

Tools are the agent’s hands.

Tools may include:

* web search
* browser control
* file reading
* file writing
* code execution
* shell commands
* APIs
* spreadsheets
* email
* calendar
* CRM tools
* automation platforms
* databases
* source control
* deployment tools

Stackfax checks:

* Which tools are enabled?
* Which tools are high risk?
* Can the agent change files?
* Can the agent send messages?
* Can the agent access credentials?
* Can the agent touch customer, money, inventory, or production systems?
* Are tool calls logged?
* Are tool failures visible?

Tool access without tool accounting creates invisible risk.

⸻

Communication Channel

The communication channel is where the user talks to the agent or where the agent reports back.

Examples:

* terminal
* web UI
* Discord
* Slack
* Matrix
* Mattermost
* WhatsApp
* email
* SMS

Stackfax checks:

* Can the agent send messages?
* Can it post publicly?
* Can it DM users?
* Can it contact customers?
* Are test channels separate?
* Is human approval required before sending?
* Are channel permissions scoped?
* Are messages logged or receipt-backed?

Communication channels turn an agent from private helper into external actor.

That requires stronger approval gates.

⸻

Schedule Or Heartbeat

A heartbeat means the agent runs on a schedule or watches for events.

Examples:

* every hour
* every morning
* when a file changes
* when a message arrives
* when a price changes
* when a support ticket appears
* when inventory changes

Stackfax checks:

* Does the agent run without being prompted?
* What can it do while unattended?
* Are there stop conditions?
* Are there logs?
* Are there run receipts?
* Is human approval required before action?
* Is the heartbeat safe for the workflow?
* Can the heartbeat be paused quickly?

A scheduled agent needs more governance than an on-demand chat.

⸻

Eyes

Agents may have eyes through screenshots, browser control, vision models, screen reading, or document viewing.

This can be useful for:

* UI testing
* reading public pages
* checking dashboards
* reviewing screenshots
* browser-based workflows
* monitoring visible state

Stackfax checks:

* What can the agent see?
* Is it viewing personal/private screens?
* Is it reading sensitive data?
* Is it relying on fragile UI layouts?
* Is screenshot automation safe enough for the task?
* Is there a better API path?
* Are screenshots saved or discarded safely?

Eyes create privacy risk.

They also create fragility when the workflow depends on pixels instead of state.

⸻

Tentacles

Agents may have tentacles through tools and APIs.

Tentacles are what let the agent act.

Examples:

* send email
* update records
* move files
* trigger automations
* edit spreadsheets
* call APIs
* post messages
* run commands
* deploy code
* modify settings

Stackfax checks:

* What can the agent touch?
* What can it change?
* What can it delete?
* What requires approval?
* What should be forbidden?
* What gets logged?
* What has rollback?

The more tentacles, the stronger the cage needs to be.

⸻

Run Receipt Layer

Run receipts explain what happened in plain language.

A useful run receipt should show:

* what task was requested
* what model was used
* what tools were touched
* what files or systems were accessed
* what changed
* what failed
* what it cost
* what approval was requested or granted
* what needs review next

Stackfax checks:

* Can a non-technical operator understand what happened?
* Are tool calls visible?
* Are file changes visible?
* Are approvals visible?
* Are failures visible?
* Is cost visible?
* Is the next action clear?

Core rule:

Agent output is a claim. A run receipt is evidence.

⸻

Safety Layer

The safety layer limits blast radius.

It may include:

* dedicated machine
* separate browser profile
* separate accounts
* separate folders
* scoped API keys
* test channels
* approval gates
* logs
* run receipts
* backups
* stop conditions
* forbidden action list
* rollback plan
* read-only mode
* sandbox environment

Stackfax checks:

* Is the agent isolated?
* Are credentials protected?
* Are personal accounts separated?
* Are business accounts separated?
* Can mistakes be contained?
* Is there a rollback path?
* Can access be revoked quickly?
* Are high-risk actions blocked by default?

Safety should be designed before autonomy expands.

⸻

Local vs Cloud

A local stack may still need cloud models.

A cloud stack may still need local safety boundaries.

Stackfax checks whether the setup should be:

* Cloud-First
* Local-Ready
* Hybrid
* Mac Mini Justified
* Local Overkill
* Cloud Overkill
* Recheck Needed

Cloud-first is not failure.

Local-first is not automatically advanced.

Hybrid is often practical.

The question is which setup fits the workflow, risk, cost, and maintenance reality.

⸻

Mac Mini Fit

A Mac mini may fit when the user wants:

* dedicated Ai lab
* local model testing
* OpenClaw experiments
* separation from personal machine
* lower blast radius
* quiet always-on workspace
* local workflow learning
* macOS tooling

A Mac mini may be overkill when:

* no workflow is defined
* user only needs occasional chat
* cloud tools are enough
* local models are not needed
* hardware is being bought because of hype
* token burn is really a routing problem
* the workload needs GPU/VRAM tradeoffs the Mac mini does not fit

Hardware should match the job, not the hype.

⸻

Common Risk Flags

Local agent stacks may trigger:

* Hardware Overbuild Risk
* Local Agent Isolation Needed
* Personal Machine Exposure Risk
* Communication Channel Risk
* Credential Isolation Risk
* Fragile UI Automation Risk
* Context Bloat Risk
* Agentic Trap Risk
* Human Approval Required
* Production Not Ready
* Run Receipts Required
* Private Memory Risk
* Tool Touch List Missing
* Cost Visibility Missing
* Version Drift Risk

⸻

Best Starter Pattern

A safe starter local agent stack should usually:

1. Run on a contained machine or workspace.
2. Use non-sensitive files.
3. Use one clear workflow.
4. Observe and summarize first.
5. Draft but not send.
6. Require human approval before action.
7. Log what happened.
8. Leave a run receipt.
9. Add tools slowly.

Do not start with full autonomy.

Start with proof that one workflow works safely.

⸻

Stackfax Principle

If an agent has eyes, tentacles, and a heartbeat, it needs a cage.

Local does not automatically mean safe.

A local agent stack still needs boundaries, approval gates, receipts, and a clear job.

⸻

Final Rule

Local does not automatically mean safe.

A local agent stack still needs boundaries, approval gates, and a clear job.
