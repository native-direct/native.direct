---
title: "Layout that counts its children"
series: "css-state"
order: 42
reader_question: "Can CSS adapt to how many items a row has?"
standards:
  - ":has()"
  - ":nth-child()"
  - ":last-child"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19 (Newly 2023-12-19). Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30). :nth-child(): UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/dragontheory/D7460N/blob/main/assets/css/styles.css (:has(> :last-child:nth-child(n))) [CODE]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Quantity Queries) [OWN]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:nth-child"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:has"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Layout that counts its children

**Reader question:** Can CSS adapt to how many items a row has?

## Outline

- **Problem:** layouts that need a script to count items.
- **Native solution:** :has() with :last-child:nth-child(n) lets a container react to its own child count. Newer: sibling-count() (baseline-watch 087).
- **Link out:** MDN :nth-child() and :has().
