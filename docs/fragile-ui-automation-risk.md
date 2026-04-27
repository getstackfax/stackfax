# Fragile UI Automation Risk

Fragile UI Automation Risk is a Stackfax risk category for Ai stacks that depend too heavily on screens, clicks, screenshots, browser layouts, or unstable app interfaces.

The goal is to identify workflows that may break when a website, app, button, page layout, modal, menu, or visual element changes.

## Core Question

Does this stack rely on fragile screen-based automation when it should use APIs, structured data, stable integrations, or human approval?

## Why This Matters

Ai agents can often use browsers, screenshots, and click-based workflows.

That can be useful for testing and exploration, but it can become fragile in real operations.

A workflow that works once may fail when:

- A button moves
- A site changes layout
- A login screen appears
- A pop-up blocks the page
- A field label changes
- A browser session expires
- A captcha appears
- A tool loads slowly
- A menu collapses
- A page returns different results

Fragile UI automation is especially risky when the stack touches customer data, payments, messages, inventory, production systems, or public posting tools.

## What Stackfax Checks

Stackfax checks whether the workflow depends on:

- Screenshots
- Browser clicks
- Visual layout recognition
- Changing web pages
- Unstable app interfaces
- Manual UI paths
- Pop-ups or modals
- Browser sessions
- Hidden menus
- Copy/paste loops
- Repeated tool loops
- Websites without stable APIs

## High-Risk Signals

Fragile UI Automation Risk may be high when:

- The agent must click through many pages
- The workflow depends on a specific page layout
- The stack has no API fallback
- The agent reads data from screenshots only
- The user does not know what the agent clicked
- The workflow has no confirmation step
- The agent acts inside customer-facing tools
- The agent changes settings, records, files, or payments through a UI
- The workflow breaks if a modal, pop-up, or login screen appears
- There are no logs of what happened

## Lower-Risk Signals

Fragile UI Automation Risk is lower when:

- The workflow uses APIs where possible
- The stack uses structured data
- The agent only observes and reports
- Human approval is required before actions
- The workflow is simple and repeatable
- Errors are logged
- The stack has clear stopping rules
- The user can review before anything is sent, changed, posted, or deleted
- Browser actions are limited to low-risk tasks

## Better Alternatives

When possible, use:

- APIs
- Webhooks
- CSV exports
- Structured data
- Spreadsheets
- Database queries
- Official integrations
- Stable automation platforms
- Manual review checkpoints

Ui automation can still be useful, but it should not be the only control layer for important business actions.

## Approval Gate Requirements

Human approval should be required before UI automation can:

- Send messages
- Submit forms
- Contact customers
- Post publicly
- Change customer records
- Move or delete files
- Change account settings
- Process payments
- Issue refunds
- Change inventory
- Modify production systems

## Tool Loop Risk

Fragile UI automation can create tool loops.

A tool loop happens when an agent repeatedly clicks, searches, refreshes, retries, or navigates without reaching a clear stopping point.

Warning signs:

- Repeated browser actions
- Repeated searches
- Repeated failed clicks
- Long task chains
- No max step count
- No max tool-call count
- No stop condition
- No human checkpoint

Stackfax may recommend:

- Max tool-call limits
- Max step limits
- Stop conditions
- Human approval before retrying
- Logs of browser actions
- API replacement where possible

## Business Use

For business automation, fragile UI workflows should start as low-risk tests.

Good first uses:

- Reading public information
- Summarizing visible data
- Drafting internal notes
- Preparing reports
- Flagging issues

Bad first uses:

- Sending customer messages
- Changing CRM records
- Updating inventory
- Processing payments
- Issuing refunds
- Changing account settings
- Posting publicly

## OpenClaw And Agent Use

OpenClaw-style stacks may use browser tools, screenshots, and click paths.

That can be useful for learning and experimentation.

But the first workflow should usually:

- Observe
- Summarize
- Report
- Draft with approval

It should not immediately automate high-risk UI actions.

## Stackfax Verdicts

Possible verdicts include:

- Fragile UI Automation Risk
- API Preferred
- Human Approval Required
- Tool Loop Risk
- Production Not Ready
- Safe To Test With Limited Access
- Observe Only
- Draft With Approval

## Common Badges

Fragile UI automation reviews may use badges such as:

- Fragile UI Automation Risk
- Human Approval Required
- Tool Loop Burn
- Production Not Ready
- API Preferred
- StackChecked
- Business System Risk
- Customer Data Risk

## What Would Improve The Score

A stack can improve by adding:

- API-first workflow
- Structured data sources
- Tool-call limits
- Step limits
- Stop conditions
- Browser action logs
- Human review checkpoints
- Low-risk testing first
- Fallback plan
- 30-day reliability review

## Stackfax Principle

If a workflow breaks because a button moved, it is not production-ready.

Use UI automation carefully.

Use APIs and structured data when the task matters.
