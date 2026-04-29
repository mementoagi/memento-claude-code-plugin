---
description: Pull the next task off the queue and start working on it.
---

Call the `get-command-instructions` MCP tool with `command: "dequeue.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/dequeue.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
