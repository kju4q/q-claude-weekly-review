# First time running this? Read this first.

Your first Sunday is different. You don't have a `me.md` yet, your Projects sidebar is whatever it is, and you don't have context files to clean.

For run 1, modify the [`CHECKLIST.md`](CHECKLIST.md) like this:

## Item 1: Update your me.md → Create your me.md

Skip the "find your corrections" version. Create your first `me.md` from scratch instead.

Run this prompt:

```
Based on our conversations together so far, what would you say I care about, how I work, and what I'm building? Draft the first version of a me.md file for me, organized into these sections:

1. Who I am (role, what I'm building, where I'm based if relevant)
2. What I'm working on (current focus, active projects)
3. My voice and preferences (how I write, what tone I prefer, banned phrases or styles)
4. What I'm avoiding (topics, formats, or framings I push back on)
5. How I work (the rhythm, the tools, the time blocks)

Use specific evidence from our chats. Don't generalize. If you don't have enough signal for a section, say "needs more data" rather than guessing.
```

Save the output as `me.md` somewhere you'll actually find it again. For Claude.ai users: paste it into the project knowledge of your main Claude Project. For Claude Code users: drop it at the root of your main work directory.

**Time**: 10 minutes on run 1 (twice as long as a normal run, because you're starting from zero)

## Item 2: Archive completed Projects → Do it lightly

Just glance at your Projects sidebar. Don't archive aggressively on run 1. You don't have enough signal yet to know what's truly dormant versus what's paused-but-real.

If anything is obviously done (shipped, abandoned, no clear connection to current work), archive it. Otherwise leave it.

**Time**: 2 minutes

## Item 3: Synthesis → Do it as written

This is the highest-value item for first-timers. Pick one of the three synthesis prompts in [`prompts/`](prompts/) and run it. The output will surface patterns you didn't know existed.

If you're not sure which one, start with [`prompts/03a-synthesis-circling.md`](prompts/03a-synthesis-circling.md). It's the most useful for someone who's never done a synthesis before.

**Time**: 5 minutes

## Item 4: Clean your context files → Do it as written

You may only have one file (`me.md`, which you just created) and that's fine. Run [`prompts/04-context-files-audit.md`](prompts/04-context-files-audit.md) on it.

If you don't have any context files yet at all, skip this item and come back to it on week 2.

**Time**: 3 minutes

## Item 5: Plan a new slash command → SKIP this run

The slash command ideas come from noticing patterns. You need at least 2 weeks of patterns before you can spot them. Skip this on run 1 and come back to it on week 2.

---

## Total time for run 1

20-25 minutes. Slightly longer than a normal run because you're building the foundation.

Run 2 onward: 15 minutes flat.

## Why the modifications

The full checklist assumes you already have a `me.md` and a sidebar full of Projects. Run 1 assumes you don't. The modified version sets up the inputs the normal weekly ritual depends on.

## After run 1

Next Sunday, run the full [`CHECKLIST.md`](CHECKLIST.md) as written. You'll have a `me.md` to update, a sidebar to clean, and a week's worth of chats to synthesize.

Welcome to the system.
