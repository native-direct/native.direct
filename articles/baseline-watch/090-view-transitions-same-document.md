---
title: "Same-document view transitions: animate state changes natively"
series: "baseline-watch"
order: 90
reader_question: "How do I animate between two states of a page without an animation library?"
standards:
  - "View Transition API (same-document)"
baseline_status_with_date_and_source: "Baseline Newly available 2025-10-14. Source: webstatus.dev id:view-transitions; web.dev Baseline 2025 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/View_Transition_API"
  - "https://drafts.csswg.org/css-view-transitions-1/"
autocss_link: "none (conflict: AGENTS.md 'CSS — the UI runtime' does not use view transitions)"
status: outline
---

# Same-document view transitions: animate state changes natively

**Reader question:** How do I animate between two states of a page without an animation library?

## Outline

- **Problem:** FLIP animation libraries to move elements between states.
- **Native solution:** startViewTransition() captures before and after and animates between them.
- **Link out:** MDN View Transition API; the spec.
