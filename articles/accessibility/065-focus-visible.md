---
title: "Style focus with :focus-visible, never outline: none"
series: "accessibility"
order: 65
reader_question: "How do I style focus without hurting keyboard users?"
standards:
  - ":focus-visible"
  - "outline"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ UX To Remember) [OWN]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/a11y.css [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:focus-visible"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/outline"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Style focus with :focus-visible, never outline: none

**Reader question:** How do I style focus without hurting keyboard users?

## Outline

- **Problem:** outline: none removes the only sign of where keyboard focus is.
- **Native solution:** :focus-visible shows a clear ring for keyboard users without drawing it on every mouse click.
- **Link out:** MDN :focus-visible and outline.
