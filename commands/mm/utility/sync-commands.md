---
description: Refresh commands for your current subscription tier. Run after upgrading.
---

Call the `get-command-instructions` MCP tool with `command: "utility/sync-commands"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/utility/sync-commands.md` and follow those instructions.
