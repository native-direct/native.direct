---
title: "Styled scrollbars that don't hijack scrolling"
series: "native-components"
order: 56
reader_question: "How do I style a scrollbar safely?"
standards:
  - "scrollbar-color"
  - "scrollbar-width"
baseline_status_with_date_and_source: "scrollbar-color: Baseline Newly available 2025-12-12. Source: webstatus.dev id:scrollbar-color (via browser-features.md, as of 2026-10-30). scrollbar-width: UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/scrolling.css [CODE]"
  - "https://github.com/dragontheory/D7460N-with-db/issues/10 [OWN]"
  - "https://codepen.io/dragontheory/pen/mdxJXyw (live status unverified) [CODE]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/scrollbar-color"
  - "https://drafts.csswg.org/css-scrollbars-1/#scrollbar-color"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Styled scrollbars that don't hijack scrolling

**Reader question:** How do I style a scrollbar safely?

## Outline

- **Problem:** custom scrollbar scripts replace native scrolling and break keyboard and touch behavior.
- **Native solution:** color and thin the native scrollbar with standard properties; skip ::-webkit-scrollbar.
- **Link out:** MDN scrollbar-color; the spec.
