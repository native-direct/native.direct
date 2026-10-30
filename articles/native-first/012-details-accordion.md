---
title: "The details element: the accordion you already have"
series: "native-first"
order: 12
reader_question: "Do I need a library for an accordion?"
standards:
  - "<details> and <summary>"
  - "name attribute (one open at a time)"
  - ":open"
baseline_status_with_date_and_source: "<details>: Baseline Widely available, across browsers since January 2020 (some parts vary). Source: MDN page banner, read 2026-10-30 via MDN MCP. :open: Newly 2026-05-11, webstatus.dev id:open-pseudo (via browser-features.md, as of 2026-10-30). name attribute: UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/disclosure.css [CODE, AI-co]"
  - "https://autocss-com.github.io/cdn/ (live, 200 on 2026-10-30)"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/details"
  - "https://html.spec.whatwg.org/multipage/interactive-elements.html#the-details-element"
autocss_link: "HTML — structure only"
status: outline
---

# The details element: the accordion you already have

**Reader question:** Do I need a library for an accordion?

## Outline

- **Hook:** an accordion plugin for something HTML ships.
- **Problem:** libraries rebuild open/close, keyboard support and state that the browser already gives you.
- **Native solution:** details and summary toggle with mouse and keyboard; giving several the same name lets only one stay open (MDN).
- **Code idea (described):** three details elements sharing one name, styled with the :open state.
- **Replaces:** accordion and disclosure plugins.
- **His test:** [his JAWS check] what a screen reader announces when one opens.
- **Link out:** MDN details page and the HTML spec. Animation comes later (native-components 055).
