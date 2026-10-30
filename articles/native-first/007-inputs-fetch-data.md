---
title: "Inputs fetch data; CSS decides what shows"
series: "native-first"
order: 7
reader_question: "Why shouldn't a click handler show and hide things?"
standards:
  - ":has()"
  - "input event"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19 (Newly 2023-12-19). Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30); web.dev Baseline digest Jun 2026"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/36 (Self Aware spec) [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/blob/main/README.md (§ Self-aware) [OWN]"
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/layout.css [CODE]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:has"
  - "https://developer.mozilla.org/en-US/docs/Web/API/Element/input_event"
  - "https://drafts.csswg.org/selectors-4/#relational"
autocss_link: "JavaScript — data transport only"
status: outline
---

# Inputs fetch data; CSS decides what shows

**Reader question:** Why shouldn't a click handler show and hide things?

## Outline

- **Hook:** [his story] a handler that fetched data, opened a panel, and left it open and empty when the call failed.
- **Problem:** when JavaScript owns both the data and what is visible, two layers are welded together.
- **Native solution:** the control only asks for data; when data lands in the page, :has() shows the panel; no data, no panel.
- **Code idea (described):** a selector that shows the detail area only while it contains an article.
- **Replaces:** show/hide toggles, isOpen flags, visibility fields in data.
- **Note:** his 2022 spec says buttons; the current AutoCSS rule uses label + input with oninput. Show the current rule (repos.md P7).
- **Link out:** MDN :has() and the input event.
