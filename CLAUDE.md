# Memento AI Memory

You have access to **persistent memory** through the Memento MCP server. This memory survives across sessions — anything you save now will be available in future conversations.

## Session Lifecycle

1. **Start of session**: Run `/memento:wake-up` to load your identity, working memory, and recent context
2. **During session**: Use `recall` MCP tool before coding tasks; use `remember` MCP tool when you learn something new
3. **End of session**: Run `/memento:sleep` to consolidate memory and create a handoff

## Key MCP Tools

- **`recall`** — Search persistent memory (keyword + semantic + graph). Use before making assumptions.
- **`remember`** — Save knowledge to memory. Use when the user corrects you or you learn something.
- **`read-file`** / **`write-file`** / **`str-replace`** — Direct file operations on memory.
- **`get-command-instructions`** — Fetch the latest command logic from Memento Cloud.

## Memory Paths

- `personal/` — Your identity, knowledge, daily stack, top of mind
- `system/` — Capabilities, commands, meta-knowledge
- `org:/` — Org-level shared knowledge (codebase, projects, conventions)

## Setup

If the Memento MCP server is not connected, the user may need to re-enter their API key. Run `/memento:wake-up` to check — if it fails, reinstall the plugin or update the key at https://mementoagi.com/dashboard/settings.
