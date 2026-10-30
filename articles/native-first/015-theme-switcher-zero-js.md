---
title: "A light, dark and accent theme switcher with zero JavaScript"
series: "native-first"
order: 15
reader_question: "How do I offer light, dark and accent choices with CSS alone?"
standards:
  - ":has()"
  - ":checked"
  - "color-scheme"
  - "light-dark()"
  - "color-mix()"
  - "oklch()"
baseline_status_with_date_and_source: "light-dark(): Newly 2024-05-13; color-mix(): Widely 2025-11-09; oklch(): Widely 2025-11-09; :has(): Widely 2026-06-19. Source: webstatus.dev (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/color-themes-system/blob/main/assets/css/themes.css [CODE]"
  - "https://dragontheory.github.io/color-themes-system/ (live demo, 200 on 2026-10-30)"
  - "https://github.com/dragontheory/D7460N-with-db/issues/4 (contrast and theme links) [OWN]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/color_value/light-dark"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/color_value/color-mix"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/color-scheme"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:checked"
autocss_link: "CSS — the UI runtime"
status: outline
---

# A light, dark and accent theme switcher with zero JavaScript

**Reader question:** How do I offer light, dark and accent choices with CSS alone?

## Outline

- **Hook:** theme toggles that flash, or need a script just to flip a class.
- **Problem:** script-driven theming duplicates what CSS already knows about color schemes.
- **Native solution:** radio inputs set the scheme through :root:has(:checked); light-dark() and color-mix() derive the colors.
- **Code idea (described):** light, dark and auto radios plus an accent group, all styled from one set of oklch tokens.
- **Replaces:** JavaScript theme toggles and duplicated prefers-color-scheme blocks.
- **Caveat:** the live demo uses !important, hsl and a Google Fonts import (repos.md D1, P7), so show the current rules; keep the inputs keyboard and screen-reader reachable (repos.md P1); remembering the choice needs storage (a script).
- **Link out:** MDN light-dark(), color-mix(), color-scheme, :checked; the live demo.
