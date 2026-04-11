# Install — Codex (OpenAI)

## Method 1: AGENTS.md (recommended)

Prepend the contents of `cognitive-protocol.md` to your project's `AGENTS.md` file. Codex reads this file automatically.

```bash
cat cognitive-protocol.md AGENTS.md > AGENTS.md.tmp && mv AGENTS.md.tmp AGENTS.md
```

If `AGENTS.md` doesn't exist yet:

```bash
cp cognitive-protocol.md AGENTS.md
```

## Method 2: System prompt

If using the Codex API, prepend `cognitive-protocol.md` contents to your system prompt.

## What to include

- **Always**: `cognitive-protocol.md` (~30 lines, fits easily in any context window)
- **Optional**: Append relevant sections from `SKILL.md` if you want the full framework available
- **Skip**: `anti-patterns.md` and `examples.md` — these are reference material, not operational rules

## Stacking with other cognitive bases

Non-attachment can be placed at any position relative to other cognitive bases. It operates on a different axis (your relationship to frameworks, not the frameworks themselves), so order doesn't matter. Place it wherever is convenient.
