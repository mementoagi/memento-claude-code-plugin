---
description: Save information to persistent memory with proper classification and linking.
argument-hint: <what to remember>
---

Call the `get-command-instructions` MCP tool with `command: "remember"` and `args: "$ARGUMENTS"`, then execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/remember.md` and follow those instructions using "$ARGUMENTS" as the information to save.
