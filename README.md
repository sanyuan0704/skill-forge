# Skill Forge

A comprehensive guide for creating high-quality Claude Code skills, distilled from analyzing 20+ top-ranked skills on [skills.sh](https://skills.sh).

## Why

Most skills are low-quality slop. But the top-ranked ones share 12 proven techniques that dramatically improve output quality, consistency, and reliability. Skill Forge teaches all 12.

## 12 Techniques Covered

| # | Technique | What It Does |
|---|-----------|-------------|
| 1 | Progressive Loading | Keep SKILL.md under 500 lines, load references on demand |
| 2 | Keyword Bombing | Write descriptions that actually trigger your skill |
| 3 | Workflow Checklist | Give the model a trackable path with ⚠️/⛔ markers |
| 4 | Script Encapsulation | Wrap deterministic operations in scripts (zero context cost) |
| 5 | Question-Style Instructions | Ask specific questions instead of giving vague directives |
| 6 | Confirmation Gates | Force the model to stop and ask before critical operations |
| 7 | Pre-Delivery Checklist | Concrete, verifiable checks before output |
| 8 | Parameter System | `$ARGUMENTS`, `--flags`, partial execution, `--quick` mode |
| 9 | Reference Organization | Organize by domain, not by type — load only what's needed |
| 10 | CLI + Skill Pattern | Replace MCP Servers with CLI tools (93% less context) |
| 11 | Iron Law | One unbreakable rule that prevents the model's #1 mistake |
| 12 | Anti-Pattern Documentation | Explicitly list what NOT to do |

## Install

```bash
npx skills add sanyuan0704/skill-forge
```

## Usage

```
/skill-forge
```

Then follow the guided workflow. The skill walks you through every step from understanding requirements to packaging.

## Structure

```
skill-forge/
├── SKILL.md                          # Core workflow (247 lines)
├── scripts/
│   ├── init_skill.py                 # Initialize new skill from template
│   ├── package_skill.py              # Package skill into .skill file
│   └── quick_validate.py             # Validate skill structure
└── references/
    ├── description-guide.md          # Keyword bombing technique
    ├── workflow-patterns.md          # Checklists, confirmation gates, pre-delivery
    ├── writing-techniques.md         # Question prompting, iron laws, anti-patterns
    ├── architecture-guide.md         # Progressive loading, scripts, CLI+Skill
    ├── parameter-system.md           # $ARGUMENTS, flags, partial execution
    └── output-patterns.md            # Templates, examples, delivery checklists
```

## Related

Based on the article: [研读 20+ 个热门 Skills 之后，我发现了这些写优质 Skill 的套路](https://mp.weixin.qq.com/s/xxx)

## License

MIT
