# skills

Agent skills for any coding agent (Claude Code, Cursor, Codex, Grok, OpenCode, and the rest). Each skill is `skills/<name>/SKILL.md` in the [Agent Skills](https://agentskills.io/) format.

## Install

```bash
npx skills add Nhuengzii/skills
```

The CLI detects installed agents and copies the skills into each one's skills directory. Add `-g` for user-wide install, `--all` to skip prompts.

```bash
npx skills add Nhuengzii/skills -g
npx skills add Nhuengzii/skills --all
npx skills add Nhuengzii/skills --skill dont-paste-the-brief
```

## Skills

| Skill | What it does |
| --- | --- |
| [dont-paste-the-brief](skills/dont-paste-the-brief/) | Before accepting a deliverable: name the job, ban nearby junk, prove with a held-out check. |

## Add a skill

Create `skills/<name>/SKILL.md` with YAML frontmatter (`name`, `description`) and instructions.
