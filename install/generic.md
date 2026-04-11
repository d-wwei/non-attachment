# Install — Generic (Any Agent/Framework)

> **Recommended**: Run `./install.sh` from the repo root for automated installation. Supports Claude Code, Gemini CLI, Codex CLI, Cursor, OpenCode, and OpenClaw.
> The manual steps below are for reference or troubleshooting.

## Universal principle

Non-Attachment is a meta-cognitive base — it prevents fusion with any analytical framework, including itself. Installation means injecting `cognitive-protocol.md` into the agent's always-on instructions (system prompt, rules file, or configuration).

## Platform mapping

| Platform | Where to inject | File to use |
|---|---|---|
| Claude Code | `~/.claude/non-attachment.md` + ref in `CLAUDE.md` | `cognitive-protocol.md` |
| Codex | Prepend to `AGENTS.md` | `cognitive-protocol.md` |
| Gemini | `system_instruction` field | `cognitive-protocol.md` |
| Cursor | Prepend to `.cursorrules` | `cognitive-protocol.md` |
| ChatGPT | Custom Instructions -> system prompt | `cognitive-protocol.md` |
| LangChain | System message in chain | `cognitive-protocol.md` |
| AutoGPT / CrewAI | Agent system prompt | `cognitive-protocol.md` |
| Any other | Find the "always-on instructions" config and inject there | `cognitive-protocol.md` |

## Step by step

1. Locate your agent's system prompt or always-on rules file
2. Copy the contents of `cognitive-protocol.md` (~30 lines)
3. Paste it into the system prompt — position doesn't matter for this cognitive base
4. Non-attachment works at any position relative to other cognitive bases

## File selection guide

| Need | File | Size |
|---|---|---|
| Minimal install (core rules only) | `cognitive-protocol.md` | ~30 lines |
| Full reference framework | + `SKILL.md` | ~200 lines |
| Anti-pattern detection | + `anti-patterns.md` | ~120 lines |
| Teaching examples | + `examples.md` | ~120 lines |

For most agents, `cognitive-protocol.md` alone is sufficient. The additional files are reference material for when the agent needs deeper guidance.

## Troubleshooting

- **Agent ignores the rules**: Move `cognitive-protocol.md` content to the beginning of the system prompt. Most models weight earlier instructions more heavily.
- **Agent becomes indecisive**: This is the nihilism anti-pattern, not correct non-attachment. Add this line to your prompt: "Non-attachment increases judgment capacity. After releasing frames, commit decisively to the best available action."
- **Agent keeps citing the protocol by name**: This is tool worship. Add: "Apply these rules silently. Never reference them by name in output."
- **Context window pressure**: `cognitive-protocol.md` is ~30 lines. If that's too much, something else in your prompt needs trimming first.
