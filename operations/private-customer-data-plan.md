# Stackfax Private Customer Data Plan

This file defines how Stackfax should think about private customer data before accepting real report requests.

The goal is to protect users, protect the business, and avoid collecting sensitive information that Stackfax does not need.

## Core Rule

Do not collect sensitive data unless it is truly needed.

For early Stackfax reports, most sensitive data is not needed.

Stackfax needs the user’s stack description, workflow, tools, concerns, and goals.

Stackfax does not need passwords, API keys, payment details, wallets, private customer records, or private legal/financial documents.

## What Stackfax Should Collect

For early reports, Stackfax may collect:

- Name or handle
- Email
- Main goal
- Current Ai stack
- Tools being used
- Subscriptions being considered
- Hardware being considered
- Workflow description
- Cost concerns
- Risk concerns
- Approval gate concerns
- Public links the user wants reviewed
- Optional non-sensitive screenshots if approved later

## What Stackfax Should Not Collect

Stackfax should not collect:

- Passwords
- API keys
- Recovery codes
- Payment card details
- Bank information
- Wallet seed phrases
- Private keys
- Trading account details
- Private customer records
- Private legal documents
- Private medical documents
- Private financial documents
- Identity documents
- Employee records
- Client confidential files
- Sensitive personal information

## If A User Submits Sensitive Data

If a user submits sensitive information:

1. Do not use it.
2. Do not copy it into a report.
3. Do not store it in the public repo.
4. Ask the user to remove it.
5. Request a cleaned-up version of the intake.
6. Continue only after the intake is safe.

## Public Repo Rule

Never put real customer data in the public GitHub repo.

The public repo may include:

- Blank templates
- Sample reports
- Fake scenarios clearly labeled as examples
- General lessons
- Public field research patterns
- Anonymized product insights

The public repo should not include:

- Real customer names
- Real customer emails
- Real customer reports
- Real business data
- Private submissions
- Private screenshots
- Payment information
- Support messages
- Internal customer notes

## Private Storage Rule

Real customer submissions and reports should be stored outside the public repo.

Possible private storage options later:

- Private Google Drive folder
- Private Notion workspace
- Private Airtable
- Private CRM
- Private encrypted folder
- Private database later

Early recommendation:

Use a private folder with simple naming and no public sharing.

## Naming Convention

Suggested private naming format:

- Date
- Report type
- Customer handle or initials
- Status

Example:

2026-04-27_quick-report_stackbuilder01_delivered

Avoid putting sensitive details in file names.

## Access Rule

Only approved people should access real customer data.

Early Stackfax access should be limited to the owner/operator.

If helpers, contractors, agents, or tools are added later, they should only access what they need.

## Agent Rule

Ai agents should not access real customer data by default.

Before an agent can touch real customer submissions, Stackfax should have:

- Explicit user permission
- Clear purpose
- Limited access
- No credential access
- No payment access
- No unnecessary private data
- Human review before delivery

## Email Rule

Customer email should be used only for:

- Intake confirmation
- Follow-up questions
- Report delivery
- Optional feedback
- Relevant report updates

Do not spam.

Do not sell emails.

Do not add users to a mailing list without clear consent.

## Payment Data Rule

Payment details should be handled by the payment provider, not Stackfax.

Stackfax should not store:

- Credit card numbers
- Bank details
- Payment credentials
- Full payment account data

Use payment tools like Gumroad, Stripe, PayPal, Ko-fi, or similar to handle payment details.

## Report Sharing Rule

Do not share a real customer report publicly unless the user gives clear permission.

If a report is reused as an example:

- Remove identifying information
- Remove private details
- Label it clearly
- Get permission when needed
- Consider rewriting as a fictionalized sample

## Feedback Rule

Feedback can be useful, but it should be handled carefully.

Use feedback to improve:

- Intake questions
- Report templates
- Scoring clarity
- Risk flags
- Offer copy
- Delivery workflow

Do not turn feedback into a testimonial unless the user gives permission.

## Retention Rule

Stackfax should eventually define how long customer submissions and reports are kept.

Early recommendation:

Keep only what is needed to deliver the report and improve the product.

Delete or archive unnecessary sensitive information.

## Red Flags

Pause or refuse work if the request requires:

- Accessing passwords
- Accessing API keys
- Accessing wallets
- Accessing financial accounts
- Reviewing private legal documents
- Handling customer records directly
- Processing sensitive medical data
- Processing identity documents
- Unsafe automation instructions
- Misleading or fraudulent use

## Final Rule

Protect the user before improving the product.

Trust is the asset.

Do not collect what you do not need.
