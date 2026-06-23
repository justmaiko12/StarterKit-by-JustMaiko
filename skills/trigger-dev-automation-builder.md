# Trigger.dev Automation Builder

Use this workflow when you want to turn a repeated task into a small automation
with Trigger.dev.

## When To Use

- You repeat the same creator or business task often.
- You want a workflow to run in the background.
- You need a safer plan before connecting APIs, tokens, or private data.
- You want Codex or Claude Code to build the smallest testable automation.

## Beginner Rule

Do not start by asking for code.

Start by describing the repeated task in normal language, then ask the AI to
map the smallest safe automation.

## Flow

1. Describe the repeated task.
2. Ask the AI to map the trigger, action, destination, and test.
3. Ask what tools, accounts, files, and secrets are needed.
4. Ask whether Trigger.dev is the right path, or whether an MCP connector, API,
   CLI, or computer-use workflow is simpler.
5. Approve only the smallest safe version.
6. Let the AI add Trigger.dev to the project if needed.
7. Let the AI build one test task.
8. Run one safe test and inspect the result.
9. Improve one thing only after the first loop works.

## Starter Prompt

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

## Build Prompt

Use this only after approving the plan:

```text
Build the smallest testable version of this automation with Trigger.dev.

Keep it beginner-friendly. Do not add extra features yet. If commands are
needed, run them or explain them in plain English. Tell me what changed, what I
need to provide privately, and how to run one safe test.
```

## Safety Rules

- Never paste API keys, bot tokens, passwords, or private keys into chat.
- Never show secrets in screenshots, recordings, commits, or shared docs.
- Ask the AI where secrets belong, then paste them privately in the right local
  env file or dashboard.
- Use a test account, test database, or test row before touching important data.
- Stop after one loop works. Do not add five more steps on the first pass.

## Good First Automations

- Save a messy content idea into Notion, Google Sheets, or Excel.
- Turn a form submission into a clean tracker row.
- Summarize a safe test email and save the key details.
- Turn a video transcript into research notes.
- Send yourself a reminder when a status changes.

## Done Criteria

- The trigger, action, destination, and test are clear.
- Secrets are handled privately.
- One safe test has run.
- The result is visible in the destination.
- The next improvement is one small change, not a rebuild.
