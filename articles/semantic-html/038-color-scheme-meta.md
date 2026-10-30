---
title: "One meta tag against the dark-mode flash"
series: "semantic-html"
order: 38
reader_question: "How do I stop the white flash before my CSS loads?"
standards:
  - "<meta name=\"color-scheme\">"
  - "color-scheme property"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/4 [OWN]"
  - "https://github.com/dragontheory/color-themes-system/blob/main/index.html [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/AGENTS.md (§ HTML — structure only) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/meta/name/color-scheme"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/color-scheme"
autocss_link: "HTML — structure only"
status: outline
---

# One meta tag against the dark-mode flash

**Reader question:** How do I stop the white flash before my CSS loads?

## Outline

- **Problem:** dark-mode users get a white flash before the stylesheet arrives.
- **Native solution:** one meta tag tells the browser both schemes are supported before any CSS loads.
- **Link out:** MDN meta color-scheme and the color-scheme property.
