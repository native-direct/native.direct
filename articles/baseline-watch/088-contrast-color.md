---
title: "contrast-color(): readable text on any background"
series: "baseline-watch"
order: 88
reader_question: "How do I pick black or white text for any brand color automatically?"
standards:
  - "contrast-color()"
baseline_status_with_date_and_source: "Baseline Newly available 2026-04-10. Source: webstatus.dev id:contrast-color; web.dev Baseline 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/4 (contrast-safe theme links) [OWN]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/color_value/contrast-color"
  - "https://drafts.csswg.org/css-color-6/#funcdef-contrast-color"
  - "https://web.dev/baseline/2026"
autocss_link: "CSS — the UI runtime"
status: outline
---

# contrast-color(): readable text on any background

**Reader question:** How do I pick black or white text for any brand color automatically?

## Outline

- **Problem:** Sass or script contrast pickers for every theme color.
- **Native solution:** contrast-color() returns black or white, whichever contrasts more; still check the WCAG ratio by hand.
- **Link out:** MDN contrast-color(); the spec.
