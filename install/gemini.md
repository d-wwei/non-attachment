# Install — Gemini

## Method 1: system_instruction (API)

```python
import google.generativeai as genai

with open("cognitive-protocol.md") as f:
    non_attachment_rules = f.read()

model = genai.GenerativeModel(
    model_name="gemini-2.0-flash",
    system_instruction=non_attachment_rules
)
```

## Method 2: Google AI Studio

1. Open AI Studio -> System Instructions panel
2. Paste the contents of `cognitive-protocol.md`
3. Save as a preset for reuse

## Method 3: CLI / framework integration

If using a framework (LangChain, LlamaIndex, etc.), inject `cognitive-protocol.md` into the system message.

## What to include

- **Always**: `cognitive-protocol.md` — compact enough for any context budget
- **Optional**: Key sections from `SKILL.md` (absorbed wisdom, anti-pattern checklist) if context allows
- **Skip**: Install files, README, full examples

## Stacking with other cognitive bases

Non-attachment can be placed at any position in the system instruction relative to other cognitive bases. It monitors your relationship to active frameworks, not the frameworks themselves. No conflicts.
