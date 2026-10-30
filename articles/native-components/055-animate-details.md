---
title: "Animating details open and closed with CSS only"
series: "native-components"
order: 55
reader_question: "How do I animate a disclosure with CSS?"
standards:
  - "::details-content"
  - "@starting-style"
  - "transition-behavior: allow-discrete"
  - "interpolate-size"
baseline_status_with_date_and_source: "::details-content: Newly 2025-09-16; @starting-style and allow-discrete: Newly 2024-08-06; interpolate-size: NOT Baseline (Chrome 129 only). Source: webstatus.dev (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/disclosure.css [CODE, AI-co]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/::details-content"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@starting-style"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/interpolate-size"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Animating details open and closed with CSS only

**Reader question:** How do I animate a disclosure with CSS?

## Outline

- **Problem:** accordion animation usually means wrapper elements and a script that measures height.
- **Native solution:** ::details-content plus transitions animates the body; animating to height: auto still needs interpolate-size, which is Chrome-only, so show a fallback.
- **Link out:** MDN ::details-content, @starting-style, interpolate-size. Follows native-first 012.
