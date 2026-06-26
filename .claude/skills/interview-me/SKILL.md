---
name: interview-me
description: Clarify a messy project idea before building. Use when the user has a rough app, site, dashboard, workflow, or product idea but has not clearly defined the user, goal, version one scope, success criteria, or out-of-scope items.
---

# Interview Me

Use this skill when the user has a rough idea but the version one project is
not clear yet.

## Goal

Help the user figure out what they actually want before you build.

## Beginner Rule

Do not start by writing code.

Interview the user one question at a time until the project is clear enough to
turn into a simple PRD.

## Flow

1. Restate your current best guess of what the user wants.
2. Give a confidence level, like `Confidence: 40%`.
3. Ask one focused question.
4. Include your best guess with the question so the user can correct you
   quickly.
5. Wait for the answer before asking the next question.
6. Keep going until you can clearly explain:
   - outcome
   - user
   - why it matters
   - version one
   - later features
   - out of scope
7. Turn the confirmed answers into a beginner-friendly PRD.

## Starter Prompt To Offer

```text
Use the Interview Me workflow.

My rough project idea is:

[describe the idea in normal language]

Ask me one question at a time. For each question, include your best guess so I
can correct it quickly.

When you are confident, summarize the project as:
- Outcome
- User
- Why this matters
- Version one
- Later features
- Out of scope

Then turn it into a beginner-friendly PRD.
```

## Rules

- Ask one question at a time.
- Attach a guess to each question.
- Do not accept vague words like "modern", "scalable", or "dashboard" without
  asking what they mean for this project.
- Do not build until the version one scope is clear.
- Keep the PRD short enough for a beginner to use.

## Done Criteria

- The project outcome is clear.
- The user is clear.
- Version one is smaller than the original idea.
- Later features are separated from must-haves.
- Out-of-scope items are written down.
