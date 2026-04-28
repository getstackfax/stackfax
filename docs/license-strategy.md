# Stackfax License Strategy

The Stackfax License Strategy defines how Stackfax should think about public access, ownership, reuse, and future licensing.

The goal is to build public trust without accidentally giving away the full business engine too early.

## Core Question

What should Stackfax make public, what should stay private, and what rights should others have to reuse the work?

## Current Recommendation

Stackfax should not rush into a standard open-source license.

The current best-fit direction is:

Public trust layer, private business engine.

This means Stackfax can show enough to build trust while keeping customer workflows, scoring automation, paid delivery systems, and internal operations protected.

## Main Structure Options

### Open-Source

Open-source means people can usually use, copy, modify, and redistribute the project under a license such as MIT, Apache, or GPL.

Potential benefits:

- Builds community trust
- Makes contribution easier
- Can help Stackfax become a shared standard
- Encourages public adoption

Potential risks:

- Others may copy the report system
- Others may reuse the templates commercially
- Brand language and structure may be cloned
- Harder to protect the early business model

Stackfax fit:

Probably too open too early.

### Source-Available

Source-available means people can see the source, docs, or system, but do not automatically get broad rights to reuse, resell, or commercialize it.

Potential benefits:

- Public can inspect the work
- Builds trust
- Shows seriousness
- Protects more of the business than open-source
- Can allow learning without allowing direct cloning

Potential risks:

- Some people dislike restrictive licenses
- Still reveals public logic
- Requires clear legal language later

Stackfax fit:

Possibly useful later for selected public tools, examples, or standards.

### Public Documentation Only

Public documentation only means the public repo contains docs, examples, guides, sample reports, and public-facing standards, but not the actual app, scoring engine, customer workflow, or internal systems.

Potential benefits:

- Good for credibility
- Good for SEO
- Good for education
- Low risk
- Fits the current repo
- Keeps operations private

Potential risks:

- Some people may copy visible docs or language
- Does not automatically create a protected product moat
- Still needs clear copyright and usage notes later

Stackfax fit:

Best current fit.

### Private-Product Foundation

Private-product foundation means the important product logic, paid workflow, scoring automation, customer reports, and operating systems stay private.

Potential benefits:

- Protects the business engine
- Protects customer data
- Protects paid report delivery
- Protects future automation
- Protects internal OpenClaw and Rabble Scout systems

Potential risks:

- Less public transparency
- Less community contribution
- Trust must be built through public docs, examples, and results

Stackfax fit:

Strong fit for the private side of the business.

### Mixed Public/Private Structure

Mixed public/private means some parts are public and some parts are private.

This may be the strongest long-term setup for Stackfax.

Public:

- Brand docs
- Field guide
- Sample reports
- Public report types
- Basic templates
- Marketing copy
- Education
- High-level scoring philosophy
- Public safety/risk language

Private:

- Actual paid report workflow
- Customer submissions
- Scoring engine
- Payment and intake operations
- Automation scripts
- Internal notes
- Advanced templates
- Real customer reports
- OpenClaw/Rabble Scout working system

Stackfax fit:

Best long-term fit.

## Current Public Layer

The public repo can safely include:

- README
- Brand assets tracker
- Report type docs
- Sample reports
- Basic templates
- Field guide
- Marketing copy
- SEO keyword map
- Risk category docs
- Public principles
- Community standards plan
- License strategy

These help users understand Stackfax without exposing private customer operations.

## Future Private Layer

The private side should include:

- Real customer submissions
- Payment links and order records
- Actual report delivery workflow
- Internal scoring system
- Paid report production process
- Customer communications
- Advanced report templates
- Internal automation scripts
- Private OpenClaw/Rabble Scout workflows
- Business analytics
- Financial records
- Refunds and support workflows

## What Not To Put In The Public Repo

Do not put these in the public repo:

- Passwords
- API keys
- Recovery codes
- Payment details
- Customer submissions
- Real customer reports
- Private emails
- Personal information
- Client data
- Wallet information
- Financial account information
- Internal automation credentials
- Private OpenClaw configs
- Anything that could expose users or customers

## License Timing

Do not choose a final license just to satisfy GitHub’s green checklist.

A license should be chosen after Stackfax decides whether the repo is:

- Public documentation only
- Source-available
- Open-source
- Mixed public/private
- Private product with public marketing docs

## Possible Future License Direction

Stackfax may eventually use different rules for different parts.

Possible split:

- Public docs: copyright protected, limited reuse
- Educational guides: shareable with attribution
- Code tools: source-available or open-source
- Brand assets: protected
- Paid templates: private
- Customer reports: private
- Scoring engine: private

## Community Standards Note

GitHub may encourage adding a license, code of conduct, contributing guide, security policy, issue templates, and pull request templates.

That checklist is useful, but it should not override business strategy.

Community files should be added when they help the project.

License should be added when the strategy is clearer.

## Stackfax Principle

Show enough to build trust.

Keep enough private to build the business.

Public trust layer.

Private business engine.
