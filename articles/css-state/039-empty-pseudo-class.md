---
title: ":empty: show it when the data arrives"
series: "css-state"
order: 39
reader_question: "How do I hide containers that have no content yet?"
standards:
  - ":empty"
  - ":not()"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/README.md (Visibility Logic) [OWN*]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/layout.css [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/css/references/reactivity.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:empty"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:not"
autocss_link: "CSS — the UI runtime"
status: outline
---

# :empty: show it when the data arrives

**Reader question:** How do I hide containers that have no content yet?

## Outline

- **Problem:** empty boxes show borders and gaps before data arrives.
- **Native solution:** :empty hides them; :not(:empty) shows them once filled. Whitespace counts as content (MDN).
- **Link out:** MDN :empty and :not().
