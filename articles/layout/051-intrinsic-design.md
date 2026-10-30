---
title: "Intrinsic design: stop thinking in breakpoints"
series: "layout"
order: 51
reader_question: "What is intrinsic design, and why skip width breakpoints?"
standards:
  - "min(), max(), clamp()"
  - "ch unit"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Intrinsic Design; credits Jen Simmons: name and link) [OWN, CREDIT]"
  - "https://github.com/Autocss-com/ai/blob/main/AGENTS.md (§ CSS — the UI runtime: no size-based @media; ch units) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/clamp"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/min"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/max"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Intrinsic design: stop thinking in breakpoints

**Reader question:** What is intrinsic design, and why skip width breakpoints?

## Outline

- **Problem:** width breakpoints guess at devices and break between them.
- **Native solution:** let content and math functions size things (min(), max(), clamp(), ch); credit Jen Simmons for the term.
- **Link out:** MDN clamp(), min(), max().
