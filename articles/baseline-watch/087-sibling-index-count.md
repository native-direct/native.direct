---
title: "sibling-index() and sibling-count(): stagger without scripts"
series: "baseline-watch"
order: 87
reader_question: "How do I stagger items without writing an index in JavaScript?"
standards:
  - "sibling-index()"
  - "sibling-count()"
baseline_status_with_date_and_source: "Baseline Newly available 2026-08-18. Source: webstatus.dev id:sibling-count; web.dev Baseline digest Aug 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/D7460N/blob/main/assets/css/styles.css (quantity queries: the older way) [CODE]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/sibling-index"
  - "https://drafts.csswg.org/css-values-5/#tree-counting"
  - "https://web.dev/blog/baseline-digest-aug-2026"
autocss_link: "CSS — the UI runtime"
status: outline
---

# sibling-index() and sibling-count(): stagger without scripts

**Reader question:** How do I stagger items without writing an index in JavaScript?

## Outline

- **Problem:** scripts write --index on every item, or long :nth-child() lists.
- **Native solution:** sibling-index() and sibling-count() give position and total as numbers for calc().
- **Link out:** MDN sibling-index(); the spec; web.dev digest.
