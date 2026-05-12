# Prompt 01: me.md corrections

**Use case**: You've been chatting with Claude all week. Somewhere in those chats, you corrected Claude. "Actually I don't prefer that." "No, write it shorter." "I never use that phrase." Each correction is a signal. This prompt extracts every correction and gives you the lines to add to your `me.md`.

**When to run**: Sunday, item 1 of the weekly review. After your full week of chats has happened.

## The prompt

```
Look at my last 7 days of Claude conversations. Identify every place I corrected you, pushed back on a suggestion, or said "actually I prefer X." List each correction as a one-line statement I could add to my me.md file. Group them by category: voice, preferences, dislikes, working style, goals.

For each line, include a one-word source tag in brackets at the end so I know which area it came from. For example: "I prefer short hooks over long ones [voice]."

If a correction came up more than once during the week, mark it as a strong pattern with a star at the end.
```

## How to use the output

1. Read the list. Each line is a candidate `me.md` addition.
2. For starred lines (came up 3+ times), add them word-for-word. Those are the patterns.
3. For single occurrences, decide if they're real preferences or one-off moods. Add the real ones, skip the moods.
4. Open `me.md`. Paste the new lines in the right section. Save.

## Customize

If you're running this inside a Claude Project where your `me.md` is already loaded as project knowledge, add this line to the end of the prompt:

```
Skip any correction that's already covered in the current me.md.
```

If you want only the strongest patterns (3+ occurrences), add:

```
Only include lines where I corrected the same thing at least 3 times this week.
```

## Example output (truncated)

```
Voice
- I prefer short hooks over long, multi-clause openers [voice]
- I don't use em dashes anywhere, including in lists [voice] *
- I avoid the word "recently" in personal context [voice]

Preferences
- I want concrete takeaways at the end of every script [preferences] *
- I prefer one specific example over three generic ones [preferences]

Working style
- I work in batched recording days, not daily filming [working style]
```

The starred lines are the ones worth adding first.
