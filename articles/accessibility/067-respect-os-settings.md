---
title: "Respect the user's OS settings: motion, contrast, colors"
series: "accessibility"
order: 67
reader_question: "Which user preferences should CSS honor?"
standards:
  - "prefers-reduced-motion"
  - "prefers-contrast"
  - "forced-colors"
  - "prefers-reduced-transparency"
  - "system colors"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/starter/blob/main/README.md (§ Where users live) [OWN*]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/color-scheme.css [CODE]"
  - "https://github.com/dragontheory/color-themes-system/blob/main/assets/css/themes.css (forced-colors block) [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-contrast"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/forced-colors"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-transparency"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/system-color"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Respect the user's OS settings: motion, contrast, colors

**Reader question:** Which user preferences should CSS honor?

## Outline

- **Problem:** sites ignore settings users chose for health or comfort.
- **Native solution:** media features read those settings; system colors (Canvas, CanvasText) are safe defaults in forced-colors mode.
- **Link out:** MDN media feature pages and system-color.
