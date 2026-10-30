---
title: "field-sizing: text boxes that grow without a script"
series: "native-first"
order: 14
reader_question: "How do I make a textarea grow with its content without JavaScript?"
standards:
  - "field-sizing: content"
baseline_status_with_date_and_source: "Baseline Newly available 2026-06-16. Source: webstatus.dev id:field-sizing; web.dev Baseline digest Jun 2026 (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/forms.css (uses field-sizing: content) [CODE]"
  - "https://d7460n.github.io/DHCP/ (live, 200 on 2026-10-30)"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/field-sizing"
  - "https://drafts.csswg.org/css-forms-1/#field-sizing"
  - "https://api.webstatus.dev/v1/features?q=id:field-sizing"
autocss_link: "CSS — the UI runtime"
status: outline
---

# field-sizing: text boxes that grow without a script

**Reader question:** How do I make a textarea grow with its content without JavaScript?

## Outline

- **Hook:** a script that measures a text box on every keystroke.
- **Problem:** autosize scripts read sizes, write heights and fight the browser.
- **Native solution:** one property lets inputs and textareas size to their content.
- **Code idea (described):** a textarea and an input with field-sizing plus minimum and maximum widths in ch.
- **Replaces:** autosize.js-style scripts (browser-features.md).
- **Caveat:** DHCP's forms.css also keys on data-dirty, which no DHCP script sets (repos.md P6); don't copy that part.
- **Link out:** MDN, the spec, webstatus.
