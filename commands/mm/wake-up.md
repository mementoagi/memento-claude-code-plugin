---
description: Start a new session — loads identity, memory, and recent context so your AI picks up where the last session left off.
---

Call the `get-command-instructions` MCP tool with `command: "wake-up"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/wake-up.md` and follow those instructions.
