---
title: "CSS nesting is widely available: drop the preprocessor"
series: "native-first"
order: 6
reader_question: "Do I still need Sass just to nest my CSS?"
standards:
  - "CSS nesting (& selector)"
baseline_status_with_date_and_source: "Baseline Widely available 2026-06-11 (Newly 2023-12-11). Source: webstatus.dev id:nesting; web.dev Baseline digest Jun 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/Nesting_selector"
  - "https://drafts.csswg.org/css-nesting-1/"
  - "https://api.webstatus.dev/v1/features?q=id:nesting"
  - "https://web.dev/blog/baseline-digest-jun-2026"
autocss_link: "Stack"
status: outline
---

# CSS nesting is widely available: drop the preprocessor

**Reader question:** Do I still need Sass just to nest my CSS?

## Outline

- **Hook:** a build step kept alive only for nesting.
- **Problem:** a preprocessor means a toolchain, config and its own upgrades (see native-first 004).
- **Native solution:** plain CSS nesting with &, now in every core browser.
- **Code idea (described):** one Sass block and its native twin; note that nested selectors take :is()-style specificity (MDN).
- **Replaces:** Sass, Less or PostCSS used only for nesting (browser-features.md).
- **Caveat:** keep nesting shallow (minimally nested, AGENTS.md Stack); Sass functions are another matter (@function is not Baseline).
- **Link out:** MDN nesting selector, the spec, webstatus.
