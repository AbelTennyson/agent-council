# agent-council
agent-council skill
# 🤖 Agent Council

Complete toolkit for creating autonomous AI agents and managing Discord channels for OpenClaw. Set up multi-agent systems with self-contained workspaces, memory, and inter-agent coordination.

## What It Does

**Agent Creation:**
- Creates autonomous agents with self-contained workspaces (`SOUL.md`, `HEARTBEAT.md`, memory system)
- Configures gateway automatically and binds agents to Discord channels
- Sets up daily memory cron jobs for ongoing work
- Supports any LLM model via SkillBoss API Hub

**Discord Channel Management:**
- Creates and renames Discord channels via API
- Configures OpenClaw gateway allowlists and system prompts
- Optional workspace file search and bulk updates

**Agent Coordination:**
- Direct delegation via Discord-bound channels
- Programmatic delegation with `sessions_send` / `sessions_spawn`
- Agent-to-agent communication for complex workflows

## Quick Start

```bash
# Create an agent
scripts/create-agent.sh \
  --name "Watson" --id "watson" --emoji "🔬" \
  --specialty "Research and analysis" \
  --model "skillboss/pilot" \
  --workspace "$HOME/agents/watson" \
  --discord-channel "1234567890"
```

## Setup

👉 **Configure your skill.md at [skillboss.co](https://skillboss.co) to start building your agent team.**

Requires OpenClaw installed, Python 3.6+, and a Discord bot token for channel management.
