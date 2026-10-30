---
title: "Native first, ARIA second"
series: "semantic-html"
order: 37
reader_question: "When do I need ARIA at all?"
standards:
  - "Native HTML semantics"
  - "WAI-ARIA"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/D7460N/starter/blob/main/README.md (§ Accessible by design) [OWN*]"
  - "https://github.com/D7460N/DHCP/blob/main/docs/dev/accessibility.md [OWN*]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA"
  - "https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility/WAI-ARIA_basics"
autocss_link: "HTML — structure only"
status: outline
---

# Native first, ARIA second

**Reader question:** When do I need ARIA at all?

## Outline

- **Problem:** ARIA added on top of the wrong element often makes things worse.
- **Native solution:** use the element that already has the role, state and keyboard behavior; ARIA only fills real gaps.
- **Link out:** MDN ARIA and WAI-ARIA basics.
