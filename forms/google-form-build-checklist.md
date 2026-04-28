# Stackfax Google Form Build Checklist

This checklist turns the Stackfax report intake layout into a real Google Form.

The goal is to create one simple form that can collect early Free Mini Report and Quick Report requests without asking users for sensitive information.

## Core Goal

Build a simple Stackfax intake form that helps users describe their Ai stack, workflow, tools, and concerns.

The form should collect clarity, not secrets.

## Form Name

Stackfax Report Intake

## Form Description

Submit your Ai stack, workflow, tools, and concerns so Stackfax can prepare a report.

Do not submit passwords, API keys, payment details, wallet information, private customer data, private legal documents, private financial documents, or sensitive personal information.

Stackfax only needs a description of your stack, workflow, tools, and concerns.

## Before Building

Confirm you have:

- A Google account for Stackfax
- Access to Google Forms
- A safe place to receive responses
- A contact email
- A private folder plan for real submissions
- The intake layout file available

Reference file:

forms/report-intake-google-form-layout.md

## Recommended Settings

In Google Forms settings:

- Collect email addresses: On
- Send responders a copy of their response: Optional
- Limit to one response: Off for now
- Allow response editing: Off for now
- Show progress bar: On
- Shuffle question order: Off
- Make this a quiz: Off

## Section 1: Contact Info

Add:

### Email

Question type:

Short answer

Required:

Yes

### Name Or Handle

Question type:

Short answer

Required:

No

### Preferred Contact Method

Question type:

Multiple choice

Required:

No

Options:

- Email
- Other

## Section 2: Report Type

Add:

### Which report are you requesting?

Question type:

Multiple choice

Required:

Yes

Options:

- Free Mini Report
- Stackfax Quick Report
- Mac Mini Hardware Verdict
- Token Burn Audit
- OpenClaw Starter Stack Check
- Model Subscription Fit Check
- Business Automation Safety Check
- Vendor Stack Verdict
- Not sure

## Section 3: Main Goal

Add:

### What are you trying to build, improve, or decide with Ai?

Question type:

Paragraph

Required:

Yes

Helper text:

Example: I want to set up OpenClaw for business automation, research summaries, and customer inquiry drafts, but I am not sure if I need a Mac mini or multiple Ai subscriptions.

## Section 4: Current Stack

Add:

### What tools, models, subscriptions, hardware, agents, or platforms are you using or considering?

Question type:

Paragraph

Required:

Yes

Helper text:

Examples: ChatGPT, Claude, Gemini, OpenRouter, OpenClaw, Ollama, Mac mini, cloud server, Gmail, Google Sheets, Notion, Zapier, Make, CRM tools, agent platforms, other tools.

## Section 5: Hardware

Add:

### Are you considering buying or using dedicated hardware?

Question type:

Multiple choice

Required:

Yes

Options:

- No
- Unsure
- Mac mini
- Local Ai box
- Existing laptop or desktop
- Cloud server or VPS
- Other

Add:

### Explain your hardware situation briefly.

Question type:

Paragraph

Required:

No

## Section 6: Models And Subscriptions

Add:

### Which Ai subscriptions, APIs, model routers, or local models are you using or considering?

Question type:

Paragraph

Required:

No

Helper text:

Examples: ChatGPT Plus, Claude Pro, Gemini, OpenRouter, API credits, Ollama, local models, business Ai tools.

## Section 7: Workflow

Add:

### Describe the workflow you want the stack to support.

Question type:

Paragraph

Required:

Yes

Helper text:

What should happen from start to finish?

Example: Research a topic, summarize findings, draft a report, flag risks, and ask for approval before saving or sending anything.

## Section 8: Cost Concern

Add:

### What are you most worried about spending money on?

Question type:

Checkboxes

Required:

No

Options:

- Hardware
- Model subscriptions
- API/token costs
- Cloud hosting
- Tools/apps
- Setup help
- Maintenance
- I am not sure yet
- Other

## Section 9: Risk Concern

Add:

### What are you most worried about breaking, exposing, or over-automating?

Question type:

Checkboxes

Required:

No

Options:

- Personal files
- Customer data
- Business data
- Email accounts
- Credentials
- Wallets or financial accounts
- Public posting
- Inventory
- Payments
- Production systems
- I am not sure yet
- Other

## Section 10: Automation Level

Add:

### What should the Ai stack be allowed to do right now?

Question type:

Multiple choice

Required:

Yes

Options:

- Observe only
- Summarize and report
- Draft but not send
- Take action only after approval
- Take some narrow actions automatically
- I am not sure yet

## Section 11: Approval Gates

Add:

### What actions should require human approval?

Question type:

Checkboxes

Required:

No

Options:

- Sending messages
- Posting publicly
- Contacting customers
- Moving or deleting files
- Changing settings
- Connecting credentials
- Accessing wallets or financial accounts
- Editing customer records
- Changing inventory
- Processing payments
- Modifying production systems
- Other

## Section 12: Local vs Cloud

Add:

### Which setup do you prefer right now?

Question type:

Multiple choice

Required:

No

Options:

- Cloud-first
- Local-first
- Hybrid
- Unsure
- I only care what fits the task

Add:

### Explain your local vs cloud preference briefly.

Question type:

Paragraph

Required:

No

## Section 13: Current Friction

Add:

### What feels most confusing right now?

Question type:

Checkboxes

Required:

No

Options:

- I do not know what stack I need
- I do not know if I need hardware
- I do not know which model to use
- I do not know which subscriptions I need
- I do not know why tokens cost so much
- I do not know what OpenClaw should be allowed to touch
- I do not know how to scale this safely
- I do not know where to start
- Other

## Section 14: Links Or Public References

Add:

### Optional public links

Question type:

Paragraph

Required:

No

Helper text:

Paste any public links, videos, docs, GitHub repos, product pages, creator stacks, or vendor stacks you want reviewed.

Do not include private links or private files unless specifically approved later.

## Section 15: Desired Output

Add:

### What do you want from the report?

Question type:

Checkboxes

Required:

No

Options:

- Buy / do not buy hardware verdict
- Token burn explanation
- Subscription simplification
- OpenClaw setup advice
- Approval gate warnings
- Business automation safety review
- Vendor stack review
- Best next move
- 30-day recheck plan
- I am not sure yet
- Other

## Section 16: Safety Confirmation

Add:

### Safety confirmation

Question type:

Checkboxes

Required:

Yes

Required option:

- I understand that I should not submit passwords, API keys, payment details, private credentials, wallet information, private customer data, or sensitive private information.

## Section 17: Final Confirmation

Add:

### Final confirmation

Question type:

Checkboxes

Required:

Yes

Required option:

- I understand that Stackfax is early, reports may be manual, and Stackfax gives stack guidance, not guaranteed business, financial, legal, trading, security, or technical outcomes.

## Confirmation Message

Set the form confirmation message to:

Thanks for submitting your Stackfax intake.

Your stack details have been received.

If this is a paid Quick Report, Stackfax will review the intake and may follow up if more context is needed.

Expected delivery target for accepted Quick Reports:

24 to 48 hours.

## Test Before Sharing

Submit one test response.

Check:

- Response is received
- Email is captured
- Required questions work
- Safety confirmation works
- Long answers are readable
- The form does not ask for secrets
- The confirmation message is clear

## Link Handling

Before sharing publicly:

- Copy the public form link
- Save it in a private note
- Add it to Gumroad later
- Add it to future soft launch posts only when ready

## Final Rule

Simple beats fancy.

One safe intake form is better than five confusing forms.
