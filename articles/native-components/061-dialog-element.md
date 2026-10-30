---
title: "The dialog element: modals without a modal library"
series: "native-components"
order: 61
reader_question: "Do I need a library to build an accessible modal?"
standards:
  - "<dialog>"
  - "requestClose()"
  - "closedby"
baseline_status_with_date_and_source: "<dialog>: Widely since 2024-09-14 (webstatus, noted in browser-features.md); requestClose(): Newly 2025-05-27; closedby: NOT Baseline (no Safari). Source: webstatus.dev (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/HTML/Reference/Elements/dialog"
  - "https://developer.mozilla.org/docs/Web/API/HTMLDialogElement/requestClose"
  - "https://html.spec.whatwg.org/multipage/interactive-elements.html#dom-dialog-requestclose"
autocss_link: "none (conflict: AGENTS.md 'HTML — structure only' uses label + input, no script-driven buttons)"
status: outline
---

# The dialog element: modals without a modal library

**Reader question:** Do I need a library to build an accessible modal?

## Outline

- **Problem:** modal libraries re-create focus handling, Esc to close and the backdrop.
- **Native solution:** dialog gives those built in; requestClose() lets a cancel check run; closedby light dismiss is not in Safari yet.
- **Link out:** MDN dialog and requestClose(); the HTML spec.
