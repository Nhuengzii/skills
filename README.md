# skills

A Grok skills repository. Each subdirectory is one skill (`<name>/SKILL.md`).

Grok loads this folder via `[skills] paths` in `~/.grok/config.toml`.

## Skills

| Skill | Command | What it does |
| --- | --- | --- |
| [dont-paste-the-brief](dont-paste-the-brief/) | `/dont-paste-the-brief` | Before accepting a deliverable: name the job, ban nearby junk, prove with a held-out check. |

## Add a skill

1. Create `<name>/SKILL.md` with YAML frontmatter (`name`, `description`) and instructions.
2. Reload with `/skills` or start a new session.
