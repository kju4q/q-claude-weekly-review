# Prompt 04: Context files audit

**Use case**: You maintain context files (`me.md`, voice files, conventions, skill files). They drift. This prompt finds the drift.

**When to run**: Sunday, item 4 of the weekly review. Run it once per file you maintain. Or, if you have a master file (like a CLAUDE.md), run it on that.

## The prompt

```
Here's my current [me.md / voice.md / CLAUDE.md / etc]:

[paste file content]

Read it and tell me:

1. Which lines feel out of date given my actual chats this week?
2. Which lines contradict each other?
3. What's missing that I clearly care about based on how I've been talking to you, but isn't in the file?
4. Which lines could be tightened (too long, too vague, redundant)?

For each issue, suggest the specific rewrite. Don't just flag the problem.
```

## How to use the output

1. Open the file in your editor.
2. Apply the rewrites you agree with. Skip the ones that feel off.
3. For "missing" items, decide if they belong in this file or a different context file. Sometimes the right answer is "create a new file for this."
4. Commit the change. If you're not on git, at least timestamp the version in a comment at the top.

## Customize

If you want a softer pass (just flag, don't rewrite):

```
Remove the "Don't just flag the problem" line at the end. Sometimes you just want a list to think about.
```

If you have multiple files to audit at once:

```
Replace "Here's my current..." with "Here are my context files:" then list each file with a clear separator. Add at the end: "Treat them as a system, not as individual files. Flag contradictions BETWEEN files, not just within."
```

## What most people skip

They run this prompt and don't apply the changes. The output is a list, not a change. Files only update if you touch them. Apply at least 2 changes per audit, even if they're small.

## Pairs with

Item 1 (update your me.md). If you're updating `me.md` AND running this audit on it, run the audit AFTER the corrections from item 1 are already in. That way you're auditing the freshest version, not last week's.
