---
title: "Same app, built with and without React: what changed"
series: "native-first"
order: 5
reader_question: "What actually changes when you build without a framework?"
standards:
  - "Installed dependency count (measured)"
  - "Source line count (measured)"
baseline_status_with_date_and_source: "n/a: measurement article"
sources:
  - "https://github.com/D7460N/DHCP/issues/66 [OWN]"
  - "https://github.com/D7460N/DHCP [CODE]"
  - "https://github.com/D7460N/DHCP-React [CODE, AI-built]"
  - "https://github.com/D7460N/DHCP-React-2 [CODE, AI-built]"
references:
  - "https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Frameworks_libraries/Main_features"
autocss_link: "Stack"
status: outline
---

# Same app, built with and without React: what changed

**Reader question:** What actually changes when you build without a framework?

## Outline

- **Hook:** one app, built three times.
- **Problem:** the framework debate runs on opinions, not counts.
- **Native solution:** count what you install and must keep updated. His counts (repos.md D14, 2026-10-30): front-end npm dependencies 0 (vanilla) vs 3 + 9 and 19 + 5 (runtime + dev); source lines 4,009 vanilla vs 2,740 and 3,735.
- **Code idea (described):** the count table plus the exact counting method, so readers can repeat it.
- **Replaces:** the frameworks-save-code assumption, and the native-means-less-code claim too: the React builds have fewer lines (repos.md P3). Upkeep is the real cost.
- **Caveat:** both React builds were AI-built; DHCP-React-2's live page returned 404 on 2026-10-30; recount before publishing.
- **Link out:** the three repos; MDN's guide to what frameworks do.
