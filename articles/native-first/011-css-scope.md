---
title: "@scope is Baseline: scoped styles without BEM or build tools"
series: "native-first"
order: 11
reader_question: "How do I keep a component's styles from leaking without naming schemes?"
standards:
  - "@scope"
baseline_status_with_date_and_source: "Baseline Newly available 2026-03-24. Source: webstatus.dev id:scope; web.dev Baseline 2026 page (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/AGENTS.md (§ CSS — the UI runtime names @layer and @scope) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@scope"
  - "https://drafts.csswg.org/css-cascade-6/#scope-atrule"
  - "https://api.webstatus.dev/v1/features?q=id:scope"
  - "https://web.dev/baseline/2026"
autocss_link: "CSS — the UI runtime"
status: outline
---

# @scope is Baseline: scoped styles without BEM or build tools

**Reader question:** How do I keep a component's styles from leaking without naming schemes?

## Outline

- **Hook:** class names long enough to act as a firewall.
- **Problem:** BEM and CSS Modules exist to stop styles leaking; one adds names, the other adds tools.
- **Native solution:** @scope limits rules to one part of the page, with an optional inner boundary where they stop.
- **Code idea (described):** a card scope that styles the card but stops at the content nested inside it.
- **Replaces:** BEM naming; CSS Modules or scoped-CSS build tooling (browser-features.md).
- **Caveat:** Newly available means recent browsers only; show the status and date.
- **Link out:** MDN @scope, the spec, webstatus.
