# Mobile Store Screenshot Requirements

This reference is the source of truth for App Store and Google Play screenshot/featured graphic generation.

## Source Inputs

- Use screenshot originals from `/Users/james/Downloads` when the user says the originals are in Downloads.
- Prefer the newest relevant image files unless the user gives an explicit file list.
- Do not use App Store search result screenshots, competitor app pages, or unrelated app screenshots as submission assets.
- For OrderiQ, use real OrderiQ screenshots. Do not fake this by only replacing visible text in an old screenshot from another app/brand.
- Generate only as many phone/tablet screenshots as there are suitable real source screenshots. Do not create fake extra screenshots to satisfy a count target.

## Initial Questions

Ask for these values when they are not already specified:

- Submission target: App Store, Google Play, or both.
- Output categories: phone screenshots, tablet/iPad screenshots, featured graphic. Default to all three for a full store set or when Google Play is included.
- Language: Korean, English, or Korean + English.
- Font style: clean sans/gothic by default; optional rounded, cute, Dotum, or Gulim.
- Color preference: automatic app-derived colors by default, or a user-specified background/text color.
- Explanation copy only when the screenshot does not provide enough visible clues to write a short accurate phrase.

Do not ask the user to do routine local file operations that can be done directly.

## Canonical Output Sizes

Use these sizes unless the user explicitly changes them:

- Phone screenshots: `1242 x 2688`
- Tablet/iPad portrait screenshots: `2064 x 2752`
- Tablet/iPad landscape screenshots: `2752 x 2064`
- Featured graphic / promotional image: `1024 x 500`

## Must Do

- Remove the status bar/top bar from all screenshots used for store submission assets.
- Create a blank canvas at the exact target size before placing screenshots.
- Place cropped screenshots into the canvas after status bar removal.
- Add a short explanation phrase above or beside the screenshots when making store screenshots.
- Keep explanation text plain and clean.
- Generate Korean and English versions when requested.
- For the `1024 x 500` featured graphic, use only two or three app screens when available.
- Validate final image dimensions after generation.
- Save generated artifacts under `/Users/james/Code` by default.

## Count Rules

- Generate from the suitable source screenshots the user provided; do not invent missing app screens.
- App Store screenshots can be submitted with a low count, but warn if the provided set is too sparse for a useful storefront.
- If Google Play is included and fewer than four phone screenshots are available, warn that Google Play publishing may still be possible with fewer screenshots but recommendation/large-format eligibility or storefront quality may be limited.
- If Google Play tablet/large-screen assets are included and fewer than four tablet screenshots are available, warn that tablet/Chromebook large-screen guidance expects at least four.
- If Google Play is included, the featured graphic is required. If no suitable screens exist for it, ask for more screenshots or confirm generating from the available ones.

## Layout Rules

- Default to straight/aligned placement for phone screenshots, tablet/iPad screenshots, and featured graphics.
- If the submission target includes Google Play, do not use iPhone notch, iPhone frame, or tilted device mockups unless the user explicitly overrides this.
- If the submission target is App Store only and the output is phone screenshots, offer style choices:
  - straight/aligned without device frame
  - iPhone frame with notch
  - tilted iPhone frame carousel treatment
- Use tilted phone treatment only after the user chooses it. Prefer connected carousel pairs such as `1-2`, `3-4`, `5-6` only when adjacent screenshots show a coherent flow.
- Keep all tablet/iPad screenshots straight/aligned by default. Tablet/iPad outputs should place the app screen on a clean canvas with explanation text.
- Do not apply tilted phone/mockup rules to tablet/iPad screenshots unless the user explicitly overrides this.

## Explanation Copy

- If a source screen contains visible clues such as labels, data, headings, or obvious actions, Codex may draft concise explanation copy.
- If a source screen lacks enough visible clues, ask the user for a short explanation before final generation.
- Keep copy factual and supported by the visible UI or user-provided explanation.
- Do not invent feature claims, rankings, awards, download counts, or unsupported functionality.

## Language And Typography

- Language choices: Korean, English, or Korean + English.
- If unspecified and the app/user context is Korean, default to Korean.
- If the user wants both stores or broad audience reach, suggest Korean + English but do not block if the user chooses one language.
- Default font style: clean sans/gothic.
- Optional font styles: rounded, cute, Dotum, Gulim.
- Use decorative/cute typography only when the app tone supports it or the user requests it.

## Color Rules

- Inspect the source screenshots for dominant app background colors and brand/accent colors.
- Choose a clean background that supports screenshot readability:
  - Light app UI: off-white or light gray background with charcoal text.
  - Dark app UI: charcoal or deep neutral background with white/light text.
  - Clear brand color: use it as an accent or soft background, not as low-contrast body text.
- If the app has no obvious brand/accent color, use neutral background colors.
- Keep all text high-contrast and readable.
- Use one consistent color system across a generated set.
- Do not use decorative gradients, heavy shadows, outlines, stickers, badges, or low-contrast color pairings unless explicitly requested.

## Text Styling

- Use simple text.
- Do not add outlines to explanation text.
- Do not add decorative text effects unless explicitly requested.
- Keep text readable and inside the canvas.

## Featured Graphic Rules

- Size must be exactly `1024 x 500`.
- Generate when Google Play is included. For App Store-only work, generate only if the user asks for it.
- Use two or three real app screens when available.
- Prefer screens that show different core values, not duplicates:
  - one primary/home/dashboard screen
  - one action/result/detail screen
  - one trust/status/summary screen if available
- If only one suitable screen is available, warn that two or three screens are preferred and ask whether to proceed with a simpler one-screen graphic unless the user has already asked to proceed.
- Remove status bars before placing the screens.
- Use straight/aligned placement by default.
- Include one short headline. If the screenshots do not provide enough clues, ask the user for that phrase.
- Make Korean and English versions when requested.
- If the user says to remove the logo, remove the standalone logo/icon from both language versions.
- Do not include a standalone logo/icon unless the user asks for it.

## Do Not Do

- Do not use competitor screenshots or App Store listing screenshots as final submission images.
- Do not merely overwrite a wrong app name inside an old screenshot and call it done.
- Do not use screenshots from the wrong app or old brand when real current-app screenshots are available.
- Do not apply iPhone frame, notch, or tilted mockup rules to Google Play-including outputs by default.
- Do not apply iPhone tilted mockup rules to tablet/iPad outputs.
- Do not add borders, outlines, stickers, badges, heavy effects, or decorative text treatments unless requested.
- Do not invent feature claims, rankings, download counts, awards, or unsupported functionality.
- Do not ask the user to do ordinary local file operations that can be done directly.

## Current User Preference Notes

- The user prefers fast execution over extended explanation during asset generation.
- The user wants clear separation between what is allowed for iPhone and what is allowed for iPad/tablet.
- The user wants straight/aligned placement by default.
- The user accepts iPhone frame/notch/tilted layout only as an App Store-only phone screenshot choice.
- The project default treats the canonical sizes in this reference as the required target sizes for generated store assets unless a user explicitly requests different dimensions.
- The user wants all store-submission screenshots to have the status bar removed.
- The user wants final assets generated directly, not just plans or explanations.
