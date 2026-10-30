---
title: "Radio buttons as a router, keyboard and screen-reader safe"
series: "css-state"
order: 41
reader_question: "Can I switch views with no JavaScript and keep them accessible?"
standards:
  - ":checked"
  - ":has()"
  - "<input type=radio> + <label>"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19 (Newly 2023-12-19). Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30). :checked: UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/docs/dev/routing.md [OWN*]"
  - "https://github.com/dragontheory/D7460N/blob/main/assets/css/styles.css [CODE]"
  - "https://github.com/dragontheory/wc/blob/main/index.html [CODE]"
  - "https://github.com/dragontheory/D7460N-with-db/issues/27 (checkbox state machine) [OWN]"
  - "https://github.com/Autocss-com/autocss/issues/101 (accessibility defect) [issue]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:checked"
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/input"
autocss_link: "HTML — structure only"
status: outline
---

# Radio buttons as a router, keyboard and screen-reader safe

**Reader question:** Can I switch views with no JavaScript and keep them accessible?

## Outline

- **Problem:** view switching usually means a router library.
- **Native solution:** a radio group plus :has(:checked) shows one view at a time; checkboxes give on/off state the same way.
- **Caveat:** his earlier hidden inputs broke keyboard and screen-reader access (repos.md P1, autocss#101); show the fixed pattern and test with JAWS.
- **Link out:** MDN :checked and input.
