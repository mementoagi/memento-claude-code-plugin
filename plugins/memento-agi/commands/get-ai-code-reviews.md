---
description: Fetch open AI code-review comments on your PRs.
---

Call the `get-command-instructions` MCP tool with `command: "beta/get-ai-code-reviews.md"` and execute the returned instructions.

If `get-command-instructions` is unavailable, call `read-node` with path `core/commands/beta/get-ai-code-reviews.md` and follow those instructions.

If the cloud rejects with a tier-related error, your account does not include AGI-tier commands. Visit https://mementoagi.com/dashboard/plan to upgrade.
