# fable5-mindset

A Claude Code skill that makes Claude Opus 4.8 think and act like Claude Fable 5: outcome-first communication, autonomous execution, readable prose, disciplined tool use, and careful handling of irreversible actions.

## Install

### Via plugin marketplace (recommended)

In Claude Code:

```
/plugin marketplace add JustinasLa/fable5-mindset
/plugin install fable5-mindset@fable5-mindset
```

### Manual

Copy the skill folder into your skills directory:

```
# personal (all projects)
~/.claude/skills/fable5-mindset/SKILL.md

# or per-project
.claude/skills/fable5-mindset/SKILL.md
```

(The skill file lives at `skills/fable5-mindset/SKILL.md` in this repo.)

## Use

Invoke it in a session:

```
/fable5-mindset
```

Claude will also load it automatically when you ask it to "act like Fable 5" or adopt the Fable 5 working style.

## What it changes

- Answers lead with the outcome, not the process.
- Works autonomously — no "Shall I…?" before reversible steps that follow from your request.
- Prose stays readable: full sentences, no shorthand or arrow chains.
- Confirms before irreversible or outward-facing actions; reports failures honestly.
- Code comments only where the code can't speak for itself.

Say "stop fable mode" to revert.
