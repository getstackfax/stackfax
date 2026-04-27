# Credential Isolation Risk

Credential Isolation Risk is a Stackfax risk category for Ai stacks that may expose accounts, clients, tools, workflows, or private data because credentials are shared too broadly.

The goal is to prevent one agent, workflow, browser session, or tool connection from getting access to more than it needs.

## Core Question

Can this stack separate accounts, clients, credentials, tools, sessions, files, and workflows safely?

## Why This Matters

Ai agents and automation tools become more dangerous when they can touch too many systems at once.

A stack may look useful, but if it has access to everything, one bad prompt, bug, config mistake, or tool loop can create a major problem.

Credential isolation is especially important for:

- Business automation
- Client work
- Customer data
- Email access
- Payment systems
- Wallets or financial accounts
- Production systems
- Browser-based agents
- Multi-client workflows
- Shared workspaces

## Common Risk Pattern

A common risky setup looks like this:

- One browser session
- One email login
- One file drive
- One set of API keys
- One agent workspace
- Multiple workflows
- Multiple clients or business functions

This can create a situation where an agent meant for one workflow can see or affect something unrelated.

## What Stackfax Checks

Stackfax checks whether the stack separates:

- Personal accounts
- Business accounts
- Client accounts
- Email inboxes
- Browser sessions
- API keys
- Payment credentials
- File storage
- Customer data
- Internal documents
- Memory stores
- Automation tools
- Production systems

## High-Risk Signals

Credential Isolation Risk may be high when:

- One agent has broad access to many tools
- Personal and business accounts are mixed
- Multiple clients share one browser session
- Customer data is available to unrelated workflows
- API keys are shared across projects
- Wallets or financial tools are accessible
- Agents can access credentials directly
- Files are not separated by workflow
- Memory is shared across unrelated tasks
- No written permission boundaries exist

## Lower-Risk Signals

Credential Isolation Risk is lower when:

- Each workflow has limited permissions
- Credentials are scoped to specific tasks
- Client accounts are separated
- Personal accounts are isolated from business accounts
- Browser sessions are separated
- Agents cannot directly view secrets
- Sensitive data is only loaded when needed
- Human approval is required before risky actions
- Logs show what tools were accessed
- Forbidden actions are written down

## Approval Gate Requirements

Human approval should be required before a stack can:

- Connect credentials
- Use payment tools
- Access wallets
- Touch financial accounts
- Change account settings
- Send messages
- Contact customers
- Edit customer records
- Move or delete files
- Change inventory
- Process refunds
- Modify production systems

## Business Use

For business automation, credential isolation is not optional.

A business stack should avoid giving one agent broad access to:

- Customer records
- CRM tools
- Email accounts
- Payment tools
- Inventory systems
- Internal files
- Production systems
- Client data

Strong business setups should create narrow tool access and clear approval gates.

## Client Work

For agencies or consultants, client separation is critical.

Each client should have separate:

- Credentials
- Browser sessions
- File access
- Memory
- Logs
- Tool permissions
- Approval rules
- Deliverables

One client workflow should not be able to see another client’s data.

## Personal Safety

Personal accounts should not be mixed with experimental agents.

Stacks should avoid giving early agents access to:

- Personal email
- Personal files
- Photos
- Messages
- Password managers
- Wallets
- Banking
- Trading accounts
- Identity documents

Early agents should operate in a limited sandbox whenever possible.

## Stackfax Verdicts

Possible verdicts include:

- Credential Isolation Needed
- Shared Session Risk
- Customer Data Risk
- Business System Risk
- Client Separation Required
- Personal Data Exposure Risk
- Approval Gates Missing
- Safe To Test With Limited Access

## Common Badges

Credential isolation reviews may use badges such as:

- Credential Isolation Risk
- Human Approval Required
- Customer Data Risk
- Shared Session Risk
- Business System Risk
- Client Separation Required
- Personal Data Risk
- StackChecked

## What Would Improve The Score

A stack can improve by adding:

- Separate browser sessions
- Separate workspaces
- Scoped API keys
- Separate client folders
- Limited file access
- Tool-specific permissions
- Written forbidden actions
- Human approval gates
- Logging
- 30-day permission review

## Stackfax Principle

One agent should not get the keys to the whole building.

Give the stack only what it needs for the job.
