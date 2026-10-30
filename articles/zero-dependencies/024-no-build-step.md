---
title: "Double-click index.html: starting with no build step"
series: "zero-dependencies"
order: 24
reader_question: "Do I need a build step to start a project?"
standards:
  - "Plain files, no toolchain"
  - "Import maps"
baseline_status_with_date_and_source: "Import maps: Baseline Widely available 2025-09-27 (Newly 2023-03-27). Source: webstatus.dev id:import-maps (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/dragontheory/tmp/blob/main/README.md [OWN]"
  - "https://github.com/D7460N/GL2/blob/main/README.md [OWN]"
  - "https://github.com/D7460N/DHCP/blob/main/README.md (To run) [OWN]"
references:
  - "https://developer.mozilla.org/docs/Web/HTML/Reference/Elements/script/type/importmap"
  - "https://html.spec.whatwg.org/multipage/webappapis.html#import-maps"
autocss_link: "Stack"
status: outline
---

# Double-click index.html: starting with no build step

**Reader question:** Do I need a build step to start a project?

## Outline

- **Problem:** new projects start with installs and config before the first line of HTML.
- **Native solution:** open index.html and work; import maps cover bare module names without a bundler.
- **Link out:** MDN import maps; the HTML spec.
