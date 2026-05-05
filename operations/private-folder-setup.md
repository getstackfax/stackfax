# Stackfax Private Folder Setup

This file defines the early private folder structure for Stackfax.

The goal is to keep public project files clean while protecting private business notes, proprietary report logic, beta user details, pricing experiments, and internal operating material.

Stackfax should have a clear boundary between:

- public doctrine
- public sample reports
- public templates
- private engine notes
- private user notes
- private business planning

---

## Core Rule

Do not store private user information, sensitive intake details, proprietary scoring logic, payment details, credentials, or internal business planning in the public repo.

Public repo is for:

- public doctrine
- templates
- sample reports
- public-safe examples
- general scoring language
- anonymized patterns
- product education

Private folder is for:

- proprietary logic
- beta notes
- manual report operations
- private planning
- intake interpretation
- pricing experiments
- internal report generation notes

---

## Recommended Private Folder Name

Use a simple local folder name:

```text
Stackfax_Private
```
Recommended local path:

~/Documents/Stackfax_Private

Alternative local path:

~/Desktop/Stackfax_Private

Do not place this folder inside the public GitHub repo.

---

Recommended Folder Structure

Stackfax_Private/
  00-control/
  01-private-engine-notes/
  02-beta-users/
  03-manual-reports/
  04-pricing-and-offers/
  05-intake-notes/
  06-gold-reports-distillation/
  07-private-prompts/
  08-business-ops/
  09-archive/

  00-control

Purpose:

Keep private source-of-truth notes for what exists, what is active, and what should not be public.

Possible files:

PRIVATE_CONTROL_PANEL.md
private-boundary-rules.md
current-private-priorities.md
do-not-publish-list.md

Use this folder for private operating control, not public-facing copy.

⸻

01-private-engine-notes

Purpose:

Protect Stackfax report logic that should not be fully public.

This may include:

* proprietary scoring logic
* intake interpretation rules
* report generation logic
* verdict selection logic
* badge assignment logic
* risk weighting
* prompt chains
* report assembly rules
* private quality checks

Possible files:

private-engine-notes.md
scoring-logic-private.md
verdict-selection-rules.md
badge-assignment-rules.md
report-generation-flow.md

Public repo can show the standard.

Private engine notes protect the deeper machinery.

⸻

02-beta-users

Purpose:

Track beta users and report outcomes privately.

This folder may include:

* beta user notes
* intake summaries
* report delivery status
* feedback
* follow-up notes
* recheck timing
* anonymized lessons

Possible files:

beta-user-tracker.md
beta-feedback-log.md
first-10-beta-targets.md

Do not store sensitive user data unless absolutely necessary.

Prefer anonymized labels such as:

Beta User 001
Hardware-Curious Builder 001
Token-Burned Builder 001
Business Automation User 001

03-manual-reports

Purpose:

Store drafts and delivered private report copies.

Possible files:

report-drafts/
delivered-reports/
report-feedback/

Recommended structure:

03-manual-reports/
  drafts/
  delivered/
  feedback/
  rechecks/

  Use anonymized file names when possible.

Example:

quick-report-beta-user-001.md
token-burn-audit-beta-user-002.md
hardware-verdict-beta-user-003.md

Do not put private report drafts in the public repo.

⸻

04-pricing-and-offers

Purpose:

Track private pricing experiments and offer tests.

This may include:

* $19 Quick Report test
* deeper report pricing
* business audit pricing
* recheck pricing
* refund observations
* conversion notes
* Gumroad or payment setup notes
* first-dollar test results

Possible files:

pricing-experiments.md
first-dollar-results.md
offer-tests.md
refund-notes.md
gumroad-cleanup.md

Public docs can mention general offers.

Private files track actual experiments and results.

⸻

05-intake-notes

Purpose:

Track how real intake answers map into report logic.

This may include:

* common intake patterns
* confusing answers
* missing fields
* unsafe submissions
* follow-up question improvements
* public form revisions
* internal interpretation rules

Possible files:

intake-patterns.md
unsafe-intake-examples.md
follow-up-question-bank.md
public-form-revisions.md

Do not store raw sensitive intake data.

Convert raw intake into safe notes when possible.

⸻

06-gold-reports-distillation

Purpose:

Turn raw scouting signals into clean Stackfax doctrine.

This is where Gold Reports become cleaned rules before public or private sourcing.

Possible files:

gold-report-distillation-log.md
diamond-gold-candidates.md
clean-for-psi.md
keeper-lines.md
report-lane-map.md

Use this folder for:

* raw signal summaries
* keeper lines
* future docs
* doctrine candidates
* report section ideas
* risk flag candidates
* product lane ideas

Do not copy private Reddit messages, private user data, or sensitive screenshots here.

Use public-safe summaries.

⸻

07-private-prompts

Purpose:

Store private prompt chains and report generation prompts.

This may include:

* report drafting prompts
* intake analysis prompts
* scoring prompts
* recheck prompts
* beta feedback prompts
* private quality review prompts

Possible files:

quick-report-drafting-prompt.md
free-mini-report-prompt.md
token-burn-audit-prompt.md
business-automation-audit-prompt.md
quality-review-prompt.md

These should stay private until the public/private boundary is intentionally changed.

Prompt logic without metadata becomes invisible infrastructure.

Treat prompts like code.

⸻

08-business-ops

Purpose:

Track internal business operations.

This may include:

* domain notes
* email setup
* Gumroad cleanup
* payment links
* landing page setup
* checklist items
* operating notes
* legal/accounting questions to ask later

Possible files:

business-ops-checklist.md
domain-and-email-notes.md
gumroad-payout-cleanup.md
payment-links.md
launch-checklist.md

Do not store passwords, API keys, recovery codes, wallet information, or payment details.

⸻

09-archive

Purpose:

Store old private notes that should not remain active.

Use this for:

* outdated pricing ideas
* retired prompt drafts
* old beta notes
* superseded report logic
* old planning notes

Possible files:

archived-pricing.md
archived-prompts.md
archived-product-notes.md

Archive does not mean public.

Archived private material should stay private.

⸻

Public Repo Boundary

The public GitHub repo may include:

* README
* public templates
* public sample reports
* public doctrine
* public-safe operating notes
* anonymized examples
* rating system overview
* badge definitions
* report schema
* field research patterns without private data

The public repo should not include:

* private user details
* beta user identities
* raw intake forms
* private report drafts
* proprietary scoring weights
* private prompt chains
* payment details
* credentials
* API keys
* wallet information
* sensitive screenshots
* customer data
* legal or financial documents

⸻

Private Folder Safety Checklist

Before adding anything to the private folder, ask:

* Does this contain private user information?
* Does this contain credentials or secrets?
* Does this belong in public repo instead?
* Does this expose proprietary report logic?
* Does this need anonymizing?
* Does this need to be deleted instead of stored?
* Would this be dangerous if accidentally committed?

If the answer is unclear, keep it out of the public repo.

⸻

Git Safety Rule

Do not initialize this private folder as a public GitHub repo.

Do not drag this folder into the Stackfax public repo.

Do not commit private files by accident.

If using Git locally later, add a clear .gitignore and keep any remote private.

Recommended warning file:

DO_NOT_COMMIT_PRIVATE_FILES.md

This folder contains private Stackfax operating notes.

Do not commit this folder to the public Stackfax repo.

Do not upload private user data, report drafts, credentials, payment details, or proprietary engine notes to public GitHub.

Naming Rule

Use clear, boring file names.

Good:

private-engine-notes.md
beta-feedback-log.md
pricing-experiments.md
quick-report-drafting-prompt.md

Avoid:

final-final-real-notes.md
secret-stuff.md
random.md
stackfax-brain-dump.md

A private folder should still be easy to navigate.

⸻

Private-To-Public Distillation Rule

Some private notes may become public later.

Before moving anything public, distill it.

Raw private note:

Beta user asked about exact customer workflow and shared sensitive details.

Public-safe distillation:

Some business automation users need approval gates before customer-facing actions.

The public version should preserve the lesson without exposing the person, business, or private details.

Clean For PSI Rule

Use this path when turning raw private notes into project canon:

raw signal → clean rule → public-safe wording → Project source it

Do not project-source raw private material.

Project-source only clean, durable, public-safe doctrine or approved internal source material.

⸻

Final Rule

Public repo builds trust.

Private folder protects the engine.

Do not confuse the two.
