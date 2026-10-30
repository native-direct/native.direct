---
title: "Call your UI like a font: host it once, use it everywhere"
series: "separation-of-concerns"
order: 22
reader_question: "Can a presentation layer be hosted once and used by many sites?"
standards:
  - "Cross-origin CSS and ES modules"
  - "CORS"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/starter/blob/main/docs/compare3.%20md [OWN*]"
  - "https://github.com/Autocss-com/cdn/blob/main/README.md [OWN*]"
  - "https://github.com/Autocss-com/id/blob/main/README.md [CODE]"
  - "https://github.com/Autocss-com/react/blob/main/README.md [CODE, AI-built]"
  - "https://autocss-com.github.io/id/ and https://autocss-com.github.io/react/ (live, 200 on 2026-10-30)"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS"
autocss_link: "Stack"
status: outline
---

# Call your UI like a font: host it once, use it everywhere

**Reader question:** Can a presentation layer be hosted once and used by many sites?

## Outline

- **Problem:** every site copies the same UI code and drifts.
- **Native solution:** host CSS and modules once and link them like a web font (called, not copied); live sites already do this.
- **Caveat:** don't claim the next project costs zero; hosting, content and QA still cost (repos.md A26).
- **Link out:** MDN CORS guide.
