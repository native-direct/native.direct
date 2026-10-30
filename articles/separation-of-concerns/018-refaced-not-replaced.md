---
title: "Refaced, not replaced: redesign without a rewrite"
series: "separation-of-concerns"
order: 18
reader_question: "Why does a redesign usually turn into a rewrite?"
standards:
  - "Presentation layer kept in CSS"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Architecture › HTML/CSS) [OWN]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Grid_layout/Accessibility (MDN: HTML is the content layer, CSS the presentation layer)"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Refaced, not replaced: redesign without a rewrite

**Reader question:** Why does a redesign usually turn into a rewrite?

## Outline

- **Problem:** when look and logic share files, a new design means new code.
- **Native solution:** keep the look in CSS only, so a redesign swaps stylesheets and leaves HTML and data alone.
- **Link out:** MDN grid and accessibility guide (states the layer split).
