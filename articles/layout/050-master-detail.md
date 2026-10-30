---
title: "Master/detail without the ping-pong"
series: "layout"
order: 50
reader_question: "How do I stop users bouncing between list and detail pages?"
standards:
  - "CSS Grid"
  - ":has()"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19 (Newly 2023-12-19). Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/THOR/blob/master/README.md (commented ping-pong effect bullet) [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ SPA › Perspective) [OWN]"
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/layout.css (aside column appears only when its fieldset has content) [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Grid_layout"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:has"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Master/detail without the ping-pong

**Reader question:** How do I stop users bouncing between list and detail pages?

## Outline

- **Problem:** list page, detail page, back, over and over.
- **Native solution:** list and detail side by side; the detail column appears only when it has content (:has()).
- **Link out:** MDN grid guide and :has().
