# Codex Project Brain

## First-Run Check

If `.kit-initialized` does not exist in this directory, your first action must
be to run the Codex starter interview from `prompts/codex-start.md`.

Tell the user:

```text
Looks like this is a fresh starter kit. I will walk you through four quick questions first.
```

Ask one question at a time, update the Project Info section below, then create
`.kit-initialized`.

## Project Info

<!-- The Codex starter interview fills these in. Do not edit by hand on first run. -->
- **Name**: [PLACEHOLDER]
- **Description**: [PLACEHOLDER]
- **Stack**: [PLACEHOLDER]
- **Experience Level**: [PLACEHOLDER]

## Behavior

### Teaching Mode

TEACHING_MODE: ON

When teaching mode is ON, before using a starter skill or workflow, tell the
user which one you are using and why in one short sentence.

### Defaults

- Brainstorm before coding for any feature touching 2+ files.
- Make the smallest useful change first.
- Explain before editing when the user is new or the task is risky.
- Run `devils-advocate` after major changes.
- Use `claudex-sync` before switching between Claude Code and Codex.
- Keep responses terse and practical.

## Starter Skills

Codex cannot rely on Claude Code slash commands, so use the markdown skill files
in `skills/` as local instructions:

| Skill | File | When |
|-------|------|------|
| Superpowers | `skills/superpowers.md` | Brainstorm, plan, test, debug, execute |
| UI/UX Pro Max | `skills/ui-ux-pro-max.md` | Review a screen or app flow |
| Skill Creator | `skills/skill-creator.md` | Turn repeated instructions into a skill |
| ClaudexSync | `skills/claudex-sync.md` | Keep Claude Code and Codex aligned |
| Devils Advocate | `skills/devils-advocate.md` | Challenge weak assumptions before shipping |

When the user asks for one of these skills, read the matching file and follow it.

## Session Protocol

**When the user says "done", "wrap up", or "save context":**

1. Update `HANDOFF.md` with current state in under 800 tokens.
2. Include what changed, what is next, and any open questions.
3. Commit and push only if the user asked you to publish changes or the repo
   workflow clearly expects it.

**When a session starts and `.kit-initialized` exists:**

1. Read `HANDOFF.md`.
2. Summarize state in one sentence.
3. Ask whether to continue from the handoff or start fresh.
