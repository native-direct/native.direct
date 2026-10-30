---
title: "Least Power: HTML first, then CSS, then JavaScript"
series: "native-first"
order: 2
reader_question: "How do I choose which language should build a feature?"
standards:
  - "Rule of Least Power (W3C TAG principle)"
baseline_status_with_date_and_source: "n/a: design principle"
sources:
  - "https://github.com/dragontheory/D7460N/blob/main/README.md (4-step list) [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Least Power, cites W3C TAG) [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/blob/main/README.md [OWN]"
references:
  - "W3C TAG, The Rule of Least Power (named in ADD.md; URL not in research files: add at review)"
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/details (an HTML-only widget used as the example)"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Least Power: HTML first, then CSS, then JavaScript

**Reader question:** How do I choose which language should build a feature?

## Outline

- **Hook:** [his story] a feature built in JavaScript that HTML already shipped.
- **Problem:** teams reach for the most powerful tool first, then maintain it forever.
- **Native solution:** his 4-step ladder: try HTML, then CSS, then JavaScript, then heavier tools only if all three fail.
- **Code idea (described):** one disclosure built three ways (details element, CSS checkbox, script), with what each costs to keep.
- **Replaces:** JavaScript-by-default habits and widget libraries for things HTML does.
- **Caveat:** Least Power is a selection rule, not a ban; JavaScript still moves data.
- **Link out:** the W3C TAG finding; MDN details page.
