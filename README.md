# fable5-mindset

A Claude Code plugin that makes Claude Opus 4.8 think and act like Claude Fable 5: outcome-first communication, autonomous execution, readable prose, disciplined tool use, and careful handling of irreversible actions.

## Installation

### Plugin marketplace (recommended)

In Claude Code:

```
/plugin marketplace add JustinasLa/fable5-mindset
/plugin install fable5-mindset@fable5-mindset
```

Then run `/reload-plugins` (or restart Claude Code) to apply.

### Manual

Copy the skill folder into your skills directory:

```
# personal (all projects)
~/.claude/skills/fable5-mindset/

# or per-project
<your-project>/.claude/skills/fable5-mindset/
```

The skill file lives at [`skills/fable5-mindset/SKILL.md`](skills/fable5-mindset/SKILL.md) in this repo.

## Usage

Invoke it in a session:

```
/fable5-mindset
```

Claude also loads it automatically when you ask it to "act like Fable 5" or adopt the Fable 5 working style.

Say "stop fable mode" or "normal mode" to revert.

## What it changes

- **Outcome-first answers.** The first sentence tells you what happened or what was found; reasoning comes after.
- **Autonomous execution.** No "Shall I…?" before reversible steps that follow from your request; the turn ends only when the task is done or blocked on you.
- **Readable prose.** Full sentences, no shorthand, abbreviations, or arrow chains; output stays short by being selective, not compressed.
- **Care with irreversible actions.** Confirms before publishing, deleting, or deploying; inspects targets before overwriting; reports failures honestly.
- **Code discipline.** Code matches surrounding style; comments only where the code can't speak for itself; changes verified end-to-end.
- **Tool discipline.** Dedicated tools over shell equivalents, parallel independent calls, clickable `file:line` references.

## Repository structure

```
.claude-plugin/
  plugin.json        # plugin manifest
  marketplace.json   # marketplace listing
skills/
  fable5-mindset/
    SKILL.md         # the skill itself
```

## Contributing

Issues and pull requests are welcome. If you spot a behavior the skill should encourage (or a default habit it should suppress), open an issue describing the before/after.

## License

[MIT](LICENSE)
