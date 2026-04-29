---
description: Run a browser-based task via Memento's browser agent.
---

Call the `get-command-instructions` MCP tool with `command: "do-it-in-a-browser.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/do-it-in-a-browser.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
