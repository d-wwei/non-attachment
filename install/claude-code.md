# Install — Claude Code

## Quick install

```bash
# 1. Copy cognitive protocol to Claude's config
cp cognitive-protocol.md ~/.claude/non-attachment.md

# 2. Add reference in CLAUDE.md
echo '@~/.claude/non-attachment.md' >> ~/.claude/CLAUDE.md
```

## What gets loaded where

| File | Destination | Purpose |
|---|---|---|
| `cognitive-protocol.md` | `~/.claude/non-attachment.md` | Always-on core rules (~30 lines) |
| `SKILL.md` | `~/.claude/skills/non-attachment/SKILL.md` | Full reference (loaded on demand) |
| `anti-patterns.md` | `~/.claude/skills/non-attachment/anti-patterns.md` | Detailed anti-pattern guide |
| `examples.md` | `~/.claude/skills/non-attachment/examples.md` | Before/after reference |

## Full install (with skill files)

```bash
# 1. Core rules
cp cognitive-protocol.md ~/.claude/non-attachment.md

# 2. Skill files
mkdir -p ~/.claude/skills/non-attachment
cp SKILL.md ~/.claude/skills/non-attachment/
cp anti-patterns.md ~/.claude/skills/non-attachment/
cp examples.md ~/.claude/skills/non-attachment/

# 3. Register in CLAUDE.md
echo '@~/.claude/non-attachment.md' >> ~/.claude/CLAUDE.md
```

## Verify

Ask Claude Code: "What are the non-attachment cognitive rules you're following?" It should list the five sections from `cognitive-protocol.md`: detect framework fusion, hold frameworks lightly, test for genuine detachment, preserve judgment through freedom, output self-check.

## Stacking with other cognitive bases

Non-attachment operates at a meta-level above all other cognitive bases. Load order doesn't matter — it monitors your relationship to whatever frameworks are active, not the frameworks themselves. No conflicts with any cognitive base.

If First Principles, Tacit Knowledge, or other cognitive bases are already in CLAUDE.md, simply add the non-attachment reference. All protocols load independently.

## Uninstall

```bash
rm ~/.claude/non-attachment.md
rm -rf ~/.claude/skills/non-attachment
# Remove the @~/.claude/non-attachment.md line from ~/.claude/CLAUDE.md
```
