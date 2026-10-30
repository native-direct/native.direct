---
title: "Why rebuild the same GUI for every client?"
series: "maintainability"
order: 79
reader_question: "Why rebuild the same UI for every new dataset?"
standards:
  - "Template reuse (pattern)"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/dragontheory/THOR/blob/master/README.md (commented intro) [OWN]"
references:
  - "none in research files"
autocss_link: "Stack"
status: outline
---

# Why rebuild the same GUI for every client?

**Reader question:** Why rebuild the same UI for every new dataset?

## Outline

- **Problem:** each client gets a new front end for the same kinds of screens.
- **Native solution:** one well-built shell, reused, with only the data changing.
- **Link out:** separation-of-concerns 021 and 022.
