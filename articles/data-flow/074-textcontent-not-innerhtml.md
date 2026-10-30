---
title: "textContent, not innerHTML"
series: "data-flow"
order: 74
reader_question: "Why is innerHTML dangerous?"
standards:
  - "Node.textContent"
  - "Element.innerHTML"
baseline_status_with_date_and_source: "textContent: Baseline Widely available, across browsers since July 2015. Source: MDN page banner, read 2026-10-30 via MDN MCP"
sources:
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/security/references/sanitization.md [AI-INST: topic only]"
  - "https://github.com/D7460N/starter/blob/main/README.md (forbidden-pattern table) [OWN*]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent"
  - "https://developer.mozilla.org/en-US/docs/Web/API/Element/innerHTML"
autocss_link: "JavaScript — data transport only"
status: outline
---

# textContent, not innerHTML

**Reader question:** Why is innerHTML dangerous?

## Outline

- **Problem:** innerHTML parses whatever it gets, which MDN warns can enable XSS.
- **Native solution:** textContent writes plain text, faster and safe by default.
- **Link out:** MDN textContent and innerHTML. Pairs with native-first 009.
