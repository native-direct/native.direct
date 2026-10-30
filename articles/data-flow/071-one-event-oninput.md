---
title: "One event for everything: oninput"
series: "data-flow"
order: 71
reader_question: "Do I need event listeners everywhere?"
standards:
  - "input event"
  - "event delegation"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/js/app.js (document.oninput) [CODE, AI-co]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/js/oninput.js [CODE, AI-co]"
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/javascript/references/lifecycle.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Element/input_event"
autocss_link: "JavaScript — data transport only"
status: outline
---

# One event for everything: oninput

**Reader question:** Do I need event listeners everywhere?

## Outline

- **Problem:** dozens of listeners, each a place for bugs and leaks.
- **Native solution:** one input handler at the top catches every control change and asks for data.
- **Caveat:** oninput.js also clears the DOM (repos.md D21); check it fits the no-DOM-for-presentation rule.
- **Link out:** MDN input event.
