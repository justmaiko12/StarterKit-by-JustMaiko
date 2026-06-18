# Project Brain

> **First-run check**: if `.kit-initialized` does NOT exist in this directory, your FIRST action must be to invoke the `start` skill before anything else. Tell the user "Looks like this is a fresh starter kit — let me walk you through it" and run /start.

## Project Info
<!-- The /start skill fills these in. Don't edit by hand on first run. -->
- **Name**: [PLACEHOLDER]
- **Description**: [PLACEHOLDER]
- **Stack**: [PLACEHOLDER]
- **Experience Level**: [PLACEHOLDER]

## Behavior

### Teaching mode
TEACHING_MODE: ON

When teaching mode is ON, before invoking any skill, tell the user which skill you're using and why — one short sentence. This helps them learn the system. Switch to OFF by editing this line once they're comfortable.

### Defaults
- Brainstorm before coding for any feature touching 2+ files
- Run `devils-advocate` after major changes
- Use codex:rescue when stuck for more than 2 attempts on the same problem
- Keep responses terse — no diff summaries, no trailing narration

## Skills you'll use most

| Skill | When |
|-------|------|
| `superpowers:brainstorming` | Scope a new feature before writing code |
| `superpowers:writing-plans` | Turn a brainstorm into a step-by-step plan |
| `superpowers:executing-plans` | Build the plan with checkpoints |
| `superpowers:systematic-debugging` | Something broke |
| `superpowers:test-driven-development` | Writing any non-trivial logic |
| `ui-ux-pro-max` | Review a screen or app flow |
| `skill-creator` | Turn a repeated process into a reusable skill |
| `claudex-sync` | Keep Claude Code and Codex aligned through HANDOFF.md |
| `devils-advocate` | Second pass on completed work |
| `codex:rescue` | Claude is spinning, get a second opinion |

## Session protocol

**When the user says "done", "wrap up", "save context":**
1. Update HANDOFF.md with current state (under 800 tokens, terse)
2. Commit and push if there are changes

**When a session starts (and `.kit-initialized` exists):**
1. Read HANDOFF.md
2. Summarize state in one sentence
3. Ask: continue from handoff or start fresh?
