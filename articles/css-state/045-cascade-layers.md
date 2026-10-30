---
title: "Cascade layers: make your defaults easy to override"
series: "css-state"
order: 45
reader_question: "How do I keep my base styles from fighting everyone else's?"
standards:
  - "@layer"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ CSS @LAYER) [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/issues/1 [OWN]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/color-scheme.css (header comment) [CODE]"
  - "https://github.com/Autocss-com/cdn/blob/main/README.md (load order) [OWN*]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@layer"
  - "https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Cascade_layers"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Cascade layers: make your defaults easy to override

**Reader question:** How do I keep my base styles from fighting everyone else's?

## Outline

- **Problem:** base styles with high specificity fight every later rule.
- **Native solution:** put defaults in a layer so unlayered or later styles win; layer order can come from load order, with no master order line.
- **Link out:** MDN @layer and the cascade-layers lesson.
