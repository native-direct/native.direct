---
title: "Ship the structure once, then stream only the data"
series: "native-first"
order: 10
reader_question: "Why preload the HTML and send only the content?"
standards:
  - "Semantic HTML shell"
  - "Fetch API"
baseline_status_with_date_and_source: "fetch(): Baseline Widely available, across browsers since March 2017 (some parts vary). Source: MDN page banner, read 2026-10-30 via MDN MCP"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Separation of Concerns: pre-staged semantic HTML, only content is dynamic) [OWN]"
  - "https://github.com/Autocss-com/id [CODE]"
  - "https://github.com/Autocss-com/bible [CODE]"
  - "https://autocss-com.github.io/id/ and https://autocss-com.github.io/bible/ (content-only sites on one shared front end; 200 on 2026-10-30)"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Window/fetch"
  - "https://fetch.spec.whatwg.org/#fetch-method"
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/main"
autocss_link: "JavaScript — data transport only"
status: outline
---

# Ship the structure once, then stream only the data

**Reader question:** Why preload the HTML and send only the content?

## Outline

- **Hook:** the page that rebuilt its whole layout on every click.
- **Problem:** sending templates with the data mixes structure with content and redraws parts that never change.
- **Native solution:** the semantic shell ships once and can be cached; fetch() brings only values.
- **Code idea (described):** the shell's landmarks listed, then one fetch that fills text into them.
- **Replaces:** client-side template engines and full re-renders for content-only updates.
- **Evidence:** two live sites run on one shared front end with only their content changed.
- **Link out:** MDN fetch() and main; the Fetch spec.
