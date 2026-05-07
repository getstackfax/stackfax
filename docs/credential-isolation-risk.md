# Credential Isolation Risk

Credential Isolation Risk is a Stackfax risk category for Ai stacks that may expose accounts, clients, tools, workflows, private data, or production systems because credentials and sessions are shared too broadly.

The goal is to prevent one agent, workflow, browser session, tool connection, or automation from getting access to more than it needs.

⸻

Core Question

Can this stack separate accounts, clients, credentials, tools, sessions, files, memory, and workflows safely?

A stack is more dangerous when one agent can touch too many unrelated systems.

⸻

Why This Matters

Ai agents and automation tools become more dangerous when they can touch too many systems at once.

A stack may look useful, but if it has access to everything, one bad prompt, bug, config mistake, hallucinated tool call, or retry loop can create a major problem.

Credential isolation is especially important for:

* business automation
* client work
* customer data
* email access
* payment systems
* wallets or financial accounts
* production systems
* browser-based agents
* multi-client workflows
* shared workspaces
* scheduled or unattended agents

The more the agent can touch, the more isolation matters.

⸻

Common Risk Pattern

A common risky setup looks like this:

* one browser session
* one email login
* one file drive
* one set of API keys
* one agent workspace
* one memory store
* multiple workflows
* multiple clients or business functions

This can create a situation where an agent meant for one workflow can see or affect something unrelated.

Example:

An agent helping with marketing drafts should not also have access to payment tools, customer records, private files, wallets, or production systems.

⸻

What Stackfax Checks

Stackfax checks whether the stack separates:

* personal accounts
* business accounts
* client accounts
* email inboxes
* browser sessions
* API keys
* payment credentials
* file storage
* customer data
* internal documents
* memory stores
* automation tools
* production systems
* communication channels
* source control
* cloud consoles
* scheduled jobs

The check is not just:

Can the agent access the tool?

The better question is:

Should this workflow need that access at all?

⸻

High-Risk Signals

Credential Isolation Risk may be high when:

* one agent has broad access to many tools
* personal and business accounts are mixed
* multiple clients share one browser session
* customer data is available to unrelated workflows
* API keys are shared across projects
* wallets or financial tools are accessible
* agents can access credentials directly
* files are not separated by workflow
* memory is shared across unrelated tasks
* no written permission boundaries exist
* production and test environments are mixed
* agents can send messages without approval
* agents can modify records without approval
* browser profiles contain too much logged-in access

⸻

Lower-Risk Signals

Credential Isolation Risk is lower when:

* each workflow has limited permissions
* credentials are scoped to specific tasks
* client accounts are separated
* personal accounts are isolated from business accounts
* browser sessions are separated
* agents cannot directly view secrets
* sensitive data is only loaded when needed
* human approval is required before risky actions
* logs or receipts show what tools were accessed
* forbidden actions are written down
* test and production environments are separated
* access can be revoked quickly
* API keys are scoped, rotated, and not reused across unrelated workflows

⸻

Approval Gate Requirements

Human approval should be required before a stack can:

* connect credentials
* use payment tools
* access wallets
* touch financial accounts
* change account settings
* send messages
* contact customers
* edit customer records
* move or delete files
* change inventory
* process refunds
* modify production systems
* change permissions
* connect new integrations
* run scheduled external actions

Approval gates only matter if the system can show they were used.

⸻

Business Use

For business automation, credential isolation is not optional.

A business stack should avoid giving one agent broad access to:

* customer records
* CRM tools
* email accounts
* payment tools
* inventory systems
* internal files
* production systems
* client data
* accounting tools
* public posting channels
* admin settings

Strong business setups should create narrow tool access and clear approval gates.

Business rule:

One workflow should not inherit the keys to the whole company.

⸻

Client Work

For agencies or consultants, client separation is critical.

Each client should have separate:

* credentials
* browser sessions
* file access
* memory
* logs
* tool permissions
* approval rules
* deliverables
* folders
* communication channels
* run receipts

One client workflow should not be able to see another client’s data.

Client separation should exist before automation scales.

⸻

Personal Safety

Personal accounts should not be mixed with experimental agents.

Stacks should avoid giving early agents access to:

* personal email
* personal files
* photos
* messages
* password managers
* wallets
* banking
* trading accounts
* identity documents
* personal browser sessions
* personal cloud drives

Early agents should operate in a limited sandbox whenever possible.

A dedicated machine can help, but only if accounts, folders, sessions, and permissions are also separated.

⸻

Browser Session Risk

Browser-based agents are especially risky when the browser is already logged into many services.

A shared browser profile may expose:

* email
* social accounts
* payment tools
* business dashboards
* cloud consoles
* admin panels
* personal accounts
* customer records
* private files

Stackfax may flag this as:

Shared Session Risk

Safer patterns include:

* separate browser profile
* test account
* limited-permission account
* read-only access
* sandbox workspace
* no personal browser profile
* approval before any write action

⸻

API Key Risk

API keys should be scoped and separated.

Risk increases when:

* one key is reused across projects
* keys have broad permissions
* keys are stored in plain text
* keys are visible to agents
* keys are committed to repos
* keys are shared with multiple workflows
* keys have no spending limits
* keys cannot be revoked safely

Safer patterns include:

* scoped keys
* project-specific keys
* environment variables
* secret managers
* spending caps
* key rotation
* read-only keys where possible
* separate dev/test/prod keys

⸻

Memory And Credential Isolation

Memory can create credential isolation problems even when the live tool access is limited.

Risk increases when:

* private data is saved into memory
* multiple clients share one memory store
* failed runs are saved as durable truth
* credentials or secrets are copied into notes
* personal and business context mix
* old memory gets injected into unrelated workflows

Stackfax checks whether memory is:

* scoped
* inspectable
* editable
* deletable
* separated by workflow or client
* free of secrets
* safe to inject later

Core rule:

Agent memory is not agent permission.

⸻

Run Receipts

Credential isolation should be visible in the run receipt.

A useful receipt should show:

* what account was used
* what tools were touched
* what files were read
* what files were changed
* what external systems were accessed
* whether credentials were used
* whether approval was requested
* whether any sensitive data was touched
* whether action happened before or after approval

If the receipt cannot show what the agent touched, the risk is invisible.

⸻

Stackfax Verdicts

Possible verdicts include:

* Credential Isolation Needed
* Shared Session Risk
* Customer Data Risk
* Business System Risk
* Client Separation Required
* Personal Data Exposure Risk
* Approval Gates Missing
* Safe To Test With Limited Access
* Read-Only First
* Sandbox Required
* Production Access Too Broad

⸻

Common Badges

Credential isolation reviews may use badges such as:

* Credential Isolation Risk
* Human Approval Required
* Customer Data Risk
* Shared Session Risk
* Business System Risk
* Client Separation Required
* Personal Data Risk
* StackChecked
* Production Not Ready
* Run Receipts Required
* Read-Only First

⸻

What Would Improve The Score

A stack can improve by adding:

* separate browser sessions
* separate workspaces
* scoped API keys
* separate client folders
* limited file access
* tool-specific permissions
* written forbidden actions
* human approval gates
* run receipts
* logging
* sandbox test accounts
* read-only mode first
* secret manager
* key rotation
* dev/test/prod separation
* 30-day permission review

The goal is not zero access.

The goal is access that matches the job.

⸻

Example Report Language

Use language like:

This stack has Credential Isolation Risk because the agent appears to share access across unrelated accounts, files, or workflows.

Before expanding automation, separate browser sessions, scope credentials by workflow, and require approval before external or customer-facing actions.

Short version:

One agent should not get the keys to the whole building.

⸻

Stackfax Principle

One agent should not get the keys to the whole building.

Give the stack only what it needs for the job.

⸻

Final Rule

Credentials should be scoped before agents are trusted.

If one workflow does not need the key, it should not hold the key.
