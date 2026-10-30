---
title: "align-content in plain blocks: center without flex or grid"
series: "baseline-watch"
order: 84
reader_question: "How do I vertically center content in a plain block?"
standards:
  - "align-content in block layout"
baseline_status_with_date_and_source: "Baseline Widely available 2026-10-16 (Newly 2024-04-16). Source: webstatus.dev id:align-content-block (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/align-content"
  - "https://drafts.csswg.org/css-align-3/#align-justify-content"
  - "https://api.webstatus.dev/v1/features?q=id:align-content-block"
autocss_link: "none (conflict: AGENTS.md 'Stack' sets Grid-only layout)"
status: outline
---

# align-content in plain blocks: center without flex or grid

**Reader question:** How do I vertically center content in a plain block?

## Outline

- **Problem:** a flex or grid wrapper added only to center one thing.
- **Native solution:** align-content now works on a plain block container.
- **Link out:** MDN align-content; the spec; webstatus.
