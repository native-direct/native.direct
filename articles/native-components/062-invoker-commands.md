---
title: "Invoker commands: buttons that open dialogs with no script"
series: "native-components"
order: 62
reader_question: "Can a button open a dialog or popover without JavaScript?"
standards:
  - "command / commandfor attributes"
baseline_status_with_date_and_source: "Baseline Newly available 2025-12-12. Source: webstatus.dev id:invoker-commands; web.dev Baseline 2025 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Invoker_Commands_API"
  - "https://html.spec.whatwg.org/multipage/form-elements.html#attr-button-command"
autocss_link: "none (conflict: AGENTS.md 'HTML — structure only' uses label + input, no buttons)"
status: outline
---

# Invoker commands: buttons that open dialogs with no script

**Reader question:** Can a button open a dialog or popover without JavaScript?

## Outline

- **Problem:** a click handler written only to open or close something.
- **Native solution:** command and commandfor on a button open dialogs and popovers declaratively.
- **Link out:** MDN Invoker Commands API; the HTML spec.
