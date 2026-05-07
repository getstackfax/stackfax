# Stackfax License Strategy

The Stackfax License Strategy defines how Stackfax should think about public access, ownership, reuse, contribution, and future licensing.

The goal is to build public trust without accidentally giving away the full business engine too early.

⸻

## Core Question

What should Stackfax make public, what should stay private, and what rights should others have to reuse the work?

Stackfax should not choose a license just to satisfy a checklist.

License strategy should follow product strategy.

⸻

## Current Recommendation

Stackfax should not rush into a standard open-source license.

The current best-fit direction is:

Public trust layer. Private business engine.

This means Stackfax can show enough to build trust while keeping customer workflows, scoring automation, paid delivery systems, advanced report logic, and internal operations protected.

⸻

# Main Structure Options

## Open-Source

Open-source means people can usually use, copy, modify, and redistribute the project under a license such as MIT, Apache, or GPL.

## Potential Benefits

* builds community trust
* makes contribution easier
* can help Stackfax become a shared standard
* encourages public adoption
* makes public tools easier to reuse

## Potential Risks

* others may copy the report system
* others may reuse templates commercially
* brand language and structure may be cloned
* harder to protect the early business model
* harder to separate public standard from paid product

## Stackfax Fit

Probably too open too early.

Open-source may make sense later for narrow tools, examples, or public helpers, but not for the full business engine.

⸻

## Source-Available

Source-available means people can see the source, docs, or system, but do not automatically get broad rights to reuse, resell, or commercialize it.

## Potential Benefits

* public can inspect the work
* builds trust
* shows seriousness
* protects more of the business than open-source
* can allow learning without allowing direct cloning

## Potential Risks

* some people dislike restrictive licenses
* still reveals public logic
* requires clear legal language later
* may confuse contributors if rights are unclear

## Stackfax Fit

Possibly useful later for selected public tools, examples, or standards.

Not the first priority right now.

⸻

## Public Documentation Only

Public documentation only means the public repo contains docs, examples, guides, sample reports, report-type definitions, and public-facing standards, but not the actual app, scoring engine, customer workflow, private prompts, or internal systems.

## Potential Benefits

* good for credibility
* good for SEO
* good for education
* low risk
* fits the current repo
* keeps operations private
* supports public trust without exposing the engine

## Potential Risks

* people may copy visible docs or language
* does not automatically create a protected product moat
* still needs clear copyright and usage notes later

## Stackfax Fit

Best current fit.

The current public repo is mostly a trust/documentation layer, not the full product engine.

⸻

## Private-Product Foundation

Private-product foundation means the important product logic, paid workflow, scoring automation, customer reports, and operating systems stay private.

## Potential Benefits

* protects the business engine
* protects customer data
* protects paid report delivery
* protects future automation
* protects internal OpenClaw and Rabble Scout systems
* protects proprietary interpretation and scoring logic

## Potential Risks

* less public transparency
* less community contribution
* trust must be built through public docs, examples, and actual delivery

## Stackfax Fit

Strong fit for the private side of the business.

⸻

# Mixed Public / Private Structure

Mixed public/private means some parts are public and some parts are private.

This is likely the strongest long-term setup for Stackfax.

## Public

* brand docs
* field guide
* sample reports
* public report types
* basic templates
* marketing copy
* education
* high-level scoring philosophy
* public safety/risk language
* public badge definitions
* public intake warnings
* public community standards
* public “what is Stackfax?” docs

## Private

* actual paid report workflow
* customer submissions
* scoring engine
* payment and intake operations
* automation scripts
* internal notes
* advanced templates
* real customer reports
* OpenClaw/Rabble Scout working system
* proprietary prompt chains
* private interpretation rules

## Stackfax Fit

Best long-term fit.

Public standard.

Private engine.

⸻

## Current Public Layer

The public repo can safely include:

* README
* brand assets tracker
* report type docs
* sample reports
* basic templates
* field guide
* marketing copy
* SEO keyword map
* risk category docs
* public principles
* community standards plan
* license strategy
* scoring philosophy
* public/private roadmap
* get involved guide
* fictional examples clearly labeled
* safe anonymized product lessons

These help users understand Stackfax without exposing private customer operations.

⸻

# Future Private Layer

## The private side should include:

* real customer submissions
* payment links and order records
* actual report delivery workflow
* internal scoring system
* paid report production process
* customer communications
* advanced report templates
* internal automation scripts
* private OpenClaw/Rabble Scout workflows
* business analytics
* financial records
* refunds and support workflows
* private feedback tied to specific users
* real testimonial permissions
* private report generator prompts
* proprietary scoring implementation
* report interpretation rules

⸻

# What Not To Put In The Public Repo

# Do not put these in the public repo:

* passwords
* API keys
* recovery codes
* payment details
* customer submissions
* real customer reports
* private emails
* personal information
* client data
* wallet information
* seed phrases
* private keys
* financial account information
* internal automation credentials
* private OpenClaw configs
* private Rabble Scout outputs
* private screenshots
* support messages
* private customer links
* anything that could expose users or customers

Default rule:

Public repo gets principles and samples. Private storage gets real people and real submissions.

⸻

## License Timing

Do not choose a final license just to satisfy GitHub’s green checklist.

A license should be chosen after Stackfax decides whether the repo is:

* public documentation only
* source-available
* open-source
* mixed public/private
* private product with public marketing docs

For now, the safest stance is:

* keep the public repo visible
* avoid adding a broad permissive license too early
* protect brand and paid workflow
* add clearer usage language later when the business boundary is firmer

⸻

## Possible Future License Direction

Stackfax may eventually use different rules for different parts.

### Possible split:

* public docs: copyright protected, limited reuse
* educational guides: shareable with attribution
* public examples: reusable with attribution if approved later
* code tools: source-available or open-source if narrow enough
* brand assets: protected
* paid templates: private
* customer reports: private
* scoring engine: private
* report generator: private
* badge verification mechanics: private

Not every part of Stackfax needs the same license.

⸻

# Brand Protection

## Stackfax should protect:

* Stackfax name
* StackChecked name
* badge names
* logos
* domain language
* report identity
* public trust marks
* paid report names

Even if some docs or tools become public, the brand should not become freely reusable by unrelated parties.

StackChecked especially should not become a loose badge anyone can apply without a real check.

⸻

## Contributor Rule

Before inviting meaningful outside contributions, Stackfax should clarify:

* what people can contribute
* whether contributions can be used commercially by Stackfax
* what rights contributors retain
* what parts are public
* what parts are private
* whether contributor work can enter paid products
* how attribution works
* what data contributors must not access

Until then, keep contributions small, reviewable, and public-doc-focused.

## Good early contributions:

* typo fixes
* clarity suggestions
* safe sample inputs
* public docs
* beginner feedback
* template cleanup
* structure suggestions

## Avoid early contributions that touch:

* customer data
* private report logic
* payment operations
* credentials
* advanced scoring engine
* private report prompts
* automation systems

⸻

## Community Standards Note

GitHub may encourage adding:

* license
* code of conduct
* contributing guide
* security policy
* issue templates
* pull request templates

That checklist is useful, but it should not override business strategy.

Community files should be added when they help the project.

License should be added when the strategy is clearer.

Do not let a green checklist accidentally give away the engine.

⸻

# Public Trust Without Full Exposure

### Stackfax can build trust publicly by showing:

* what the product checks
* why risk flags matter
* what sample reports look like
* how ratings work
* what safety rules apply
* what the public/private boundary is
* how customer data is protected
* what StackChecked does and does not mean

## Stackfax does not need to expose:

* paid report generator logic
* private scoring weights
* customer-specific reports
* internal prompts
* automation scripts
* private operations
* business lead flow
* badge verification mechanics

Public clarity is not the same thing as full disclosure.

⸻

# Stackfax Principle

Show enough to build trust.

Keep enough private to build the business.

Public trust layer.

Private business engine.

⸻

# Final Rule

Do not license away the engine before the business exists.

The standard can be visible.

The customer data stays private.

The paid engine stays protected.
