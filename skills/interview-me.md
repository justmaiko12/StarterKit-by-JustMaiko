# Interview Me

Use this workflow when your project idea is still messy and you need the AI to
help you figure out what you actually want before building.

## When To Use

- You have a rough idea, but not a clear version one.
- You are not sure who the project is for.
- You are not sure what the project should include.
- You feel tempted to ask the AI to build before the scope is clear.
- You want the AI to ask better questions before writing code.

## Beginner Rule

Do not start by asking for the full app.

Start by asking the AI to interview you one question at a time. The questions
are part of the build process because they help the AI avoid building the wrong
thing.

## Flow

1. Describe the rough idea in normal language.
2. Ask the AI to use the Interview Me workflow.
3. The AI should state its current guess and confidence level.
4. The AI should ask one focused question at a time.
5. Each question should include the AI's best guess, so you can correct it
   faster.
6. When the idea is clear, ask the AI to summarize:
   - what you are building
   - who it is for
   - what version one includes
   - what can wait until later
   - what is out of scope
7. Turn that summary into a simple PRD before building.

## Starter Prompt

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

## Rule

If the AI cannot explain the project clearly, it is too early to build. Keep
interviewing until the version one project is simple enough to describe.
