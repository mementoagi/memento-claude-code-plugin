---
description: Loop through queued tasks, executing each in turn.
---

Call the `get-command-instructions` MCP tool with `command: "task/work-on-tasks.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/task/work-on-tasks.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
