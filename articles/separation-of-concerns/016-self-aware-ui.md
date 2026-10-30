---
title: "The self-aware UI: content decides what shows"
series: "separation-of-concerns"
order: 16
reader_question: "How can a panel know it has data?"
standards:
  - ":has()"
  - ":empty"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19 (Newly 2023-12-19). Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30). :empty: UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/5 [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Self-Aware) [OWN]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:has"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:empty"
autocss_link: "CSS — the UI runtime"
status: outline
---

# The self-aware UI: content decides what shows

**Reader question:** How can a panel know it has data?

## Outline

- **Problem:** visibility kept in script flags or in the data drifts away from what the page really holds.
- **Native solution:** let selectors read presence: :has() for has-content, :empty for nothing-yet; the panel shows itself when data arrives.
- **Link out:** MDN :has() and :empty. Builds on native-first 007 and 008.
