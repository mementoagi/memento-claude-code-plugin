---
description: Save the current task to persistent memory (AGI plan).
---

Call the `get-command-instructions` MCP tool with `command: "task/add-task-to-memory.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/task/add-task-to-memory.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
