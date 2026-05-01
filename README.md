# Stackfax

**The first report card for Ai stacks.**

Stackfax helps builders, small businesses, and Ai-agent users understand what their setup actually needs before they buy more tools, burn tokens, copy a random agent setup, or overbuild local hardware.

The goal is simple:

**Turn tool confusion into a clear next-step map.**

---

## What is an Ai stack?

An Ai stack is the combination of tools used to get Ai-assisted work done.

That can include:

- models
- providers
- subscriptions
- agents
- memory
- hosting
- hardware
- permissions
- workflows
- communication channels
- approval gates

Most people do not need one giant expensive model, one perfect machine, or every subscription at once.

They need the right stack for the job.

---

## What Stackfax checks

Stackfax reviews an Ai stack across practical risk and fit categories:

| Category | What it checks |
|---|---|
| Cost / token burn | Whether premium models are being used for low-value or repetitive work |
| Model / provider fit | Whether the chosen models match the actual workload |
| Hardware verdict | Whether local hardware is justified, overbuilt, or unnecessary |
| Workflow reliability | Whether the setup can repeat the same task without constant babysitting |
| Memory / state | Whether important context is saved, retrieved, and trusted correctly |
| Permissions / secrets | Whether tools, files, keys, accounts, and private data are protected |
| Approval gates | Whether humans approve risky actions before they happen |
| Automation fit | Whether the task should be automated, drafted, monitored, or kept manual |
| Upgrade path | The next safest improvement instead of random tool chasing |

---

## Common Stackfax questions

Stackfax helps answer questions like:

- What stack do I actually need?
- Do I need a Mac mini, Mac Studio, GPU box, cloud server, or nothing yet?
- Am I paying for overlapping model subscriptions?
- Am I burning premium tokens on cheap tasks?
- Should this be an agent, a simple automation, or a manual workflow?
- Where are the risk points before I connect this to customers, files, email, money, or private data?
- What should I improve next?

---

## Example verdicts

A Stackfax report may include verdicts like:

- **Cloud-first**
- **Local-ready**
- **Hardware overkill warning**
- **Human approval required**
- **Token burn risk**
- **Provider routing risk**
- **Memory/state risk**
- **Workflow reliability gap**
- **Permissions/secrets risk**

The report is not just a tool list.

It is a practical map of what fits, what is risky, what is overbuilt, and what to do next.

---

## Example reports

This repo includes early sample reports showing how Stackfax turns a messy setup into a clear verdict:

- [Business Automation Starter Stack](reports/sample-business-automation-stack.md)
- [Noob OpenClaw Starter Stack](reports/sample-noob-openclaw-starter-stack.md)

These are early examples of the report style: practical, direct, risk-aware, and focused on the next safest step.

---

## Current repo structure

```text
docs/
  badge-definitions.md
  rating-system.md

examples/
  business-automation-input.json

reports/
  sample-business-automation-stack.md
  sample-noob-openclaw-starter-stack.md

schema/
  stackfax-report-v0.1.json
Current status

Stackfax is in an early manual-report phase.

The current focus is:

* defining the Stackfax report format
* building sample reports
* documenting rating categories
* identifying common Ai-stack failure patterns
* testing small manual reports before automating the system

Early reports may be created manually before the product becomes more automated.

⸻

Core rule

Clarity before you build.

Before buying hardware, stacking subscriptions, giving an agent permissions, or wiring Ai into a business workflow, map the stack first.

Stackfax exists to answer:

What should this setup actually do, what can go wrong, and what is the next safest step?
