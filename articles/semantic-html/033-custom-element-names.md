---
title: "Custom element names without JavaScript"
series: "semantic-html"
order: 33
reader_question: "Can I invent a tag like app-logo without customElements.define?"
standards:
  - "Autonomous custom element names"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Custom HTML Elements; cites Jim Nielsen: credit by name and link, URL to add) [OWN, CREDIT]"
  - "https://github.com/dragontheory/D7460N-with-db/blob/main/README.md (Custom HTML Elements bullets) [OWN]"
  - "https://github.com/Autocss-com/cdn/blob/main/index.html [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/html/references/custom-elements.md (when not to invent a tag) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Web_components/Using_custom_elements"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:defined"
autocss_link: "HTML — structure only"
status: outline
---

# Custom element names without JavaScript

**Reader question:** Can I invent a tag like app-logo without customElements.define?

## Outline

- **Problem:** class-heavy wrappers where a named tag would read better.
- **Native solution:** a hyphenated custom name works in HTML and CSS without a script; add a section on when a custom tag is the wrong answer (it has no built-in meaning).
- **Link out:** MDN custom elements guide and :defined.
