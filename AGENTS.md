# AGENTS.md

Beginner-friendly course teaching GitHub Copilot CLI. Educational content, not software.

## Structure

| Path | Purpose |
|------|---------|
| `00-07/` | Chapters: analogy → concepts → hands-on → assignment → next |
| `samples/buggy-code/` | **Intentional bugs** for debugging exercises |
| `QUICK-REFERENCE.md` | Command cheat sheet (source of truth) |
| `QUICK-REFERENCE.pdf` | Auto-generated from above |

## Do

- Keep explanations beginner-friendly; explain AI/ML jargon when used
- Ensure bash examples are copy-paste ready
- Use terminology from `QUICK-REFERENCE.md`
- Tone: friendly, encouraging, practical

## Don't

- Fix bugs in `samples/buggy-code/` — they're intentional
- Add chapters without updating README.md course table
- Assume readers know AI/ML terminology

## Build

```bash
npm install && npm run generate:pdf
```
