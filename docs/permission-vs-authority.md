# Stackfax Permission Versus Authority

Permission Versus Authority is the Stackfax doctrine for separating what an Ai agent technically can do from what it should be allowed to do.

The goal is to prevent users from mistaking capability, access, or tool availability for safe authority.

⸻

Core Idea

An agent being able to do something does not mean it should be allowed to do it.

Capability is technical.

Authority is operational.

Permission is the boundary between them.

Core rule:

Capability is not authority.

⸻

Core Question

Does this stack clearly define what the agent can do, what it may do, what requires approval, and what is forbidden?

If not, the stack has permission risk.

⸻

Why This Matters

Modern Ai agents can touch more than text.

They may be able to:

* read files
* write files
* run commands
* browse websites
* send messages
* post publicly
* access email
* update spreadsheets
* call APIs
* touch CRM records
* trigger automations
* use credentials
* modify settings
* interact with payment tools
* access production systems

That does not mean they should.

Stackfax verdict:

Tool access without authority rules creates invisible risk.

⸻

Capability

Capability means what the stack can technically do.

Examples:

* the model can reason
* the browser tool can click
* the shell can run commands
* the email tool can send
* the API key can write records
* the file tool can delete
* the CRM integration can update customers
* the payment tool can issue refunds

Capability describes the possible action.

It does not decide whether the action is allowed.

⸻

Permission

Permission means what the system allows the agent to access or execute.

Examples:

* read-only file access
* draft-only email access
* limited browser profile
* scoped API key
* test workspace only
* no public posting
* no customer contact
* no payments
* no production changes

Permission should be narrower than capability.

A safe stack does not expose every capability just because it exists.

⸻

Authority

Authority means what the agent is trusted to do on behalf of the user, business, or workflow.

Authority depends on:

* role
* workflow
* risk level
* approval state
* data sensitivity
* business policy
* user intent
* legal/compliance context
* rollback ability
* evidence layer

Authority should be earned through tested workflows, receipts, and human approval.

⸻

Approval

Approval is the explicit human decision that allows a risky action to happen.

Human approval should be required before Ai can:

* send messages
* contact customers
* post publicly
* move or delete files
* edit customer records
* connect credentials
* process payments
* issue refunds
* change inventory
* modify production systems
* change account settings
* trigger external workflows

Approval should be recorded.

Core rule:

Human approval is only real if the receipt shows what was approved.

⸻

Forbidden Actions

A strong stack should define what the agent must never do.

Examples:

* reveal credentials
* access wallets
* trade automatically
* send customer messages without approval
* delete files without approval
* post publicly without approval
* change production systems without approval
* use private data outside the approved workflow
* contact people from the wrong account
* mix client data
* bypass cost caps
* ignore uncertainty

Forbidden actions should be written down.

Do not rely on vibes.

⸻

Prompt Rules Are Not Enough

A prompt can say:

Do not send messages without approval.

That is good.

But it is not enough.

The tool layer should also limit the agent when possible.

Safer controls include:

* read-only mode
* draft-only mode
* scoped API keys
* separate test account
* separate browser profile
* disabled send/post permissions
* tool-call limits
* approval gate before action
* run receipts
* sandbox environment

Stackfax principle:

A prompt is not a cage.

Prompts guide behavior.

Permissions limit blast radius.

⸻

Permission Boundary Examples

Read-Only

The agent can observe, summarize, or report.

Allowed:

* read approved files
* summarize public pages
* inspect non-sensitive data
* draft notes
* flag issues

Not allowed:

* write
* send
* delete
* post
* purchase
* modify records

Best for:

* early testing
* research
* low-risk workflows
* first agent runs

⸻

Draft-Only

The agent can prepare outputs but cannot execute them.

Allowed:

* draft emails
* draft posts
* draft reports
* suggest replies
* prepare checklists
* recommend next actions

Not allowed:

* send
* publish
* modify customer records
* trigger external workflows

Best for:

* customer support drafts
* outreach drafts
* content creation
* business review workflows

⸻

Approved Action

The agent can act only after human approval.

Allowed:

* take a narrow action after explicit approval
* update a specific record
* send an approved draft
* run a bounded command
* submit an approved form

Requires:

* approval record
* action receipt
* rollback or correction path
* scope limit

Best for:

* limited business automation
* controlled workflows
* repeatable low-risk actions

⸻

Narrow Autonomy

The agent can take limited actions without approval inside a tightly defined boundary.

Allowed only when:

* workflow is proven
* risk is low
* permissions are narrow
* actions are reversible or low impact
* logs and receipts exist
* failure path exists
* cost caps exist
* owner accountability exists

Best for:

* internal routing
* non-sensitive tagging
* low-risk classification
* scheduled summaries
* safe housekeeping

Most early stacks should not start here.

⸻

Broad Autonomy

The agent can act across tools, accounts, customers, files, or systems.

This is high risk.

Broad autonomy requires:

* strong governance
* credential isolation
* approval policy
* receipts
* monitoring
* rollback
* owner accountability
* production readiness review
* security/compliance review where relevant

Most Stackfax verdicts should treat broad autonomy as not ready until proven.

⸻

Common Permission Mistakes

Tool Exists, So Agent Uses It

The stack exposes a tool and assumes the agent should decide when to use it.

Risk:

* unnecessary tool calls
* wrong action
* data exposure
* token burn
* side effects

Verdict:

Tool access should follow workflow need.

⸻

One Agent Gets Everything

The agent has access to all files, tools, accounts, channels, and credentials.

Risk:

* large blast radius
* client data mixing
* personal/business mixing
* accidental changes
* hard-to-audit actions

Verdict:

One agent should not get the keys to the whole building.

⸻

Approval Only In Chat

The user says “ask first,” but the system does not enforce or record approval.

Risk:

* approval gets skipped
* approval is ambiguous
* no evidence exists
* action happens before review

Verdict:

Approval should be a workflow state, not just a sentence in a prompt.

⸻

Permission Creep

The agent slowly gains more access over time without review.

Risk:

* old permissions stay active
* new tools expand blast radius
* no one remembers what the agent can touch
* production access appears accidentally

Verdict:

Permission should expand slower than capability.

⸻

Wrong Role Authority

An agent role is given authority outside its purpose.

Example:

* research agent can send email
* drafting agent can modify CRM
* scout agent can post publicly
* support summarizer can issue refunds
* coding agent can deploy production changes

Verdict:

Role should define authority, not just personality.

⸻

Permission And Communication Channels

Communication channels are authority surfaces.

If an agent can speak through a channel, it may affect real people.

Stackfax checks whether the agent can:

* DM users
* reply to customers
* send email
* post publicly
* speak from a brand account
* access private threads
* trigger workflows from messages

Core rule:

The channel is part of the stack.

⸻

Permission And Customer Data

Customer data raises authority requirements.

If the agent can access customer data, Stackfax checks:

* what data it can see
* why it needs the data
* whether access is scoped
* whether data enters memory
* whether output is reviewed
* whether customer-facing actions require approval
* whether receipts show data access

Customer data is not generic context.

⸻

Permission And Credentials

Credentials should be scoped before agents are trusted.

Stackfax checks:

* Can the agent view secrets?
* Can it use API keys?
* Are keys scoped?
* Are credentials shared across workflows?
* Can credentials be revoked?
* Are dev/test/prod keys separated?
* Are credentials stored safely?

Core rule:

If one workflow does not need the key, it should not hold the key.

⸻

Permission And Memory

Memory is not authority.

An agent may remember that a customer exists.

That does not mean it may contact the customer.

An agent may know a file path.

That does not mean it may edit the file.

An agent may know a business rule.

That does not mean it may execute the rule without approval.

Stackfax principle:

Agent memory is not agent permission.

⸻

Permission And Agent ROI

Agent ROI should subtract permission risk.

An agent may appear productive, but ROI drops if it:

* touches too much
* requires too much review
* creates unsafe side effects
* uses broad credentials
* acts outside approval gates
* creates cleanup work
* cannot prove what it did

Useful work must be counted after permission risk.

⸻

Permission Verdicts

Possible verdicts include:

* Permission Boundary Needed
* Capability Exceeds Authority
* Approval Gates Missing
* Read-Only First
* Draft-Only Required
* Narrow Permissions Recommended
* Broad Access Too Early
* Credential Isolation Needed
* Human Approval Required
* Safe To Test With Limited Access
* Production Not Ready

⸻

Common Risk Flags

Permission reviews may include:

* Permission Boundary Needed
* Approval Gates Missing
* Credential Isolation Risk
* Customer Data Risk
* Communication Channel Risk
* Fragile UI Automation Risk
* Business System Risk
* Personal Data Risk
* Production Not Ready
* Run Receipts Required
* Agent ROI Unclear

⸻

What Would Improve The Score

A stack can improve permission safety by adding:

* role-based permissions
* read-only mode first
* draft-only mode
* scoped API keys
* separate browser profiles
* test accounts
* forbidden action list
* approval gates
* run receipts
* tool-call limits
* channel restrictions
* customer-data boundaries
* dev/test/prod separation
* 30-day permission review

The goal is not zero capability.

The goal is authority that matches the job.

⸻

Example Report Language

Use language like:

This stack has Permission Boundary Risk because the agent appears technically capable of taking actions that have not been approved by the workflow.

Before expanding automation, separate read-only, draft-only, approved-action, and forbidden actions. Add scoped permissions and receipts before giving the agent write access.

Short version:

Capability is not authority.

⸻

Stackfax Principle

Capability is not authority.

A prompt is not a cage.

Permission should expand slower than capability.

⸻

Final Rule

Do not give an agent authority just because the tool exists.

Define what it can see, what it can prepare, what it can do only after approval, and what it must never touch.

