# Memento: AI Memory for Claude Code

Persistent, transparent, shareable memory for your AI coding assistant. Your AI remembers your codebase, conventions, and team knowledge across every session.

## What Memento Does

Every AI coding session starts from zero. Memento changes that.

- **Persistent memory** across sessions. Your AI remembers your architecture, conventions, and patterns.
- **Transparent markdown.** See, edit, and control everything your AI knows.
- **Team shared context.** Org-level memory so your whole team's AI shares knowledge.
- **Autonomous coding.** A memory-powered AGI loop that plans, builds, tests, reviews, and ships.
- **Cloud-native.** Works across machines, zero local setup.

## Memory Is Mostly Automatic

The `memento-memory` skill teaches Claude to recall context before starting work and save discoveries as they happen. Most of the time you won't need explicit commands.

When you want to drive it directly:

- `/mm/remember <thing>` to save something specific (a decision, a convention, a gotcha)
- `/mm/recall <topic>` to search memory for a topic
- `/mm/wake-up` at the start of a session to load your full context

## What This Plugin Provides

### Skills (auto-loaded by Claude when relevant)

| Skill | What it does |
|-------|-------------|
| `memento-memory` | Teaches Claude to proactively save discoveries and recall context before working |
| `memento-session` | Teaches Claude session lifecycle: wake-up to load memory, sleep to consolidate |
| `memento-tickets` | Teaches Claude to use the ticket system for task tracking |

### Hooks

| Event | Action |
|-------|--------|
| `SessionStart` | Reminds Claude to run wake-up and load memory |

### Agents

| Agent | What it does |
|-------|-------------|
| `memento-coder` | Memory-powered coding agent that recalls context before working and saves discoveries |

### MCP Server

Automatically connects to Memento Cloud. No manual `claude mcp add` needed.

## Setup

### 1. Create an account (free)

Sign up at [mementoagi.com](https://mementoagi.com/signup).

### 2. Install the plugin

```bash
claude plugin install memento@memento-plugins
```

Claude Code will prompt you for your Memento API key. Find it at [mementoagi.com/dashboard/settings](https://mementoagi.com/dashboard/settings). The key is stored securely in your system keychain.

### 3. Start your first session

```
/memento:mm/wake-up
```

Your AI comes with its own identity. The first session introduces it to you and begins building memory.

## Commands

### Included (all tiers)

| Command | What it does |
|---------|-------------|
| `/mm/wake-up` | Start a session: loads identity, memory, recent context |
| `/mm/recall` | Search and load from memory |
| `/mm/remember` | Save information to persistent memory |
| `/mm/sleep` | End session, consolidate memory |
| `/mm/utility/sync-commands` | Refresh commands after upgrading your tier |

Additional commands are available depending on your plan. Run `/mm/utility/sync-commands` to pull them in.

## How It Works

Memento uses the [Model Context Protocol (MCP)](https://spec.modelcontextprotocol.io/) to connect Claude Code to cloud-hosted persistent memory.

**Skills** teach Claude behavioral patterns: when to remember, when to recall, how to manage sessions. These are auto-loaded by Claude when relevant to your conversation.

**Commands** are thin stubs that fetch the latest logic from Memento Cloud at runtime, so your commands are always up to date.

**Hooks** automate lifecycle events. The `SessionStart` hook prompts Claude to load your memory at the beginning of each session.

Your AI's memory is stored as transparent markdown files:
- **Personal**: your identity, working memory, daily activity
- **Org**: team-shared codebase knowledge, conventions, projects
- **System**: AI capabilities, commands, meta-knowledge

---

For more information, visit [mementoagi.com](https://mementoagi.com).
