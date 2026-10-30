---
title: "The Popover API: menus and notices without a library"
series: "native-first"
order: 13
reader_question: "What is the popover attribute, and what can it replace?"
standards:
  - "popover attribute (Popover API)"
baseline_status_with_date_and_source: "Baseline Newly available 2025-01-27. Source: webstatus.dev id:popover; web.dev Baseline 2025 (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/notifications.css [CODE, AI-co]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/css/references/menu.md [AI-INST: topic only]"
  - "https://github.com/Autocss-com/autocss/issues/8 [issue]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Popover_API"
  - "https://html.spec.whatwg.org/multipage/popover.html"
  - "https://api.webstatus.dev/v1/features?q=id:popover"
  - "https://web.dev/baseline/2025"
autocss_link: "CSS — the UI runtime"
status: outline
---

# The Popover API: menus and notices without a library

**Reader question:** What is the popover attribute, and what can it replace?

## Outline

- **Hook:** the z-index arms race.
- **Problem:** modal, dropdown and tooltip libraries each carry their own show/hide, stacking and dismiss code.
- **Native solution:** the popover attribute puts content in the top layer and closes it on outside click or Esc.
- **Code idea (described):** one notice and one menu, each a popover, with no stacking rules.
- **Replaces:** show/hide, z-index and dismiss code from modal, dropdown and tooltip libraries (browser-features.md).
- **Caveat:** placing it next to its trigger needs anchor positioning, not Baseline yet; popover=hint is not in Safari (browser-features.md).
- **Link out:** MDN Popover API, the spec, webstatus.
