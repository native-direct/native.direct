---
title: "Zero-specificity resets with :where()"
series: "css-state"
order: 46
reader_question: "How do I write a reset that anything can override?"
standards:
  - ":where()"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/inputs.css [CODE]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/media.css [CODE]"
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/reset.css [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:where"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Zero-specificity resets with :where()

**Reader question:** How do I write a reset that anything can override?

## Outline

- **Problem:** resets that need !important to beat later rules.
- **Native solution:** wrap reset selectors in :where() so they carry zero specificity.
- **Link out:** MDN :where().
