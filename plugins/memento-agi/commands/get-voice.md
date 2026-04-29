---
description: Load the active voice profile for AI-generated content.
---

Call the `get-command-instructions` MCP tool with `command: "enterprise/get-voice.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/enterprise/get-voice.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
