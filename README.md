# Memento — AI Memory for Claude Code

Persistent, transparent, shareable memory for your AI coding assistant. Your AI remembers your codebase, conventions, and team knowledge across every session.

## What Memento Does

Every AI coding session starts from zero. Memento changes that.

- **Persistent memory** across sessions — your AI remembers your architecture, conventions, and patterns
- **Transparent markdown** — see, edit, and control everything your AI knows
- **Team shared context** — org-level memory so your whole team's AI shares knowledge
- **Autonomous coding** — memory-powered AGI loop that plans, builds, tests, reviews, and ships
- **Cloud-native** — works across machines, zero local setup

## What This Plugin Provides

### Skills (auto-loaded by Claude when relevant)

| Skill | What it does |
|-------|-------------|
| `memento-memory` | Teaches Claude to proactively remember discoveries and recall context before working |
| `memento-session` | Teaches Claude about session lifecycle — wake-up to load memory, sleep to consolidate |
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

Automatically connects to Memento Cloud — no manual `claude mcp add` needed.

## Setup

### 1. Create a free account

Sign up at [mementoagi.com](https://mementoagi.com).

### 2. Install the plugin

```bash
claude plugin install memento@memento-plugins
```

Claude Code will prompt you for your Memento API key. Find it at [mementoagi.com/dashboard/settings](https://mementoagi.com/dashboard/settings). The key is stored securely in your system keychain.

### 3. Start your first session

```
/memento:mm/wake-up
```

Your AI will create its identity, learn about you, and start building persistent memory.

## Commands

### Included (all tiers)

| Command | What it does |
|---------|-------------|
| `/mm/wake-up` | Start a session — loads identity, memory, recent context |
| `/mm/recall` | Search and load from memory (auto-runs `/frame` afterward) |
| `/mm/remember` | Save information to persistent memory (auto-runs `/frame` afterward) |
| `/mm/sleep` | End session, consolidate memory |
| `/mm/utility/sync-commands` | Refresh commands after upgrading your subscription tier |

### After upgrading (Pro and above)

Run `/mm/utility/sync-commands` after upgrading your tier to pull in additional commands:

| Command | Tier | What it does |
|---------|------|-------------|
| `/mm/frame` | Pro | Assess state, propose next action |
| `/mm/handoff` | Pro | Prepare context for a new thread |
| `/mm/commit` | Pro | Stage, commit, push with conventions |
| `/mm/investigate-and-cache` | Pro | Deep-dive a codebase area, save findings |
| `/mm/note-gotcha` | Pro | Save file-specific code warning to technical mirror |
| `/mm/todo/*` | Pro | Task management (add, list, work, save to memory) |
| `/mm/complete-project` | AGI | End-to-end: plan, build, test, review, ship |
| `/mm/make-a-project` | AGI | Create project structure in memory |
| `/mm/do-it-in-a-browser` | AGI | Browser-based UI verification |

## How It Works

Memento uses the [Model Context Protocol (MCP)](https://spec.modelcontextprotocol.io/) to connect Claude Code to cloud-hosted persistent memory.

**Skills** teach Claude behavioral patterns — when to remember, when to recall, how to manage sessions. These are auto-loaded by Claude when relevant to your conversation.

**Commands** are generated dynamically based on your subscription tier. Each is a thin stub that fetches the latest logic from Memento Cloud at runtime — so your commands are always up to date.

**Hooks** automate lifecycle events. The `SessionStart` hook prompts Claude to load your memory at the beginning of each session.

Your AI's memory is stored as transparent markdown files:
- **Personal**: your identity, working memory, daily activity
- **Org**: team-shared codebase knowledge, conventions, projects
- **System**: AI capabilities, commands, meta-knowledge

## Pricing

- **Free**: 50 MB storage, 3 orgs
- **Pro**: 500 MB, unlimited orgs, priority support
- **Team**: 2 GB, team management, shared memory

## Links

- [Website](https://mementoagi.com)
- [Dashboard](https://mementoagi.com/dashboard)
- [Vision](https://mementoagi.com/vision)
- [AGI Features](https://mementoagi.com/agi)
