---
title: "The Custom Highlight API: highlight text without wrapper spans"
series: "baseline-watch"
order: 89
reader_question: "How do I highlight search matches without wrapping them in spans?"
standards:
  - "Custom Highlight API"
  - "::highlight()"
baseline_status_with_date_and_source: "Baseline Newly available 2026-03-24. Source: webstatus.dev id:highlight; web.dev Baseline 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/API/Highlight"
  - "https://drafts.csswg.org/css-highlight-api-1/"
autocss_link: "none (ranges are built in JavaScript; check against 'JavaScript — data transport only')"
status: outline
---

# The Custom Highlight API: highlight text without wrapper spans

**Reader question:** How do I highlight search matches without wrapping them in spans?

## Outline

- **Problem:** highlight libraries wrap every match in a span and change the DOM.
- **Native solution:** register text ranges and style them with ::highlight(), no extra elements.
- **Link out:** MDN Highlight; the spec.
