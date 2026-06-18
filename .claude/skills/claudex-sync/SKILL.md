---
name: claudex-sync
description: Keep Claude Code and Codex aligned by updating HANDOFF.md before switching agents or ending a session.
---

# ClaudexSync

Use this workflow when switching between Claude Code and Codex, or when ending
a session that another agent may continue.

## Goal

Keep the two agents from acting like separate brains.

## What To Do

1. Read `HANDOFF.md`.
2. Summarize current state in plain language.
3. Update `HANDOFF.md` with:
   - current state
   - last action
   - next step
   - open questions
4. Mention any files changed in this session.
5. Keep the handoff under 800 tokens.

## Rule

The handoff should help the next agent continue immediately. Do not turn it
into a long diary.
