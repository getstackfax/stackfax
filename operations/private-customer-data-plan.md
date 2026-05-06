Stackfax Private Customer Data Plan

This file defines how Stackfax should handle private customer data before accepting real report requests.

The goal is to protect users, protect the business, and avoid collecting sensitive information that Stackfax does not need.

Stackfax is a trust product.

Trust starts with data restraint.

⸻

Core Rule

Do not collect sensitive data unless it is truly needed.

For early Stackfax reports, most sensitive data is not needed.

Stackfax needs the user’s stack description, workflow, tools, concerns, and goals.

Stackfax does not need passwords, API keys, payment details, wallets, private customer records, private legal documents, private medical documents, or private financial documents.

Core principle:

Collect the stack problem, not the user’s private life.

⸻

What Stackfax Should Collect

For early reports, Stackfax may collect:

* name or handle
* email
* main goal
* current Ai stack
* tools being used
* subscriptions being considered
* hardware being considered
* workflow description
* cost concerns
* risk concerns
* approval gate concerns
* run receipt or logging concerns
* public links the user wants reviewed
* optional non-sensitive screenshots if approved later

Only collect information that helps produce the report.

⸻

What Stackfax Should Not Collect

Stackfax should not collect:

* passwords
* API keys
* recovery codes
* payment card details
* bank information
* wallet seed phrases
* private keys
* trading account details
* private customer records
* private legal documents
* private medical documents
* private financial documents
* identity documents
* employee records
* client confidential files
* sensitive personal information
* private messages
* private inbox exports
* password manager exports
* production credentials
* source code secrets

If the report can be completed without the data, do not collect the data.

⸻

If A User Submits Sensitive Data

If a user submits sensitive information:

1. Do not use it.
2. Do not copy it into a report.
3. Do not store it in the public repo.
4. Ask the user to remove it.
5. Request a cleaned-up version of the intake.
6. Continue only after the intake is safe.

Suggested response:

Thanks for sending this. Please remove any passwords, API keys, private customer records, payment details, wallet information, or sensitive documents before we review the stack. Stackfax only needs the setup, workflow, tools, risks, and goals.

⸻

Public Repo Rule

Never put real customer data in the public GitHub repo.

The public repo may include:

* blank templates
* sample reports
* fictional examples
* fake scenarios clearly labeled as examples
* general lessons
* public field research patterns
* anonymized product insights
* public doctrine

The public repo should not include:

* real customer names
* real customer emails
* real customer reports
* real business data
* private submissions
* private screenshots
* payment information
* support messages
* internal customer notes
* credentials
* private files
* unapproved testimonials

Public examples should be fictional, anonymized, or explicitly approved.

⸻

Private Storage Rule

Real customer submissions and reports should be stored outside the public repo.

Possible private storage options later:

* private Google Drive folder
* private Notion workspace
* private Airtable
* private CRM
* private encrypted folder
* private database later

Early recommendation:

Use a private folder with simple naming and no public sharing.

Do not store private customer files in the Stackfax public repo.

⸻

Naming Convention

Suggested private naming format:

* date
* report type
* customer handle or initials
* status

Example:

2026-04-27_quick-report_stackbuilder01_delivered

Avoid putting sensitive details in file names.

Do not include:

* customer secrets
* legal issues
* health details
* payment details
* private business disputes
* confidential project names unless approved

⸻

Access Rule

Only approved people should access real customer data.

Early Stackfax access should be limited to the owner/operator.

If helpers, contractors, agents, or tools are added later, they should only access what they need.

Access should follow the minimum necessary rule:

Give each person or system the least data needed to do the job.

⸻

Agent Rule

Ai agents should not access real customer data by default.

Before an agent can touch real customer submissions, Stackfax should have:

* explicit user permission
* clear purpose
* limited access
* no credential access
* no payment access
* no unnecessary private data
* human review before delivery
* logging of what the agent accessed
* clear deletion or retention plan

Agents may help with sanitized summaries, templates, and fictional examples.

Agents should not freely browse private customer folders.

⸻

Data Boundary Rule

Stackfax should separate data into clear boundaries.

Public

Examples:

* public Reddit threads
* public GitHub repos
* public product docs
* public websites
* public pricing pages
* public vendor announcements

Customer-Provided Non-Sensitive

Examples:

* stack description
* tools used
* workflow goals
* general cost concerns
* public links
* non-sensitive screenshots

Customer-Provided Sensitive

Examples:

* customer records
* legal files
* payment details
* credentials
* private messages
* business financials
* employee records
* client files

Default rule:

Public and non-sensitive stack information can be used for reports.

Sensitive customer information should be avoided unless a future paid workflow explicitly requires it and has stronger controls.

⸻

Email Rule

Customer email should be used only for:

* intake confirmation
* follow-up questions
* report delivery
* optional feedback
* relevant report updates

Do not spam.

Do not sell emails.

Do not add users to a mailing list without clear consent.

If a newsletter or update list is added later, it should require clear opt-in.

⸻

Payment Data Rule

Payment details should be handled by the payment provider, not Stackfax.

Stackfax should not store:

* credit card numbers
* bank details
* payment credentials
* full payment account data
* wallet private keys
* seed phrases

Use payment tools like Gumroad, Stripe, PayPal, Ko-fi, or similar to handle payment details.

Stackfax may store basic payment status only when needed, such as:

* paid
* unpaid
* refunded
* delivered
* pending

⸻

Report Sharing Rule

Do not share a real customer report publicly unless the user gives clear permission.

If a report is reused as an example:

* remove identifying information
* remove private details
* label it clearly
* get permission when needed
* consider rewriting it as a fictionalized sample
* avoid implying endorsement without permission

Default rule:

Customer reports are private.

Public samples should be fictional unless explicitly approved.

⸻

Feedback Rule

Feedback can be useful, but it should be handled carefully.

Use feedback to improve:

* intake questions
* report templates
* scoring clarity
* risk flags
* offer copy
* delivery workflow
* report structure

Do not turn feedback into a testimonial unless the user gives permission.

If a testimonial is used, confirm:

* what name or handle can be shown
* whether the company name can be shown
* whether the quote can be edited for clarity
* whether the report type can be referenced

⸻

Retention Rule

Stackfax should eventually define how long customer submissions and reports are kept.

Early recommendation:

Keep only what is needed to deliver the report and improve the product.

Delete or archive unnecessary sensitive information.

If a user requests deletion of their private intake or report, Stackfax should honor the request when possible.

Default principle:

Keep the minimum useful record. Remove unnecessary sensitive data.

⸻

Red Flags

Pause or refuse work if the request requires:

* accessing passwords
* accessing API keys
* accessing wallets
* accessing financial accounts
* reviewing private legal documents
* handling customer records directly
* processing sensitive medical data
* processing identity documents
* unsafe automation instructions
* misleading or fraudulent use
* evading platform rules
* bypassing security controls
* automating harmful actions
* making legal, medical, financial, or compliance claims without proper review

Stackfax can review the stack shape without touching unsafe private material.

⸻

Early Report Safe Intake Standard

A safe early Stackfax intake should answer:

* What are you trying to build or improve?
* What tools, models, subscriptions, agents, or hardware are you using?
* What workflow are you trying to run?
* What feels expensive, risky, confusing, or overbuilt?
* What should the system be allowed to do?
* What should require human approval?
* What public links or non-sensitive screenshots help explain the setup?
* What decision do you need the report to help with?

A safe intake should not include secrets, credentials, customer records, or sensitive documents.

⸻

Private / Public Boundary

Stackfax should keep a clear boundary between public doctrine and private customer work.

Public Map

Can include:

* general risk categories
* sample report templates
* fictional examples
* educational guides
* public field research patterns
* product doctrine
* community rules
* public-facing verdict language

Private Engine

Should protect:

* customer submissions
* paid report drafts
* scoring interpretation
* report generation prompts
* customer communications
* pricing or fulfillment notes
* internal lead flow
* private delivery workflow

Core rule:

Open the map. Protect the engine.

⸻

Final Rule

Protect the user before improving the product.

Trust is the asset.

Do not collect what you do not need.

Source verdict …

Project source it.

This is core trust doctrine for paid reports, intake forms, private folders, and future customer handling.
