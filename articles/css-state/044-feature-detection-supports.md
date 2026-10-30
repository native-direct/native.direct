---
title: "Feature detection without Modernizr: @supports selector()"
series: "css-state"
order: 44
reader_question: "How do I detect support for a CSS feature?"
standards:
  - "@supports"
  - "selector()"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing. Note: @supports at-rule() is NOT Baseline (browser-features.md)"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/_browser-support.css [CODE]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ CSS @supports) [OWN]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/css/references/feature-detection.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@supports"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Feature detection without Modernizr: @supports selector()

**Reader question:** How do I detect support for a CSS feature?

## Outline

- **Problem:** a detection library loaded just to ask whether this browser supports X.
- **Native solution:** @supports, including selector(), answers in CSS; his DHCP file swaps in a message when :has() is missing.
- **Link out:** MDN @supports.
