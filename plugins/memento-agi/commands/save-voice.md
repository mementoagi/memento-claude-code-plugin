---
description: Save a new voice profile from current AI output style.
---

Call the `get-command-instructions` MCP tool with `command: "enterprise/save-voice.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/enterprise/save-voice.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
