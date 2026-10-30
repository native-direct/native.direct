---
title: "Empty and error states written in CSS"
series: "css-state"
order: 40
reader_question: "What should users see when data never arrives?"
standards:
  - ":empty"
  - "::before content"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/fallbacks.css [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:empty"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/::before"
autocss_link: "No Dead-Ends"
status: outline
---

# Empty and error states written in CSS

**Reader question:** What should users see when data never arrives?

## Outline

- **Problem:** a blank screen when the data never comes.
- **Native solution:** CSS shows a short message and a way forward when a container stays empty.
- **Caveat:** text in CSS content is hard to translate and read by screen readers (repos.md P5).
- **Link out:** MDN :empty and ::before.
