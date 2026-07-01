# Generation Checklist

Use this before claiming App Store screenshot work is complete.

## Inputs

- [ ] Source files came from `/Users/james/Downloads` or another user-specified path.
- [ ] Source files are real current-app screenshots.
- [ ] No competitor/store listing screenshots are used as final assets.
- [ ] Wrong-brand screenshots were not patched by text-only replacement.
- [ ] Submission target is known: App Store, Google Play, or both.
- [ ] Requested output categories are known, or defaulted to phone screenshots, tablet/iPad screenshots, and featured graphic.
- [ ] Language choice is known, or defaulted appropriately.
- [ ] Font choice is known, or defaulted to clean sans/gothic.
- [ ] Color preference is known, or automatic app-derived colors were used.
- [ ] Screens lacking enough visible clues have user-provided short explanation copy.

## Count Warnings

- [ ] Generated only from suitable source screenshots the user provided.
- [ ] No fake extra screenshots were invented.
- [ ] If Google Play is included and fewer than four phone screenshots are available, the user was warned.
- [ ] If Google Play tablet/large-screen assets are included and fewer than four tablet screenshots are available, the user was warned.
- [ ] If Google Play is included, a `1024 x 500` featured graphic was generated or the blocker was reported.

## Processing

- [ ] Status bar/top bar removed.
- [ ] Correct target canvas created first.
- [ ] Screenshots placed after cropping.
- [ ] Straight/aligned placement used by default.
- [ ] App Store-only phone mockup/frame/notch/tilted style used only if the user chose it.
- [ ] Google Play-including outputs do not use iPhone notch/frame/tilted mockups unless explicitly requested.
- [ ] Tablet/iPad screenshots are not tilted unless explicitly requested.
- [ ] Text is plain, readable, and inside the canvas.
- [ ] No text outline/effects unless requested.
- [ ] Background and text colors are high-contrast and consistent across the set.
- [ ] Standalone logo removed if user requested no logo.

## Outputs

- [ ] Phone outputs are `1242 x 2688`.
- [ ] Tablet/iPad portrait outputs are `2064 x 2752`.
- [ ] Tablet/iPad landscape outputs are `2752 x 2064`.
- [ ] Featured graphics are `1024 x 500`.
- [ ] Korean version generated when requested.
- [ ] English version generated when requested.
- [ ] Output files saved under `/Users/james/Code`.
- [ ] Pixel dimensions validated with `sips` or equivalent.
