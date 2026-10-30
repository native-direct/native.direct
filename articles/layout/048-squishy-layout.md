---
title: "Squishy layout: let content set the height"
series: "layout"
order: 48
reader_question: "How do I avoid hard-coded heights and height-polling scripts?"
standards:
  - "Intrinsic height"
  - "overflow"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Squishy Layout, 3 steps) [OWN]"
  - "https://github.com/dragontheory/tmp [CODE]"
  - "https://dragontheory.github.io/tmp/ (live, 200 on 2026-10-30)"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/overflow"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Squishy layout: let content set the height

**Reader question:** How do I avoid hard-coded heights and height-polling scripts?

## Outline

- **Problem:** fixed heights and scripts that measure and resize panels.
- **Native solution:** his three steps: let content size the boxes, and give overflow to the one region that should scroll.
- **Caveat:** the demo uses overflow: overlay, which is non-standard (repos.md D3).
- **Link out:** MDN overflow.
