---
title: "Lists or tables? Picking the right element for a data grid"
series: "semantic-html"
order: 36
reader_question: "Should a data grid be a list or a table?"
standards:
  - "<table>, <thead>, header cells"
  - "<ul>/<li>"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/dragontheory/responsive/blob/main/assets/css/tables.css [CODE]"
  - "https://github.com/Autocss-com/cdn/blob/main/index.html (header ul[aria-hidden]) [CODE]"
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/STYLEGUIDE.md [OWN*]"
  - "https://github.com/D7460N/DHCP/blob/main/docs/architecture/accessibility-checklist-ready.md [AI-DOC: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/table"
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/thead"
autocss_link: "HTML — structure only"
status: outline
---

# Lists or tables? Picking the right element for a data grid

**Reader question:** Should a data grid be a list or a table?

## Outline

- **Problem:** list-based grids with a hidden header row lose the link between headers and cells (repos.md P2).
- **Native solution:** tabular data goes in a table; lists suit cards. His own checklist says the same.
- **Caveat:** AutoCSS rows are ul/li; resolve this bridge conflict before writing.
- **Link out:** MDN table and thead.
