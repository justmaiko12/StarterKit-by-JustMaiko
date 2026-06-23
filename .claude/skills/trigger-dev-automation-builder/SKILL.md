---
name: trigger-dev-automation-builder
description: Plan and build the smallest safe Trigger.dev automation from a repeated workflow. Use when the user wants automations, background jobs, Trigger.dev, scheduled workflows, API workflows, or creator/business tasks that should run without manual repetition.
---

# Trigger.dev Automation Builder

Use this skill when the user wants to turn a repeated task into a small
automation with Trigger.dev.

## Beginner Rule

Do not start by writing code.

Start by asking the user to describe the repeated task in normal language. Then
map the smallest safe automation before changing files.

## Flow

1. Identify the repeated workflow.
2. Map the trigger, action, destination, and first safe test.
3. List required tools, accounts, files, and secrets.
4. Decide whether Trigger.dev is the right path, or whether an MCP connector,
   API, CLI, or computer-use workflow is simpler.
5. Ask the user to approve the smallest safe version.
6. If Trigger.dev is needed, add it to the project using the current
   Trigger.dev setup flow.
7. Build one test task only.
8. Run one safe test and inspect the destination.
9. Suggest one next improvement after the first loop works.

## Starter Prompt To Offer

```text
I want to automate this repeated workflow:

[describe the workflow in normal language]

Use the Trigger.dev Automation Builder workflow.

First, stay in plan mode. Map the trigger, action, destination, and first safe
test. Tell me what tools, accounts, files, and secrets are needed. Tell me
whether Trigger.dev is the right path or if a simpler connector/API/computer-use
workflow makes more sense.

Do not write code yet. Do not ask me to paste secrets into chat.
```

## Build Rule

After the user approves the plan, build the smallest testable version only.

If commands are needed, run them or explain them in plain English. The user
should not have to memorize commands.

## Safety Rules

- Never ask the user to paste API keys, bot tokens, passwords, or private keys
  into chat.
- Never expose secrets in screenshots, recordings, commits, or shared docs.
- Tell the user where secrets belong, then let them paste secrets privately in
  the correct local env file or dashboard.
- Use test data before touching important data.
- Stop after one loop works.

## Good First Automations

- Save a messy content idea into Notion, Google Sheets, or Excel.
- Turn a form submission into a clean tracker row.
- Summarize a safe test email and save the key details.
- Turn a video transcript into research notes.
- Send yourself a reminder when a status changes.

## Done Criteria

- The workflow has a clear trigger, action, destination, and test.
- Secrets are handled privately.
- One safe test has run.
- The result is visible in the destination.
- The next improvement is one small change, not a rebuild.
