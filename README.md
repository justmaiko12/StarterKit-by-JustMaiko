# Michael's Starter Kit

One starter kit for Claude Code or Codex.

Use Claude Code if you want slash-command flow. Use Codex if you want Codex's
project-context flow. The project setup, handoff file, and starter skills are
the same.

## What you get

- First-run onboarding for Claude Code and Codex
- Teaching mode so you learn the system as you build
- The five starter skills/workflows from the Day 3 lesson
- A Trigger.dev automation skill for Day 6-style workflow builds
- A shared handoff file so sessions do not start from zero

## Setup

1. Click **Use this template** and clone it to your machine.
2. Open the folder in your coding tool.
3. Choose your path:

### Claude Code path

Open Claude Code in this folder and type:

```text
/start
```

Claude interviews you, updates `CLAUDE.md`, and suggests your first move.

### Codex path

Open Codex in this folder and paste the prompt from:

```text
prompts/codex-start.md
```

Codex interviews you, updates `AGENTS.md`, and suggests your first move.

## What's inside

```text
.claude/
  settings.json                  # Claude Code permissions + plugins
  skills/start/SKILL.md          # Claude first-run interview
  skills/ui-ux-pro-max/SKILL.md  # screen and UX review
  skills/skill-creator/SKILL.md  # turn repeated process into a skill
  skills/claudex-sync/SKILL.md   # keep Claude/Codex handoffs aligned
  skills/devils-advocate/SKILL.md # pushback and review pass
  skills/trigger-dev-automation-builder/SKILL.md # small automations
skills/
  *.md                           # Codex-readable versions of the starter skills
prompts/
  codex-start.md                 # first prompt for Codex users
docs/
  choose-your-agent.md           # Claude Code vs Codex
  skills.md                      # what each starter skill does
CLAUDE.md                        # Claude Code project brain
AGENTS.md                        # Codex project brain
HANDOFF.md                       # session continuity
.env.example                     # env var template
```

## The five starter skills

- **Superpowers** - brainstorm, plan, test, debug, and execute without guessing.
- **UI/UX Pro Max** - review screens and improve app usability.
- **Skill Creator** - turn a repeated process into a reusable skill.
- **ClaudexSync** - keep Claude Code and Codex aligned through `HANDOFF.md`.
- **Devils Advocate** - challenge weak assumptions before you ship.

Superpowers is installed through the Claude Code plugin settings. The other
starter skills are included directly in this repo for Claude Code and Codex.

## Day 6 automation skill

- **Trigger.dev Automation Builder** - turn one repeated workflow into a small
  safe Trigger.dev automation. It teaches the AI to map the trigger, action,
  destination, test, required tools, and secrets before building.

## Going further

This kit gets you 80% of the way.

The other 20% - connecting Supabase, Vercel, building real features, debugging
when things go sideways, writing deeper custom skills - is inside **AI Kreator
Academy**.

Join AKA: https://www.skool.com/aka

## License

MIT
