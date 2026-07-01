---
name: appstore-screenshot-requirements
description: Create mobile store screenshot and featured graphic assets from real app screenshots. Use when Codex needs to generate, resize, crop, compose, validate, or review App Store or Google Play phone screenshots, tablet/iPad screenshots, Korean/English variants, typography/color choices, straight vs mockup layout decisions, or 1024x500 featured graphics, especially when source screenshots are in Downloads and final files must be saved under /Users/james/Code.
---

# Mobile Store Screenshot Requirements

Use this skill to produce App Store and/or Google Play-ready visual assets from real current-app source screenshots.

## Workflow

1. Read `references/requirements.md` before planning or generating assets.
2. If the task involves final generation, read `references/checklist.md` and use it as the completion checklist.
3. If the task involves reused screenshots, wrong-brand assets, feature graphics, mockups, or fixing prior bad assets, read `references/mistakes.md` before editing.
4. Locate source images in the user-specified folder. If the user says the originals are in Downloads, use `/Users/james/Downloads` and prefer the newest relevant real app screenshots.
5. Ask only for missing choices that materially affect the final asset: submission target, requested output categories, language, font, color preference, or explanation copy that cannot be inferred from the screen. Do not ask for routine local file operations.
6. Count suitable source screenshots before generation and warn when the count is below platform guidance or storefront quality expectations.
7. Remove the status bar/top bar before placing any screenshot into a submission canvas.
8. Create the target-size canvas first, then place the cropped screenshot or screens into it.
9. Validate exact pixel dimensions before claiming completion.
10. Save generated artifacts under `/Users/james/Code` by default.

## Decision Tree

Start by identifying:

- Submission target: App Store, Google Play, or both.
- Output categories: phone screenshots, tablet/iPad screenshots, featured graphic. Default to all three when Google Play is included or when the user asks for a full store set.
- Language: Korean, English, or both.
- Font style: default clean sans/gothic unless the user chooses rounded, cute, Dotum, or Gulim.
- Color preference: use automatic app-derived colors by default; honor explicit user colors when they preserve readability.

Generate only from suitable source screenshots the user provided. Do not invent missing screens.

## Required Sizes

- iPhone screenshots: `1242 x 2688`
- iPad portrait screenshots: `2064 x 2752`
- iPad landscape screenshots: `2752 x 2064`
- Featured graphic / promotional image: `1024 x 500`

## Design Rules

- Use real screenshots from the current app. Do not use competitor screenshots, App Store listing screenshots, or wrong-brand screenshots as final assets.
- Keep explanation text short, plain, readable, and inside the canvas.
- Do not add text outlines, stickers, badges, heavy effects, unsupported claims, rankings, awards, or download counts unless explicitly requested and supported.
- Default to straight/aligned screenshot placement for both stores.
- Offer iPhone frame/notch or tilted layout only for App Store-only phone screenshots, and only as a user-facing style choice.
- Keep Google Play-including work, tablet/iPad screenshots, and featured graphics straight/aligned unless the user explicitly overrides this.
- For `1024 x 500` featured graphics, use two or three real app screens when available.
- If a screen has enough visible clues, draft the explanation copy. If it does not, ask the user for a short explanation before final generation.
- Pick background and text colors from app/screenshot cues with readability first; use neutral high-contrast defaults when cues are unclear.

## Completion Evidence

Before final response, report the output path and the dimension validation method used, such as `sips -g pixelWidth -g pixelHeight`.
