---
description: Edit an existing Memento slash command in the cloud catalog.
---

Call the `get-command-instructions` MCP tool with `command: "edit-command.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/edit-command.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include Beta-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
