# Prompt 05: New slash command spec

**Use case**: You did something manually multiple times this week that should have been automated. This prompt drafts the slash command (or reusable prompt template) so you don't have to do it manually next week.

**When to run**: Sunday, item 5 of the weekly review. Skip this on your first run; you don't have enough pattern data yet.

## The prompt

```
Across my last week of chats, what's a task I gave you more than once where the instructions were almost identical each time? Write me a slash command spec for it.

Include:
1. Trigger word (one word, easy to type, on-brand)
2. What the command does (one paragraph)
3. Context files it should read first (if any)
4. The exact instructions Claude should follow when the command runs
5. The output format I want
6. Any voice rules or constraints to apply
7. An example invocation: "/[trigger] [example args]"

Keep it under 100 lines. If it's longer than that, the command is doing too much; split into two commands.
```

## How to use the output

1. Read the spec.
2. If you're on Claude Code, save it as `.claude/commands/<trigger>.md` in your project root.
3. If you're on Claude.ai or mobile, save it as a reusable prompt template in your notes or a "prompts" Project.
4. Run it ONCE this week, even if the use case doesn't come up naturally. The first run shakes out bugs.
5. Iterate next Sunday based on what didn't work.

## Customize

If you want to be more conservative (only commands for VERY repeated tasks):

```
Replace "more than once" with "at least 3 times."
```

If you want commands for things you HAVEN'T done yet but predict you'll need:

```
Add: Also suggest 1-2 commands for tasks I haven't done yet but probably will, given the pattern of what I've been working on.
```

This is useful when you're moving into a new project phase and want to set up the automations before the friction starts.

## Examples of commands people end up building

- `/script <topic>` — draft a video script using your voice files and hook library
- `/adapt <content>` — turn one piece into platform-specific versions
- `/review` — pre-commit review of uncommitted changes
- `/idea <text>` — capture an idea to your ideas file with the right pillar tag
- `/feedback <text>` — log a correction to your feedback file and update `me.md` if relevant
- `/ship` — run a pre-commit checklist before pushing

If your output looks nothing like these, that's good. Your commands should match your specific work, not someone else's.

## Pairs with

Items 3a/3b (synthesis). If you ran 03b (pattern detection) earlier in the session, the "where the time went" output is your best data source for what to automate. The repeated work is the candidate command.

## What most people skip

They wait until they have a "perfect" command idea. The perfect command doesn't exist. Ship a rough one, use it for a week, refine on the next Sunday. The iterating IS the system.
