# Mobile Store Screenshot Requirements

Codex skill for generating App Store / Google Play screenshot sets and `1024 x 500` featured graphics from real app screenshots.

## Use

Invoke the skill as:

```text
Use $screenshot to generate mobile store screenshots from the latest app screenshots in Downloads.
```

## Skill Files

- `SKILL.md`: trigger metadata and high-level workflow
- `references/requirements.md`: authoritative decision tree
- `references/checklist.md`: completion checklist
- `references/mistakes.md`: known failure modes
- `agents/openai.yaml`: UI metadata for skill surfaces

## Core Rules

- Ask for submission target: App Store, Google Play, or both.
- Default to three output categories: phone screenshots, tablet/iPad screenshots, and featured graphic.
- Generate only from suitable real source screenshots the user provides.
- Use straight/aligned placement by default.
- Offer iPhone frame/notch/tilted layout only for App Store-only phone screenshots.
- If Google Play is included, generate the `1024 x 500` featured graphic or report why it cannot be generated.
- If a screenshot lacks enough clues for explanation copy, ask the user for a short phrase before final generation.
