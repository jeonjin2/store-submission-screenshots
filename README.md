# Screenshot

Codex skill for generating store-submission screenshots and `1024 x 500` featured graphics from real app screenshots.

It turns vague requests like "make App Store screenshots" into a repeatable decision flow: ask only for missing choices, use only real provided screens, keep layouts submission-safe, and validate final pixel dimensions.

## What It Does

- Generates phone screenshots, tablet/iPad screenshots, and featured graphics.
- Supports App Store, Google Play, or both.
- Defaults to straight/aligned layouts for safer store submission.
- Offers iPhone frame/notch/tilted layouts only for App Store-only phone screenshots.
- Creates Korean, English, or bilingual variants.
- Picks readable background/text colors from app screenshots unless the user provides colors.
- Warns when the provided screenshot count is low instead of inventing fake screens.
- Requires a Google Play featured graphic when Google Play is included.

## Install

Clone the repo, then expose it to Codex as the `$screenshot` skill:

```bash
git clone https://github.com/jeonjin2/store-submission-screenshots.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/store-submission-screenshots" ~/.codex/skills/screenshot
```

If you keep skills somewhere else, point the symlink at that local clone.

## Use

```text
Use $screenshot to generate mobile store screenshots from the latest app screenshots in Downloads.
```

```text
$screenshot Use the screenshots in /Users/james/Downloads and make Korean App Store and Google Play assets.
```

```text
$screenshot Create phone screenshots, tablet screenshots, and a featured graphic. Use a clean rounded font and infer the copy when the screen labels are clear.
```

## Output Defaults

- Phone screenshots: `1242 x 2688`
- Tablet/iPad portrait screenshots: `2064 x 2752`
- Tablet/iPad landscape screenshots: `2752 x 2064`
- Featured graphic: `1024 x 500`

Generated assets should be saved under `/Users/james/Code` by default unless the user gives another destination.

## Rules It Enforces

- Ask for submission target: App Store, Google Play, or both.
- Ask for language, font, and color preferences only when they are not already clear.
- Use only suitable real screenshots provided by the user.
- Remove status bars/top bars before placing screenshots on final canvases.
- Use straight/aligned placement by default.
- Ask for a short phrase when the screen does not contain enough clues for explanation copy.
- Do not invent features, rankings, awards, download counts, or unsupported marketing claims.
- Do not use competitor screenshots, store listing screenshots, or wrong-brand screenshots as final assets.
- Do not create fake extra screenshots when too few source screens are available.
- Validate exact pixel dimensions before claiming completion.

## Skill Files

- `SKILL.md`: trigger metadata and high-level workflow
- `references/requirements.md`: authoritative decision tree
- `references/checklist.md`: completion checklist
- `references/mistakes.md`: known failure modes
- `agents/openai.yaml`: UI metadata for skill surfaces

## Notes

This is a Codex skill, not a standalone image generator. It gives Codex the reusable rules for deciding what to ask, what to generate, what to avoid, and how to verify the outputs.
