---
title: "Container style queries: variant state without scripts"
series: "baseline-watch"
order: 92
reader_question: "How do I style children from a parent's custom property value?"
standards:
  - "@container style()"
baseline_status_with_date_and_source: "Baseline Newly available 2026-05-19. Source: webstatus.dev id:container-style-queries; web.dev Baseline 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/diag.css (@container style(--theme: dark), dev-only) [CODE]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Style Queries) [OWN]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@container"
  - "https://drafts.csswg.org/css-conditional-5/#style-container"
  - "https://api.webstatus.dev/v1/features?q=id:container-style-queries"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Container style queries: variant state without scripts

**Reader question:** How do I style children from a parent's custom property value?

## Outline

- **Problem:** script or class toggles for theme and variant state.
- **Native solution:** a parent sets a custom property; children respond with @container style().
- **Caveat:** the repo named chained-css-style-queries has no style query in it (repos.md D5).
- **Link out:** MDN @container; the spec; webstatus.
