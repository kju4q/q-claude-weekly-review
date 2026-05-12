# Prompt 02: Projects inventory

**Use case**: Your Claude sidebar has too many Projects (or starred chats, or saved conversations, depending on which Claude product). You want to archive aggressively but you're not sure what counts as "done" versus "paused-but-real." This prompt does the triage.

**When to run**: Sunday, item 2 of the weekly review. Optional. If you already know what to archive, skip the prompt and just do it.

## The prompt

```
Here are the titles of all my current active Projects (or saved chats):

[paste the list, one per line]

Group them into three buckets:

1. Actively shipping this week (clear next step, real momentum)
2. Paused but real (waiting on something specific, will resume in the next 2-4 weeks)
3. Zombie (no clear next step, no recent activity, unclear if I care anymore)

For each zombie, suggest a one-line decision: archive, ship in 2 hours, or convert to a different project.
```

## How to use the output

1. Bucket 1 stays open. Don't touch them.
2. Bucket 2 stays open but write down the "waiting on" condition somewhere visible (the project itself, or a notes file).
3. Bucket 3 is your archive list. Default to archive unless you can name a specific 2-hour ship.

## Customize

If your Claude products have actual usage data (last opened, message count), include that in your paste. The bucketing gets sharper:

```
Here are the titles of my Projects, with the last time I opened each one:

q-os system design — 2 days ago
burnout app architecture — 11 days ago
random naming brainstorm — 47 days ago
[etc]
```

The 47-day-ago one is almost certainly a zombie. Make the call without ceremony.

## What most people skip

They keep zombies around "in case." You won't need them. If you do, the context rebuilds fast.

## Pairs with

Item 1 of the checklist. After you archive, the surviving Projects are the ones whose `me.md` files most deserve maintenance attention.
