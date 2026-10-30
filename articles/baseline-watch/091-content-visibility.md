---
title: "content-visibility: skip rendering what nobody can see yet"
series: "baseline-watch"
order: 91
reader_question: "How do I speed up a long page without virtual-scroll scripts?"
standards:
  - "content-visibility"
baseline_status_with_date_and_source: "Baseline Newly available 2025-09-15. Source: webstatus.dev id:content-visibility; web.dev Baseline 2025 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/content-visibility"
  - "https://drafts.csswg.org/css-contain-2/#content-visibility"
autocss_link: "CSS — the UI runtime"
status: outline
---

# content-visibility: skip rendering what nobody can see yet

**Reader question:** How do I speed up a long page without virtual-scroll scripts?

## Outline

- **Problem:** virtual-scroll scripts for long pages.
- **Native solution:** content-visibility: auto lets the browser skip off-screen rendering; measure before and after (zero-dependencies 028).
- **Link out:** MDN content-visibility; the spec.
