# lhnhidev-skill

A personal collection of AI skills I build for my own workflows. Each skill packages instructions (and optionally scripts or reference files) so an AI assistant such as Claude Code can perform a specific task consistently.

> This repo is tailored to my own needs. Feel free to browse or borrow ideas, but expect skills to reflect my personal preferences and setup.

## What is a skill?

A skill is a folder containing a `SKILL.md` file with YAML frontmatter (`name`, `description`) followed by instructions. The AI loads a skill when its `description` matches the task at hand.

```
skill-name/
├── SKILL.md        # Required: frontmatter + instructions
├── scripts/        # Optional: helper scripts
└── references/     # Optional: supporting docs and templates
```

## Skills

| Skill | Description |
| ----- | ----------- |
| _None yet_ | Skills will be listed here as they are added. |

## Installation

Copy (or symlink) a skill folder into your Claude Code skills directory:

```bash
# Personal skills (available in all projects)
cp -r <skill-name> ~/.claude/skills/

# Or project-level skills
cp -r <skill-name> <your-project>/.claude/skills/
```

Restart the session if the skill does not show up right away.

## Adding a new skill

1. Create a folder named after the skill in kebab-case.
2. Add a `SKILL.md` with a clear `name` and a specific `description` that states when the skill should trigger.
3. Keep instructions concise and actionable; move long material into `references/`.
4. Test it on a real task, then add it to the table above.

## License

Personal use. No license has been specified yet.
