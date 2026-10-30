---
title: "A component pool in a template element"
series: "data-flow"
order: 75
reader_question: "How can a page clone only approved elements?"
standards:
  - "<template>"
  - "cloneNode()"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/pool.html [CODE, AI-co]"
  - "https://github.com/Autocss-com/cdn/blob/main/README.md (called, not copied) [OWN*]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/template"
autocss_link: "HTML — structure only"
status: outline
---

# A component pool in a template element

**Reader question:** How can a page clone only approved elements?

## Outline

- **Problem:** scripts that build elements from strings.
- **Native solution:** keep approved elements in a template and clone them; nothing else gets made.
- **Link out:** MDN template.
