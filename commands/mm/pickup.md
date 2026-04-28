---
description: Load a specific handoff by topic name, or list all pending handoffs.
argument-hint: [topic]
---

Call the `get-command-instructions` MCP tool with `command: "pickup"` and `args: "$ARGUMENTS"`, then execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/pickup.md` and follow those instructions using "$ARGUMENTS" as the topic.
