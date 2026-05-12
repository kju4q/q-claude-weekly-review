# The 5-item Sunday Checklist

Run these in order. One Claude session. 15 minutes once you've done it 2-3 times.

If this is your first time, read [`FIRST_TIME.md`](FIRST_TIME.md) first. The first run skips and modifies a few items.

---

## 1. Update your me.md

**What to do**: Skim your past week's Claude chats. Find the corrections you made (where you told Claude "no, I prefer X" or "actually I don't do that"). Add those corrections to your `me.md` file.

**Why it matters**: Every correction you make in a chat dies when the chat ends. Every correction you write into `me.md` becomes a default for every future chat. Once is a fix. Twice is a pattern. Three times is a `me.md` line.

`me.md` is where your AI co-founder learns who you actually are, beyond what's on your LinkedIn or your bio. After 4 weeks of maintenance, this file is more accurate about your working style than anyone else in your life including you.

**Prompt**: [`prompts/01-me-md-corrections.md`](prompts/01-me-md-corrections.md)

**Time**: 5 minutes (3 to read the output, 2 to copy the new lines into your file)

**What most people skip**: They notice the corrections in real time and feel like they'll remember. They won't. The whole point of this ritual is that you don't have to remember. Capture, file, move on.

---

## 2. Archive completed Projects

**What to do**: Open your Claude sidebar. Look at every Project (or saved chat / starred conversation, depending on which Claude product). Anything that's done? Archive it. Anything that's been dormant for 3+ weeks with no clear next step? Archive it.

**Why it matters**: A cluttered sidebar slows down which version of yourself opens Claude. If you have 12 Projects, you spend 30 seconds picking. If you have 3, you click and start working. The 30 seconds compounds across the year into hours of decision tax.

This is also a forcing function for finishing. Projects that have been "almost done" for a month aren't almost done. Archive them. If they matter, they come back. If they don't, you got the closure.

**Prompt** (optional, for inventory before you archive): [`prompts/02-projects-inventory.md`](prompts/02-projects-inventory.md)

**Time**: 3 minutes

**What most people skip**: They keep "in case I need it later" Projects forever. You won't need it later. If you do, you'll remember the context fast enough to rebuild it. Clutter is more expensive than rebuild cost.

---

## 3. Run a synthesis prompt on your week

**What to do**: Ask Claude to look at the patterns across your past week of chats and tell you what you're actually working on, what you keep avoiding, and what's been silently consuming your time.

**Why it matters**: You think you know what you spent the week on. You're wrong about a third of it. The chats are the ground truth. A synthesis prompt surfaces the gap between what you said you'd focus on and what you actually focused on.

The output is uncomfortable in a useful way. You see the topic you've been circling without committing to. You see the meeting prep you keep redoing instead of automating. You see the friction points worth fixing.

**Prompts** (pick the one that fits your week, or run all three):

- [`prompts/03a-synthesis-circling.md`](prompts/03a-synthesis-circling.md): what you keep circling without committing to
- [`prompts/03b-pattern-detection.md`](prompts/03b-pattern-detection.md): where the time actually went vs. where you thought it went
- [`prompts/03c-what-im-avoiding.md`](prompts/03c-what-im-avoiding.md): the hard question you've been avoiding

**Time**: 5 minutes (1 to run, 4 to actually sit with the output)

**What most people skip**: They run the prompt and don't write down what surfaced. The whole value is in the writing-down. Open a note, capture the 1-2 lines that hit hardest, decide what changes next week because of it.

---

## 4. Clean your context files

**What to do**: Open every context file you maintain. For most builders this is some combination of: `me.md`, a voice file or `voice.md`, a conventions file, skill files (if you're using Claude Code or skill folders), and any project-specific context docs.

Read each one top to bottom. Anything stale? Rewrite it. Anything missing that you noticed yourself explaining to Claude multiple times this week? Add it. Anything contradictory between files? Reconcile.

**Why it matters**: Context files are the highest-leverage code you'll ever write. One line in a context file replaces one paragraph of typed context every chat for the next year. Maintain them like the infrastructure they are.

Stale context is worse than no context. If your `me.md` still says you're working on a project you shipped two months ago, Claude is making decisions based on a version of you that doesn't exist.

**Prompt**: [`prompts/04-context-files-audit.md`](prompts/04-context-files-audit.md)

**Time**: 7 minutes for the full sweep (assuming 3-4 context files of moderate length)

**What most people skip**: They never look at these files between major events. The files quietly become fossils. The ritual is the fix.

---

## 5. Plan one new slash command

**What to do**: Look at your past week. What did you do manually 3+ times that should have been automated? Write the command for it. Drop it in `.claude/commands/` (if you're on Claude Code) or save it as a reusable prompt template (if you're on web or mobile Claude).

**Why it matters**: A slash command is a one-line investment that pays off forever. If you find yourself typing the same 200 words of instructions every time you draft a script, that's not work. That's friction you forgot to remove.

This is the compounding habit that turns Claude from a tool into a system. Each Sunday adds one command. After a year you have 52 personal automations.

**Prompt**: [`prompts/05-slash-command-spec.md`](prompts/05-slash-command-spec.md)

**Time**: 5 minutes (2 to identify, 3 to draft the command)

**What most people skip**: They wait until they have a "good enough" idea for a command. The good ideas come from running this ritual, not from waiting for inspiration. Run the prompt, write the command, ship it. Iterate next week.

---

## What success looks like

You run this every Sunday for 4 weeks. By the end:

- Your `me.md` is genuinely accurate. Claude stops making the same wrong assumption about you.
- Your sidebar has 3-4 active Projects, not 12.
- You've shipped 1-2 changes to how you work based on the synthesis prompts.
- Your context files are clean and current.
- You have 2-3 personal slash commands you use multiple times a week.

None of these are dramatic individually. The compounding is dramatic.

---

## Going deeper

If this ritual changes how you work and you want to see the full system, check [`GOING_DEEPER.md`](GOING_DEEPER.md). The other q-os repos. Where to take this next.

## See you next Sunday

Put this checklist on your calendar. Sunday, 15 minutes, recurring. The habit IS the system.
