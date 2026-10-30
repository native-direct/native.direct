---
title: "Full-height app shells on phones: dvh, not 100vh"
series: "layout"
order: 54
reader_question: "Why does 100vh break on phones?"
standards:
  - "svh / lvh / dvh units"
baseline_status_with_date_and_source: "Baseline Widely available 2025-06-05 (Newly 2022-12-05). Source: webstatus.dev id:viewport-unit-variants (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/layout.css (100dvb) [CODE]"
  - "https://github.com/dragontheory/tmp (layout.css, 100dvh) [CODE]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/length"
  - "https://drafts.csswg.org/css-values-4/#viewport-variants"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Full-height app shells on phones: dvh, not 100vh

**Reader question:** Why does 100vh break on phones?

## Outline

- **Problem:** 100vh ignores the phone's moving toolbars, so the bottom gets cut off.
- **Native solution:** dynamic viewport units (dvh, or dvb for the block axis) track the visible area; no --vh script.
- **Link out:** MDN length units; the spec.
