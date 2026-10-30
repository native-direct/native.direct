---
title: "inert: switch off part of a page without a focus-trap library"
series: "accessibility"
order: 70
reader_question: "How do I make a region unreachable while a dialog is open?"
standards:
  - "inert attribute"
baseline_status_with_date_and_source: "Baseline Widely available 2025-10-11 (Newly 2023-04-11). Source: webstatus.dev id:inert (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/HTML/Reference/Global_attributes/inert"
  - "https://html.spec.whatwg.org/multipage/interaction.html#inert-subtrees"
autocss_link: "none (check against AGENTS.md before linking)"
status: outline
---

# inert: switch off part of a page without a focus-trap library

**Reader question:** How do I make a region unreachable while a dialog is open?

## Outline

- **Problem:** focus-trap libraries and aria-hidden toggling to block the background.
- **Native solution:** the inert attribute makes a subtree unfocusable and non-interactive.
- **Link out:** MDN inert; the HTML spec.
