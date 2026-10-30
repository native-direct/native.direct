---
title: "Container queries or media queries: which one, when"
series: "layout"
order: 52
reader_question: "When do I query the container instead of the viewport?"
standards:
  - "@container (size)"
  - "media query range syntax"
baseline_status_with_date_and_source: "Container size queries: Baseline Widely available 2025-08-14 (Newly 2023-02-14); media query range syntax: Widely 2025-09-27 (Newly 2023-03-27). Source: webstatus.dev id:container-queries, id:media-query-range-syntax (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Container Queries) [OWN]"
  - "https://github.com/dragontheory/chained-css-style-queries/blob/main/assets/css/layout.css (range syntax) [CODE]"
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/css/references/containers.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@container"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@media"
  - "https://drafts.csswg.org/css-conditional-5/#container-queries"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Container queries or media queries: which one, when

**Reader question:** When do I query the container instead of the viewport?

## Outline

- **Problem:** components that only look right at certain screen widths.
- **Native solution:** query the container for component layout; use range syntax when a viewport query is truly needed.
- **Link out:** MDN @container and @media; the spec.
