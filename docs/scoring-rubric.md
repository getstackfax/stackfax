# Stackfax Scoring Rubric

The Stackfax scoring rubric defines how Ai stacks are reviewed, scored, and explained.

The goal is not to reward the biggest stack, the most expensive tools, or the newest hardware.

The goal is to measure whether the stack fits the task.

## Core Question

Does this stack match the user's workload, budget, skill level, risk tolerance, privacy needs, and scaling goals?

## Score Range

Stackfax uses a 0–100 Stack Score.

Suggested rating bands:

- 0–39: Poor fit
- 40–59: Risky or unclear fit
- 60–74: Usable starter stack
- 75–89: Strong stack
- 90–100: Excellent stack

A higher score does not mean the stack is bigger.

A higher score means the stack is better matched to the job.

## Star Rating

Stackfax also uses a 1–5 star rating.

Suggested star bands:

- ⭐: 0–24
- ⭐⭐: 25–49
- ⭐⭐⭐: 50–69
- ⭐⭐⭐⭐: 70–84
- ⭐⭐⭐⭐⭐: 85–100

A 5-star stack is not always the most expensive stack.

A 5-star stack is the stack that best fits the task.

## Main Categories

### 1. Use-Case Fit

Checks whether the stack matches what the user is actually trying to do.

Signals of good fit:

- Clear primary use case
- Tools match the task
- Models are assigned to the right jobs
- Hardware is justified by the workload
- Workflow is understandable

Signals of weak fit:

- No clear task
- Too many tools
- Copying a creator or vendor stack without context
- Buying hardware before proving the workflow
- Using one powerful model for everything

### 2. Cost And Token Discipline

Checks whether the stack avoids unnecessary spending.

Signals of good fit:

- Cheap models handle simple work
- Strong models are reserved for judgment or final review
- Token use is bounded
- Session budget caps exist
- Context is kept relevant
- Subscriptions do not heavily overlap

Signals of weak fit:

- Premium models used for routine tasks
- Large context loaded by default
- Silent fallback escalation
- Multiple overlapping subscriptions
- No cost visibility
- No budget caps

### 3. Model Routing

Checks whether the stack uses the right model for each layer of work.

Recommended pattern:

- Cheap model drafts
- Cheap or mid-tier model summarizes
- Strong model reasons or decides
- Human approves important actions

Signals of weak fit:

- One model handles every task
- Expensive model does extraction work
- No fallback visibility
- No model cap
- No separation between draft, review, and decision layers

### 4. Hardware Fit

Checks whether local hardware is actually needed.

Signals of good fit:

- Hardware is tied to a specific workflow
- Local model testing is justified
- Privacy or isolation requirements are real
- Always-on local workflows are proven
- Dedicated workspace has a clear purpose

Signals of weak fit:

- Buying a Mac mini because of hype
- Buying local hardware before defining the workflow
- Running cloud-friendly tasks locally for no clear reason
- Overbuying RAM or storage without a workload
- Treating hardware as the solution before stack design

### 5. Local Vs Cloud Fit

Checks whether the stack should be cloud-first, local-first, or hybrid.

Cloud-first fits when:

- Tasks are mostly research, summaries, drafts, or reports
- Local models are not required
- Uptime can be handled by hosted tools
- The user is still proving the workflow

Local-first fits when:

- Privacy isolation matters
- Local model testing matters
- The user needs a dedicated Ai lab
- The workload benefits from local runtime control

Hybrid fits when:

- Cloud models handle heavy reasoning
- Local tools handle safe, bounded workflows
- Private or sensitive data stays isolated
- The workflow is proven enough to split cleanly

### 6. Permission And Approval Gates

Checks whether the stack has safe boundaries.

Human approval should be required before:

- Sending messages
- Posting publicly
- Contacting customers
- Changing files
- Moving or deleting files
- Connecting credentials
- Accessing wallets
- Touching financial accounts
- Editing customer records
- Changing inventory
- Processing payments
- Modifying production systems

Signals of weak fit:

- Agents can act without review
- Credentials are broadly shared
- Customer-facing actions are automated too early
- No written approval rules
- No list of forbidden actions

### 7. Privacy And Credential Isolation

Checks whether sensitive data is separated properly.

Signals of good fit:

- Personal files are isolated
- Client data is separated
- Credentials are scoped
- Browser sessions are not shared across clients
- Agents have limited access
- Private data is not loaded unless needed

Signals of weak fit:

- One agent has access to everything
- Multiple clients share the same browser/session/context
- Credentials are stored loosely
- Personal and business data are mixed
- Private data is loaded into unnecessary model calls

### 8. Workflow Design

Checks whether the task is structured well.

Good workflow structure:

- Define task
- Gather data
- Filter or extract with code/tools where possible
- Summarize
- Reason
- Draft
- Review
- Human approves
- Save/send only after approval

Weak workflow structure:

- One broad agent prompt does everything
- Ai performs deterministic work that code could do
- No clear inputs or outputs
- No checkpoint before action
- No separation between research, judgment, and execution

Stackfax principle:

Use code for extraction. Use Ai for judgment.

### 9. Reliability And Uptime

Checks whether the stack is ready for real use.

Signals of good fit:

- Failures are expected
- Restart behavior is understood
- Logs exist
- Important tasks have human review
- Production workflows are not run from fragile setups
- Uptime needs match hosting choice

Signals of weak fit:

- Always-on workflows run on a machine not designed for them
- Updates or restarts can break work
- No fallback plan
- No monitoring
- Real customer workflows rely on experimental setups

### 10. Scaling Path

Checks whether the stack can grow without breaking cost, safety, or control.

Signals of good fit:

- First workflow is clear
- Future upgrades are staged
- More tools are added only after need is proven
- Costs can be tracked
- Permissions can be tightened
- New users or clients can be isolated

Signals of weak fit:

- Scaling plan depends only on buying bigger hardware
- Costs are unknown
- More agents are added before the first workflow is proven
- Client/customer boundaries are unclear
- No 30-day recheck plan

## Common Risk Badges

Stackfax may apply badges such as:

- StackChecked
- Token-Smart
- Cloud-First
- Local-Ready
- Mac Mini Justified
- Hardware Not Required Yet
- Overbuild Risk
- Human Approval Required
- Customer Data Risk
- Credential Isolation Risk
- Context Bloat Risk
- Silent Escalation Risk
- Fragile UI Automation Risk
- Vendor Stack Overkill Risk
- Uptime Risk

## Scoring Guidance

A sample scoring split:

- Use-case fit: 15 points
- Cost and token discipline: 15 points
- Model routing: 10 points
- Hardware fit: 10 points
- Local vs cloud fit: 10 points
- Permission and approval gates: 15 points
- Privacy and credential isolation: 10 points
- Workflow design: 10 points
- Reliability and uptime: 5 points

Total: 100 points

The weighting can change by report type.

For example:

- A hardware verdict may weigh hardware fit more heavily.
- A token burn audit may weigh cost, context, and model routing more heavily.
- A business automation audit may weigh approval gates and credential isolation more heavily.

## Final Rule

Do not reward complexity by default.

Reward fit, clarity, safety, cost discipline, and upgrade path.

A small stack that does the job safely can score higher than a huge stack that is expensive, risky, or unclear.
