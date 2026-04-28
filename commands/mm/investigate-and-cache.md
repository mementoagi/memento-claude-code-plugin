---
description: Deep-scan a codebase area and save structured findings to memory.
argument-hint: <area to investigate>
---

Call the `get-command-instructions` MCP tool with `command: "investigate-and-cache"` and `args: "$ARGUMENTS"`, then execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/investigate-and-cache.md` and follow those instructions using "$ARGUMENTS" as the area to investigate.
