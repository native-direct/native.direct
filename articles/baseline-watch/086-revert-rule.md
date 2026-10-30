---
title: "revert-rule: undo one rule without !important"
series: "baseline-watch"
order: 86
reader_question: "How do I roll back a property without piling on overrides?"
standards:
  - "revert-rule keyword"
baseline_status_with_date_and_source: "Baseline Newly available 2026-09-14. Source: webstatus.dev id:revert-rule (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/color-themes-system/blob/main/assets/css/themes.css (uses !important: the before case) [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/AGENTS.md (§ CSS — the UI runtime: no !important) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Values/revert-rule"
  - "https://drafts.csswg.org/css-cascade-5/#revert-rule-keyword"
autocss_link: "CSS — the UI runtime"
status: outline
---

# revert-rule: undo one rule without !important

**Reader question:** How do I roll back a property without piling on overrides?

## Outline

- **Problem:** !important and override stacks to undo one earlier rule (repos.md #44, P7).
- **Native solution:** revert-rule rolls a property back as if the current rule did not exist.
- **Link out:** MDN revert-rule; the spec.
