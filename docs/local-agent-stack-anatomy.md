# Stackfax Local Agent Stack Anatomy

The Local Agent Stack Anatomy explains the major layers of a local or hybrid Ai agent setup.

The goal is to help users understand that a local agent stack is not just a model.

It is a system made of hardware, runtime, model, memory, tools, communication channels, schedules, permissions, and human approval.

## Core Idea

Local agents are not just “run a model.”

A local agent stack includes:

- Host machine
- Operating system
- Agent framework
- Model runner
- Model
- Memory
- Tools
- Communication channel
- Schedule or heartbeat
- File access
- Browser access
- Approval gates
- Safety boundaries

A model is one layer.

The stack is the whole system around it.

## Simple Stack Layers

A local agent stack may include:

1. Host machine
2. Local runtime
3. Model runner
4. Model
5. Agent framework
6. Memory
7. Tools
8. Communication channel
9. Schedule or heartbeat
10. Safety layer

## Host Machine

The host machine is where the local agent runs.

Examples:

- Existing laptop
- Old laptop
- Desktop
- Mac mini
- Local Ai box
- Home server
- VPS or cloud machine

Stackfax checks:

- Is this a personal daily machine?
- Is this a dedicated agent machine?
- Can the agent access personal files?
- Is the machine isolated enough?
- Does the hardware match the workload?

## Local Runtime

The local runtime is the environment that runs the agent stack.

It may include:

- macOS
- Linux
- Windows
- Docker
- Python
- Node.js
- Homebrew
- Local services
- Command-line tools

Stackfax checks:

- Is the setup repeatable?
- Is it fragile?
- Does it depend on many manual steps?
- Can the user troubleshoot it?
- Is the environment separate from sensitive personal use?

## Model Runner

The model runner manages local models.

Examples:

- Ollama
- LM Studio
- llama.cpp
- vLLM
- Other local inference tools

Stackfax checks:

- What models can it run?
- Is setup simple?
- Is speed acceptable?
- Is quality good enough for the task?
- Does it reduce API cost for the right jobs?
- Is it being used where local models actually fit?

## Model Layer

The model is the brain used for reasoning, drafting, summarizing, coding, classification, or review.

A stack may use:

- Local models
- Cloud models
- Hybrid routing
- Cheap draft models
- Strong review models
- Specialized coding models

Stackfax checks:

- Which model handles which job?
- Is the strongest model doing everything?
- Are local models being asked to do work they are not good at?
- Are cloud models being overused?
- Is model routing clear?

## Agent Framework

The agent framework coordinates tasks, tools, memory, prompts, and actions.

Examples:

- OpenClaw
- Claude Code-style workflows
- Custom scripts
- Agent platforms
- Local automation tools

Stackfax checks:

- What can the agent do?
- What tools can it call?
- What files can it access?
- What workflows are defined?
- What requires approval?
- What should be forbidden?

## Memory Layer

Memory stores context for the agent.

It may include:

- Markdown files
- Notes
- Project docs
- Vector databases
- Chat history
- Local folders
- Database records
- Long-term memory stores

Stackfax checks:

- What memory does the agent load?
- Is memory scoped to the task?
- Is private data exposed?
- Is history getting bloated?
- Is memory shared across unrelated workflows?
- Can memory create context bloat?

## Tool Layer

Tools are the agent’s hands.

Tools may include:

- Web search
- Browser control
- File reading
- File writing
- Code execution
- Shell commands
- APIs
- Spreadsheets
- Email
- Calendar
- CRM tools
- Automation platforms

Stackfax checks:

- Which tools are enabled?
- Which tools are high risk?
- Can the agent change files?
- Can the agent send messages?
- Can the agent access credentials?
- Can the agent touch customer, money, inventory, or production systems?

## Communication Channel

The communication channel is where the user talks to the agent or where the agent reports back.

Examples:

- Terminal
- Web UI
- Discord
- Slack
- Matrix
- Mattermost
- WhatsApp
- Email
- SMS

Stackfax checks:

- Can the agent send messages?
- Can it post publicly?
- Can it DM users?
- Can it contact customers?
- Are test channels separate?
- Is human approval required before sending?

## Schedule Or Heartbeat

A heartbeat means the agent runs on a schedule or watches for events.

Examples:

- Every hour
- Every morning
- When a file changes
- When a message arrives
- When a price changes
- When a support ticket appears
- When inventory changes

Stackfax checks:

- Does the agent run without being prompted?
- What can it do while unattended?
- Are there stop conditions?
- Are there logs?
- Is human approval required before action?
- Is the heartbeat safe for the workflow?

## Eyes

Agents may have eyes through screenshots, browser control, vision models, or screen reading.

This can be useful for:

- UI testing
- Reading public pages
- Checking dashboards
- Reviewing screenshots
- Browser-based workflows

Stackfax checks:

- What can the agent see?
- Is it viewing personal/private screens?
- Is it reading sensitive data?
- Is it relying on fragile UI layouts?
- Is screenshot automation safe enough for the task?

## Tentacles

Agents may have tentacles through tools and APIs.

Tentacles are what let the agent act.

Examples:

- Send email
- Update records
- Move files
- Trigger automations
- Edit spreadsheets
- Call APIs
- Post messages
- Run commands

Stackfax checks:

- What can the agent touch?
- What can it change?
- What can it delete?
- What requires approval?
- What should be forbidden?

## Safety Layer

The safety layer limits blast radius.

It may include:

- Dedicated machine
- Separate browser profile
- Separate accounts
- Separate folders
- Scoped API keys
- Test channels
- Approval gates
- Logs
- Backups
- Stop conditions
- Forbidden action list

Stackfax checks:

- Is the agent isolated?
- Are credentials protected?
- Are personal accounts separated?
- Are business accounts separated?
- Can mistakes be contained?
- Is there a rollback path?

## Local vs Cloud

A local stack may still need cloud models.

A cloud stack may still need local safety boundaries.

Stackfax checks whether the setup should be:

- Cloud-first
- Local-ready
- Hybrid
- Mac Mini justified
- Local overkill
- Cloud overkill

## Mac Mini Fit

A Mac mini may fit when the user wants:

- Dedicated Ai lab
- Local model testing
- OpenClaw experiments
- Separation from personal machine
- Lower blast radius
- Quiet always-on workspace
- Local workflow learning

A Mac mini may be overkill when:

- No workflow is defined
- User only needs occasional chat
- Cloud tools are enough
- Local models are not needed
- Hardware is being bought because of hype

## Common Risk Flags

Local agent stacks may trigger:

- Hardware Overbuild Risk
- Local Agent Isolation Needed
- Personal Machine Exposure Risk
- Communication Channel Risk
- Credential Isolation Risk
- Fragile UI Automation Risk
- Context Bloat Risk
- Agentic Trap Risk
- Human Approval Required
- Production Not Ready

## Best Starter Pattern

A safe starter local agent stack should usually:

1. Run on a contained machine or workspace.
2. Use non-sensitive files.
3. Use one clear workflow.
4. Observe and summarize first.
5. Draft but not send.
6. Require human approval before action.
7. Log what happened.
8. Add tools slowly.

## Stackfax Principle

If an agent has eyes, tentacles, and a heartbeat, it needs a cage.

## Final Rule

Local does not automatically mean safe.

A local agent stack still needs boundaries, approval gates, and a clear job.
