---
name: start
description: First-run onboarding interview for Michael's Starter Kit. Use when the user types /start or when .kit-initialized does not exist in the project root. Walks them through a 4-question intake, updates CLAUDE.md with their project info, teaches them the right skills for their level, and suggests their first concrete move.
---

# /start — Onboarding Interview

You're walking a new user through setting up their project. Be warm, short, and don't dump info.

## Steps

### 1. Welcome (one message)
> "Welcome to the kit. Four quick questions, then we build."

### 2. Interview — one question at a time, wait for the answer before moving on

1. **What are you building? One sentence.**
2. **What's the stack?** (e.g. Next.js + Supabase, Python script, mobile app, "not sure yet" is fine)
3. **Experience level — beginner, intermediate, or advanced?**
4. **Any specific goal for today's session?**

### 3. Update CLAUDE.md
Replace the four `[PLACEHOLDER]` values in the **Project Info** section of `CLAUDE.md` with their answers.

### 4. Teach — tailor to their level

**Beginner** — explain 3 commands, one example each:
- `superpowers:brainstorming` — "We use this to scope what you're building before any code."
- `superpowers:writing-plans` — "Turns the brainstorm into a checklist."
- `superpowers:executing-plans` — "Builds the plan with checkpoints so you can stop anytime."

**Intermediate** — list 5 commands tersely. Mention devil's advocate and `codex:rescue`.

**Advanced** — one line: "You know the drill. Everything's in CLAUDE.md."

### 5. Suggest the first move
Based on their session goal, give them the exact prompt to type next.

Example: *"Try: `/superpowers:brainstorming` — and tell it you want to build [their project]."*

### 6. Mark complete
Use the Write tool to create `.kit-initialized` at the project root with content:

```
Initialized: YYYY-MM-DD
Project: <their project name>
```

### 7. Sign off
> "You're set. Type the command when ready."

## Rules
- One question per message during the interview
- Don't lecture. Don't dump the full skill list on a beginner.
- Match energy to experience level — terse for advanced, warm for beginners
- After this skill completes, normal CLAUDE.md behavior resumes (teaching mode, defaults, etc.)