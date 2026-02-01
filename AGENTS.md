# AGENTS.md

> Instructions for AI assistants working with this repository.

## Project Overview

This is a **beginner-friendly course** teaching GitHub Copilot CLI. It's educational content, not a software project.

**Target audience**: Developers new to AI-assisted CLI tools.

## Repository Structure

```
├── 00-quick-start/          # Installation and setup
├── 01-setup-and-first-steps/# First interactions
├── 02-context-conversations/# Multi-file analysis
├── 03-development-workflows/# Code review, debug, testing
├── 04-agents-custom-instructions/# Custom AI personas
├── 05-skills/               # Reusable commands
├── 06-mcp-servers/          # External service connections
├── 07-putting-it-together/  # Complete feature workflows
├── samples/
│   ├── buggy-code/          # Intentionally broken code for practice
│   ├── agents/              # Example agent configurations
│   └── mcp-configs/         # MCP server examples
├── demos/                   # Demo scripts/recordings
├── QUICK-REFERENCE.md       # Command cheat sheet
└── README.md                # Course introduction
```

## Content Conventions

### Chapter Structure
Each chapter folder contains a `README.md` following this pattern:
1. Real-world analogy
2. Core concepts
3. Hands-on examples (runnable bash blocks)
4. Assignment
5. What's next

### Code Examples
- All bash blocks are **runnable** as-is
- Sample bugs in `samples/buggy-code/` are **intentional** for debugging exercises
- Don't "fix" the buggy code unless specifically asked

## Key Files

| File | Purpose |
|------|---------|
| `QUICK-REFERENCE.md` | Command cheat sheet (source of truth for syntax) |
| `QUICK-REFERENCE.pdf` | Print-friendly version (auto-generated) |
| `IMAGE_PROMPTS.md` | Prompts used to generate course images |
| `.md-to-pdf.json` | PDF generation config |

## Working With This Repo

### Do
- Keep explanations beginner-friendly
- Use consistent terminology from `QUICK-REFERENCE.md`
- Ensure bash examples are copy-paste ready
- Maintain the chapter numbering pattern (00-07)

### Don't
- Fix intentional bugs in `samples/buggy-code/`
- Add advanced jargon without explanation
- Create new chapters without updating README.md course table
- Assume readers know AI/ML terminology

## Build Commands

```bash
npm install           # Install dependencies
npm run generate:pdf  # Regenerate QUICK-REFERENCE.pdf
```

## Content Style

- **Tone**: Friendly, encouraging, practical
- **Format**: GitHub-flavored markdown
- **Diagrams**: ASCII art boxes (see README.md for examples)
- **Commands**: Always show full syntax, not abbreviated
