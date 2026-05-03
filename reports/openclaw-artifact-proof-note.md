# OpenClaw Artifact Proof Note

This note captures a simple Stackfax rule for beginner OpenClaw and coding-agent workflows.

Core rule:

> No claim without an artifact.

If an agent says it created, ran, tested, changed, sent, moved, or fixed something, the user should be able to see proof.

Useful artifacts include:

- file path
- command output
- screenshot
- log entry
- test result
- diff
- run receipt
- clear summary of what changed

---

## Why This Matters

Beginner OpenClaw users may trust the agent’s summary before they know how to verify the work.

That creates risk.

An agent can sound confident while:

- creating the file in the wrong place
- failing to run the command
- skipping the test
- changing the wrong file
- summarizing stale output
- hiding an error
- claiming completion without evidence

The fix is not distrust.

The fix is evidence.

---

## Safer Beginner Pattern

Use this pattern:

```text
agent suggests → human approves → agent acts → result is logged
