---
description: Investigate the user's codebase and auto-fill their AGI config guides, asking only about gaps the code can't answer.
---

Call the `get-command-instructions` MCP tool with `command: "utility/scan-environment"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/utility/scan-environment.md` and follow those instructions.
