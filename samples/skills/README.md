# Sample Skills

Ready-to-use skill templates for GitHub Copilot CLI. Copy any skill folder to start using it immediately.

## Quick Start

```bash
# Copy a skill to your personal skills folder
cp -r hello-world ~/.copilot/skills/

# Or copy to your project for team sharing
cp -r code-review .github/skills/
```

## Available Skills

| Skill | Description | Best For |
|-------|-------------|----------|
| `hello-world` | Minimal example (learning the format) | First-time skill creators |
| `code-review` | Python code review checklist (PEP 8, type hints, validation) | Consistent code reviews |
| `pytest-gen` | Generate comprehensive pytest tests | Structured test generation |
| `commit-message` | Conventional commit messages | Standardized git history |

## How Skills Work

Skills are **automatically triggered** when your prompt matches the skill's `description` field. You don't need to invoke them manually.

```bash
copilot

> Review this code for issues
# Copilot detects this matches "code-review" skill and loads it automatically

> Generate a commit message
# Copilot loads the "commit-message" skill
```

You can also invoke skills directly:
```bash
> /code-review Check books.py
> /pytest-gen Generate tests for BookCollection
> /commit-message
```

## Skill Structure

Each skill is a folder containing a `SKILL.md` file:

```
skill-name/
└── SKILL.md    # Required: Contains frontmatter + instructions
```

The `SKILL.md` file has YAML frontmatter with `name` and `description` (both required):

```markdown
---
name: my-skill
description: What this skill does and when to use it
---

# Skill Instructions

Your instructions here...
```

## Finding More Skills

- **[github/awesome-copilot](https://github.com/github/awesome-copilot)** - Official GitHub resources with community skills
- **`/plugin marketplace`** - Browse and install skills from within Copilot CLI

## Creating Your Own

1. Create a folder: `mkdir ~/.copilot/skills/my-skill`
2. Create `SKILL.md` with frontmatter
3. Add your instructions
4. Test by asking Copilot something that matches your description

See [Chapter 05: Skills](../../05-skills/README.md) for detailed guidance.
