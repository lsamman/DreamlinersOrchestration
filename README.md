# DreamlinersOrchestration

A Claude Code skill: **Fable orchestrates, Opus / Sonnet / Haiku execute, and tokens are spent only where they help.**

Fable (the main session) plans the work, splits it, briefs each helper, reviews every result, and alone commits and merges. Opus takes the hard reasoning, Sonnet standard building and writing, Haiku repetitive bulk work. Work starts on the cheapest model that can do it and moves up a tier only after a failure. Briefs point at files instead of pasting them; reports are one line per file changed.

The skill itself is [`skills/DreamlinersOrchestration/SKILL.md`](skills/DreamlinersOrchestration/SKILL.md).

## Install

For every project (once per machine):

```sh
mkdir -p ~/.claude/skills/DreamlinersOrchestration && curl -fsSL https://raw.githubusercontent.com/lsamman/DreamlinersOrchestration/main/skills/DreamlinersOrchestration/SKILL.md -o ~/.claude/skills/DreamlinersOrchestration/SKILL.md
```

For one project only, put the same file at `.claude/skills/DreamlinersOrchestration/SKILL.md` inside that repo and commit it.

Or tell Claude in any chat: *"install the DreamlinersOrchestration skill from lsamman/DreamlinersOrchestration"*.

## Use

Run `/DreamlinersOrchestration` on a task with real parts to split, or let Claude pick it up on its own. For Fable to hold the orchestrator seat, the session should run on Fable: `/model claude-fable-5-2` with `/advisor fable`.

MIT licensed.
