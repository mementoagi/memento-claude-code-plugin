---
description: Create a handoff document for the next session or agent.
---

Call the `get-command-instructions` MCP tool with `command: "handoff"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/handoff.md` and follow those instructions.
