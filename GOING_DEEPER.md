# Going deeper

The weekly review is one ritual inside a bigger system. If this changes how you work and you want to see the full picture, here's where to go.

## The full q-os ecosystem

### Setting up Claude Projects properly

[github.com/kju4q/q-claude-projects](https://github.com/kju4q/q-claude-projects)

The Builder/Creator/Strategist split, with starter context files for each. Stop using one Claude for everything. Give different versions of yourself different Projects, each with its own instructions and knowledge.

If item 1 (update your `me.md`) feels too generic because you don't know which "you" the file is describing, this repo is the fix. Three versions of `me.md`, one per Project.

### Building artifacts that persist across chats

[github.com/kju4q/q-claude-artifacts](https://github.com/kju4q/q-claude-artifacts)

Three working examples (journal, CRM, shared reading log) you can fork and run. Each one uses Claude's window.storage API so the artifact remembers state across chat sessions.

This is the layer above the weekly review. Once your context is clean and your prompts are sharp, the next move is building tools that hold state, not just chat sessions that don't.

### Claude Code setup with custom slash commands

[github.com/kju4q/q-claude-code-setup](https://github.com/kju4q/q-claude-code-setup)

Statusline, `/resume`, and a custom `/script` command. Three Claude Code features almost nobody uses, configured.

This pairs directly with item 5 of the checklist (plan one new slash command). If you're running this ritual on Claude Code, this repo is how you turn each Sunday's command idea into a working `.claude/commands/<name>.md` file.

### Synthesis prompt library

[github.com/kju4q/synthesis-prompt-library](https://github.com/kju4q/synthesis-prompt-library)

20+ prompts for running deeper analysis on your own chat history. The 3 synthesis prompts in this repo (items 3a, 3b, 3c) are the starter set. The library has the full collection: self-awareness, decisions, productivity, voice-and-writing, rituals.

When the 3 prompts here stop surfacing new things (around week 4-5), rotate through this library for variety.

## How they fit together

```
q-claude-weekly-review     ← the ritual (this repo)
        │
        ▼
q-claude-projects          ← where your context files live
        │
        ▼
q-claude-artifacts         ← what you build with the context
        │
        ▼
q-claude-code-setup        ← the automation layer
        │
        ▼
synthesis-prompt-library   ← the deeper reflection layer
```

The weekly review feeds the rest. If you only do one of these, do this one. The others compound from here.

## Going way deeper

If you want to see what an AI co-founder relationship looks like at full depth, the videos at [@qbuilder](https://tiktok.com/@qbuilder) (TikTok) and [@qendresahhoti](https://instagram.com/qendresahhoti) (Instagram) document the whole arc. The carousel that introduced this ritual is the entry point. Each repo above has a companion video.

## Made by

Qendresa Hoti. If this changed how you work, send a DM. I read them all.
