---
title: "The hidden-input pattern and its screen-reader traps"
series: "accessibility"
order: 68
reader_question: "I hid the checkbox that drives my CSS. Did I break screen readers?"
standards:
  - "<input> + <label> semantics"
  - "ARIA (what not to add)"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/AGENTS.md (§ HTML — structure only states the fix) [AI-INST: topic only]"
  - "https://github.com/Autocss-com/autocss/issues/101 [issue]"
  - "https://github.com/Autocss-com/cdn/blob/main/index.html (hidden inputs in labels) [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:checked"
  - "https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA"
autocss_link: "HTML — structure only"
status: outline
---

# The hidden-input pattern and its screen-reader traps

**Reader question:** I hid the checkbox that drives my CSS. Did I break screen readers?

## Outline

- **Problem:** hiding the input with display:none, the hidden attribute or aria-hidden removes it from keyboards and screen readers (repos.md P1).
- **Native solution:** hide it visually but keep it focusable; the label names it; :checked still drives the CSS. Test with JAWS.
- **Link out:** MDN :checked and ARIA.
