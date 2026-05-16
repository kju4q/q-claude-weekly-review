# The Slides, Expanded

The 7 slides from the carousel, plus the thinking behind each one. The slides themselves are short by design (carousels reward brevity). This file is the long version: what I would have said about each slide if I had more room. The procedural version of the ritual lives in [`../CHECKLIST.md`](../CHECKLIST.md). This file is the reasoning.

---

## Slide 1 (cover)

> **your Claude weekly review**
>
> 5 things to check every Sunday so next week starts smarter than this one did
>
> _swipe →_

### What's behind this slide

The cover is doing two jobs in one line. The first job is naming a category that doesn't exist yet: a weekly review for your AI. People run weekly reviews for their work, their projects, their bodies. Almost nobody runs one for the tool they spend the most hours of their day inside. That's the gap this opens.

The second job is the promise of compounding, hidden inside "next week starts smarter." Claude itself isn't getting smarter week to week. The model is the model. What gets smarter is the context Claude reads about you, your goals, your work, your voice. If you maintain that context every week, the curve compounds. If you don't, you start every Monday from where you started last Monday.

Sunday specifically because it's the day most builders have unstructured time and the day right before the work week kicks back in. 15 minutes on Sunday is the lowest-friction window where this ritual actually fits without competing with anything urgent.

Five items because four feels arbitrary and six feels like a project. Five fits in a single Claude session, in 15 minutes, with one round of "wait, what was the next one again" allowed.

---

## Slide 2

> **1. update your me.md**
>
> skim this week's chats, what did Claude get wrong about you, what did you correct more than once, add it
>
> next week, those corrections become defaults

### What's behind this slide

`me.md` is a single markdown file you keep at the root of any Claude Project (or in your Claude Code working directory) that tells Claude who you are. It's not your bio. It's the running document of your preferences, your voice, your goals, the way you work, the things you push back on. After a few months of maintaining it, this file is more accurate about you than anyone else in your life including you.

The reason this is item one: every correction you make in a chat dies when the chat ends. You can be telling Claude "no, I don't write that way" twenty times a week, and on the twenty-first chat, Claude will write that way again because the chat is the unit of memory, not your account. The me.md is what gets you out of that loop.

The rule I use: once is a fix, twice is a pattern, three times is a me.md line. If you've corrected Claude on the same thing three times in a week, that's not a one-off, that's your default preference, and it belongs in the file.

What most people get wrong: they think this is hard. It isn't. You don't write me.md from scratch every week. You read this week's chats, find the corrections, and append them. Five minutes.

---

## Slide 3

> **2. archive completed Projects**
>
> every Project in your sidebar that's done? archive it
>
> less clutter, sharper context, which version of yourself opens which Claude

### What's behind this slide

Your Claude sidebar (or saved chat list, or starred conversations, depending on which Claude product) is where you pick which version of yourself shows up to work. If you have 12 Projects, you spend 30 seconds picking. If you have 3, you click and start. The 30 seconds compounds across the year into hours of decision tax.

The harder reason to archive: keeping zombie Projects around is a form of avoidance. The "almost done" project that's been almost done for a month isn't almost done. Archiving it forces a decision: ship it in 2 hours, or accept that it's not going to happen and move on. Both outcomes are useful. The avoidance state isn't.

What counts as a Project to archive: anything you haven't touched in 3+ weeks AND can't name a specific next step for. That's the zombie filter. If you can name a specific next step ("call so-and-so," "write the X paragraph"), it's paused but real. Leave it.

People keep things "in case I need it later." You won't. If you do, you'll rebuild the context faster than you think. Clutter is more expensive than rebuild cost.

---

## Slide 4

> **3. synthesize your week**
>
> run this prompt: "look at my last 7 days of chats and tell me what i've been circling without committing to"
>
> claude knows what you've been avoiding, let it tell you

### What's behind this slide

You think you know how you spent your week. You're wrong about a third of it. The chats are the ground truth, and a synthesis prompt across a week of chats surfaces patterns you can't see in real time.

The prompt on the slide is the most useful version for builders. It specifically asks for "circling without committing to" because that's the failure mode that's hardest to spot in the moment. You keep returning to the same topic, you keep almost-deciding, you keep generating more analysis instead of more decisions. The synthesis surfaces that pattern in 30 seconds.

The output of this prompt is rarely comfortable. You'll see the topic you've been avoiding. You'll see the friction point you keep solving the same wrong way. You'll see the meeting prep you keep redoing instead of automating. Sit with the output for 60 seconds before doing anything. Then pick ONE thing from it and commit to a decision this week.

If you skip the writing-down part, the synthesis is wasted. The value isn't in knowing what you're circling. The value is in stopping.

If you want a longer prompt library for synthesis variants (pattern detection, what-you're-avoiding, end-of-month reflection), see [`../prompts/`](../prompts/). The slide shows the one I use weekly. The prompts folder shows the rotation.

---

## Slide 5

> **4. clean your context files**
>
> skill files, voice files, conventions, read them, anything stale rewrite it, anything missing add it
>
> your context files compound when you maintain them

### What's behind this slide

Context files are the highest-leverage code you'll ever write. One line in a context file replaces one paragraph of typed context every chat for the next year. Maintain them like the infrastructure they are.

What counts as a context file: your me.md, any voice file or style guide you've written, conventions docs, skill files (if you're on Claude Code), project-specific context docs. Anything you write once and Claude reads many times.

Stale context is worse than no context. If your me.md still says you're working on a project you shipped two months ago, Claude is making decisions based on a version of you that doesn't exist. The file becomes a fossil and the fossil shapes the responses.

The audit prompt: paste each file into Claude and ask "which lines feel out of date given my actual chats this week, which lines contradict each other, what's missing that I clearly care about based on how I've been talking to you." Then apply at least two changes per file. Reading alone isn't the ritual. Editing is.

Most people never look at these files between major events (a job change, a project launch). The files quietly become fossils. The Sunday ritual is the maintenance that prevents this.

---

## Slide 6

> **5. plan one new command**
>
> what did you do manually 3+ times this week that should be a slash command?
>
> write it, drop it in .claude/commands/, next week it runs in one keystroke

### What's behind this slide

A slash command is a one-line investment that pays off forever. If you find yourself typing the same 200 words of instructions every time you draft something, that's not work. That's friction you forgot to remove.

Once a week, you spot one thing you did manually multiple times, and you turn it into a command. After a year, you have 52 personal automations. That's the compounding turn from "I use Claude" to "Claude is part of my system."

Examples of commands people end up building once they start this ritual:

- `/script` for drafting in their voice
- `/adapt` for repurposing one piece into platform versions
- `/review` for pre-commit code review
- `/idea` for capturing ideas to a specific file
- `/feedback` for logging a correction and updating me.md if relevant

Your commands should match your specific work, not someone else's. The reason the ritual surfaces them is that the pattern is in YOUR week. By the time you spot the friction, the command is half-written.

The trap most people fall into: waiting until they have a "perfect" command. The perfect command doesn't exist. Ship rough, use it for a week, refine next Sunday.

If you're on Claude Code, the command file goes in `.claude/commands/<name>.md`. If you're on Claude.ai or mobile, save it as a reusable prompt template in your notes or in a dedicated "prompts" Project. Same principle, different storage.

---

## Slide 7 (CTA)

> do this every Sunday
>
> your Claude gets smarter every week, the compounding is real
>
> comment WEEK for the full checklist as a markdown file
>
> @qbuilder

### What's behind this slide

The ritual works because it compounds. Each Sunday adds one more pattern to your me.md, removes one more zombie from your sidebar, surfaces one thing you've been avoiding, fixes one stale line in a context file, and turns one repeated task into a one-keystroke command.

After 4 weeks, none of those moves looks dramatic. After 4 months, your Claude is unrecognizable compared to where it started. Your me.md is accurate enough that Claude stops making the same wrong assumption about you. Your sidebar has 3-4 active Projects instead of 12. You've shipped 1-2 changes to how you work based on synthesis prompts. Your context files are clean and current. You have 8-10 personal slash commands you use multiple times a week.

The failure mode is skipping. People run this once, feel good, and then forget for 3 weeks. The first run gives you the framework. The compounding only starts at run 4 or 5. Most people quit at run 2 and never see the compounding.

What I'd tell you if we were in the same room: the difference between people who use Claude and people who have an AI co-founder isn't the prompt library. It's whether they spend 15 minutes a week maintaining the context. Everything else is downstream of that.

---

## If you want to go deeper

The slides are the lean version. The reasoning above is the long version. The procedural version (open-Claude, run-this-prompt, save-here) lives in [`../CHECKLIST.md`](../CHECKLIST.md). All three exist because some people want the why (you're here), some want the depth (CHECKLIST), and some want the artifact they screenshot (the carousel itself).

Run it tomorrow. Send me a DM and tell me how it went.
