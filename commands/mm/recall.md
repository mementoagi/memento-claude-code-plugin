---
description: Search and load knowledge from persistent memory into active context.
argument-hint: <query>
---

Call the `get-command-instructions` MCP tool with `command: "recall"` and `args: "$ARGUMENTS"`, then execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/recall.md` and follow those instructions using "$ARGUMENTS" as the query.
