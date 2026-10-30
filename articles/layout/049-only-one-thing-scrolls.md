---
title: "Only one thing scrolls: scroll containment for app shells"
series: "layout"
order: 49
reader_question: "Why does my whole page scroll when only the list should?"
standards:
  - "overflow"
  - "scroll containers"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/README.md (Scroll Behavior) [OWN*]"
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/STYLEGUIDE.md [OWN*]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Squishy Layout, step 3) [OWN]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Overflow"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Only one thing scrolls: scroll containment for app shells

**Reader question:** Why does my whole page scroll when only the list should?

## Outline

- **Problem:** the whole page scrolls and the header and nav slide away.
- **Native solution:** the shell stays fixed to the viewport; only the content region is a scroll container.
- **Link out:** MDN overflow guide.
