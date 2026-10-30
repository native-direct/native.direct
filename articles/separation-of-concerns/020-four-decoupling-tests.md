---
title: "Four yes/no questions that prove your layers are decoupled"
series: "separation-of-concerns"
order: 20
reader_question: "How do I check whether my layers are actually separate?"
standards:
  - "Separation-of-concerns self-test"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/Autocss-com/ai/blob/main/AGENTS.md (§ Architecture Tests) [AI-INST: topic only, write fresh]"
references:
  - "https://developer.mozilla.org/en-US/docs/Glossary/MVC"
autocss_link: "Architecture Tests"
status: outline
---

# Four yes/no questions that prove your layers are decoupled

**Reader question:** How do I check whether my layers are actually separate?

## Outline

- **Problem:** we-follow-SoC is easy to say and hard to check.
- **Native solution:** four questions, one per layer (HTML, CSS, JS, JSON); any yes means a hidden wire. Written fresh in his words.
- **Link out:** MDN MVC entry.
