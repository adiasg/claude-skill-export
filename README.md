# Claude Skill Export

A Claude skill to export all of its skills to other coding agents. 

This creates a `SKILLS.md` file that contains a manifest of all skills. Feed this into other coding agents, e.g., in `AGENTS.md` ask to read `SKILLS.md`.

## Quickstart

```bash
# Clone this skill
https://github.com/adiasg/claude-skill-export

# Add to your Claude skills
cp -R claude-skill-export/skill-export ~/.claude/skills

# Ask Claude to export skills - it'll make a SKILLS.md file
claude -- "Export all skills"
```

To use the skills with Codex, simply add this line to `AGENTS.md`:
```
Read the SKILLS.md file for loading available skills.
```
