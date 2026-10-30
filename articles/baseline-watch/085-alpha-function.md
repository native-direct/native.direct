---
title: "alpha(): change a color's opacity without Sass"
series: "baseline-watch"
order: 85
reader_question: "How do I make a color token semi-transparent without duplicating it?"
standards:
  - "alpha()"
baseline_status_with_date_and_source: "Baseline Newly available 2026-09-14. Source: webstatus.dev id:alpha; MDN Firefox 155 notes; WebKit Safari 27.0; web.dev Sep 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/color_value/alpha"
  - "https://drafts.csswg.org/css-color-5/#relative-alpha"
  - "https://web.dev/blog/web-platform-09-2026"
autocss_link: "CSS — the UI runtime"
status: outline
---

# alpha(): change a color's opacity without Sass

**Reader question:** How do I make a color token semi-transparent without duplicating it?

## Outline

- **Problem:** a second, semi-transparent copy of every color token, or a Sass function.
- **Native solution:** alpha() changes only the transparency of an existing color.
- **Link out:** MDN alpha(); the spec; web.dev Sep 2026.
