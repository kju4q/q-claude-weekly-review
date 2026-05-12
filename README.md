# Your Claude Weekly Review

A 15-minute ritual you run every Sunday so next week's Claude starts smarter than this week's did.

> The difference between using Claude and having an AI co-founder is whether you maintain your context or not. This is the maintenance.

## Who this is for

You use Claude regularly. You've felt the gap between "Claude knows what I'm working on this morning" and "Claude has forgotten everything by Friday." You don't want to keep retyping the same context. You want compounding instead.

This checklist is the smallest weekly ritual that closes that gap. It takes 15 minutes. You run it on Sunday so Monday morning's Claude is already up to date.

## How to use this doc

Read the intro to each item, run the prompt, save the output where the item tells you to save it. The whole thing fits in one Claude session. Open one Project (or one chat), work through all 5 items, close when done.

Total time: 15 minutes once you've done it 2-3 times. First time, give it 25-30. The friction drops fast.

---

## 1. Update your me.md

**What to do**: Skim your past week's Claude chats. Find the corrections you made (where you told Claude "no, I prefer X" or "actually I don't do that"). Add those corrections to your `me.md` file.

**Why it matters**: Every correction you make in a chat dies when the chat ends. Every correction you write into `me.md` becomes a default for every future chat. Once is a fix. Twice is a pattern. Three times is a `me.md` line.

`me.md` is where your AI co-founder learns who you actually are, beyond what's on your LinkedIn or your bio. After 4 weeks of maintenance, this file is more accurate about your working style than anyone else in your life including you.

**Prompt to run**:

```
Look at my last 7 days of Claude conversations. Identify every place I corrected you, pushed back on a suggestion, or said "actually I prefer X." List each correction as a one-line statement I could add to my me.md file. Group them by category: voice, preferences, dislikes, working style, goals.
```

If you're running this in a Claude Project that already has your `me.md` loaded, also add: "Skip any correction that's already covered in the current me.md."

**Time**: 5 minutes (3 to read the output, 2 to copy the new lines into your file)

**What most people skip**: They notice the corrections in real time and feel like they'll remember. They won't. The whole point of this ritual is that you don't have to remember. Capture, file, move on.

---

## 2. Archive completed Projects

**What to do**: Open your Claude sidebar. Look at every Project (or saved chat / starred conversation, depending on which Claude product). Anything that's done? Archive it. Anything that's been dormant for 3+ weeks with no clear next step? Archive it.

**Why it matters**: A cluttered sidebar slows down which version of yourself opens Claude. If you have 12 Projects, you spend 30 seconds picking. If you have 3, you click and start working. The 30 seconds compounds across the year into hours of decision tax.

This is also a forcing function for finishing. Projects that have been "almost done" for a month aren't almost done. Archive them. If they matter, they come back. If they don't, you got the closure.

**Prompt to run** (optional, for inventory before you archive):

```
Here are the titles of all my current active Projects: [paste list]. Group them into: actively shipping this week, paused but real, and zombie (no clear next step). For the zombies, suggest a one-line decision: archive, ship in 2 hours, or convert to a different project.
```

**Time**: 3 minutes

**What most people skip**: They keep "in case I need it later" Projects forever. You won't need it later. If you do, you'll remember the context fast enough to rebuild it. Clutter is more expensive than rebuild cost.

---

## 3. Run a synthesis prompt on your week

**What to do**: Ask Claude to look at the patterns across your past week of chats and tell you what you're actually working on, what you keep avoiding, and what's been silently consuming your time.

**Why it matters**: You think you know what you spent the week on. You're wrong about a third of it. The chats are the ground truth. A synthesis prompt surfaces the gap between what you said you'd focus on and what you actually focused on.

The output is uncomfortable in a useful way. You see the topic you've been circling without committing to. You see the meeting prep you keep redoing instead of automating. You see the friction points worth fixing.

**Prompts to run** (pick the one that fits your week, or run all three):

```
Synthesis: Look at my last 7 days of chats with you. What topics have I been circling without committing to? What's the recurring friction I keep solving the same way instead of fixing once?
```

```
Pattern detection: Across my last week, where did I spend the most time? Where did I make the most progress? Where's the gap between those two answers, and what does that gap suggest about what I should change next week?
```

```
What I'm avoiding: Look at the questions I've asked you this week. What hard question have I been avoiding asking? What would happen if I asked it now?
```

**Time**: 5 minutes (1 to run, 4 to actually sit with the output)

**What most people skip**: They run the prompt and don't write down what surfaced. The whole value is in the writing-down. Open a note, capture the 1-2 lines that hit hardest, decide what changes next week because of it.

---

## 4. Clean your context files

**What to do**: Open every context file you maintain. For most builders this is some combination of: `me.md`, a voice file or `voice.md`, a conventions file, skill files (if you're using Claude Code or skill folders), and any project-specific context docs.

Read each one top to bottom. Anything stale? Rewrite it. Anything missing that you noticed yourself explaining to Claude multiple times this week? Add it. Anything contradictory between files? Reconcile.

**Why it matters**: Context files are the highest-leverage code you'll ever write. One line in a context file replaces one paragraph of typed context every chat for the next year. Maintain them like the infrastructure they are.

Stale context is worse than no context. If your `me.md` still says you're working on a project you shipped two months ago, Claude is making decisions based on a version of you that doesn't exist.

**Prompt to run** (per file):

```
Here's my current [me.md / voice.md / etc]: [paste file]. Read it and tell me: which lines feel out of date given my actual chats this week? Which lines contradict each other? What's missing that I clearly care about based on how I've been talking to you?
```

**Time**: 7 minutes for the full sweep (assuming 3-4 context files of moderate length)

**What most people skip**: They never look at these files between major events. The files quietly become fossils. The ritual is the fix.

**Going deeper**: If you want to see what a serious context-file system looks like, the [q-claude-projects repo](https://github.com/kju4q/q-claude-projects) has examples of the structure. The pattern translates to whatever AI tool you use.

---

## 5. Plan one new slash command

**What to do**: Look at your past week. What did you do manually 3+ times that should have been automated? Write the command for it. Drop it in `.claude/commands/` (if you're on Claude Code) or save it as a reusable prompt template (if you're on web or mobile Claude).

**Why it matters**: A slash command is a one-line investment that pays off forever. If you find yourself typing the same 200 words of instructions every time you draft a script, that's not work. That's friction you forgot to remove.

This is the compounding habit that turns Claude from a tool into a system. Each Sunday adds one command. After a year you have 52 personal automations.

**Prompt to run**:

```
Across my last week of chats, what's a task I gave you more than once where the instructions were almost identical each time? Write me a slash command spec for it: the trigger word, what context files it should read first, the output format I want, and any voice rules to apply. Keep it short enough to live as a single .md file.
```

**Time**: 5 minutes (2 to identify, 3 to draft the command)

**What most people skip**: They wait until they have a "good enough" idea for a command. The good ideas come from running this ritual, not from waiting for inspiration. Run the prompt, write the command, ship it. Iterate next week.

---

## First-time running this? Read this.

Your first Sunday is different. You don't have a `me.md` yet, your Projects sidebar is whatever it is, and you don't have context files to clean.

For run 1, do this instead:

1. **Skip item 1.** Create your first `me.md` from scratch. Use this prompt:
   ```
   Based on our conversations together so far, what would you say I care about, how I work, and what I'm building? Draft the first version of a me.md file for me, organized into: who I am, what I'm working on, my voice and preferences, what I'm avoiding.
   ```

2. **Do item 2 lightly.** Just glance at your Projects. Don't archive aggressively on run 1. You don't have enough signal yet.

3. **Do items 3 and 4** as written. These are the highest-value items for first-timers.

4. **Skip item 5** for run 1. Wait until you've done the ritual twice. The slash command ideas come from noticing patterns, and you need 2 weeks of patterns before you can spot them.

Total time for run 1: 20 minutes. Run 2 onward: 15 minutes.

---

## What success looks like after a month

You run this every Sunday for 4 weeks. By the end:

- Your `me.md` is genuinely accurate. Claude stops making the same wrong assumption about you.
- Your sidebar has 3-4 active Projects, not 12.
- You've shipped 1-2 changes to how you work based on the synthesis prompts.
- Your context files are clean and current.
- You have 2-3 personal slash commands you use multiple times a week.

None of these are dramatic individually. The compounding is dramatic. Most people get more value from this ritual than from any single Claude feature, because the ritual is what makes the features compound.

---

## Going deeper

If you want to see how this fits into a full AI operating system, here's where to go:

- **Setting up Claude Projects properly**: [q-claude-projects repo](https://github.com/kju4q/q-claude-projects). The Builder/Creator/Strategist split, with starter context files for each.
- **Building artifacts that persist across chats**: [q-claude-artifacts repo](https://github.com/kju4q/q-claude-artifacts). Three working examples (journal, CRM, shared reading log) you can fork and run.
- **Claude Code setup with custom slash commands**: [q-claude-code-setup repo](https://github.com/kju4q/q-claude-code-setup). Statusline, /resume, and a custom /script command.
- **Synthesis prompt library**: [synthesis-prompt-library repo](https://github.com/kju4q/synthesis-prompt-library). 20+ prompts for running deeper analysis on your own chat history.

The whole point is that one Sunday at a time, your Claude becomes more yours. Keep going.

---

## See you next Sunday

Put this checklist on your calendar. Sunday, 15 minutes, recurring. The habit IS the system.

If you run this for a month and want to tell me how it went, send a DM. I read them all.

Made by [@qbuilder](https://tiktok.com/@qbuilder) on TikTok, [@qendresahhoti](https://instagram.com/qendresahhoti) on Instagram.

If this saved you time, the carousel that introduced it is the canonical source. Sharing it is the whole point.
