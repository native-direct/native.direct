---
title: "JSON keys become element names"
series: "data-flow"
order: 73
reader_question: "How can data map to markup without templates?"
standards:
  - "Custom element names from data keys"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/js/to-tag-name.js [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/data-flow/references/totagname.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Web_components/Using_custom_elements"
autocss_link: "HTML — structure only"
status: outline
---

# JSON keys become element names

**Reader question:** How can data map to markup without templates?

## Outline

- **Problem:** template engines map each field to markup by hand.
- **Native solution:** turn each key into a valid custom element name and put the value inside as text.
- **Link out:** MDN custom elements guide (naming rules).
