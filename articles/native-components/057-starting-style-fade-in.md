---
title: "Fade in on first paint with @starting-style"
series: "native-components"
order: 57
reader_question: "How do I animate an element as it appears, with no script?"
standards:
  - "@starting-style"
  - "transition-behavior: allow-discrete"
baseline_status_with_date_and_source: "@starting-style: Baseline Newly available 2024-08-06. Source: webstatus.dev id:starting-style (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/transitions.css [CODE]"
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/css/references/starting-style.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/At-rules/@starting-style"
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Properties/transition-behavior"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Fade in on first paint with @starting-style

**Reader question:** How do I animate an element as it appears, with no script?

## Outline

- **Problem:** a script adds a class one frame after insert just to trigger a fade.
- **Native solution:** @starting-style gives the before values, so a normal transition runs on first render; respect reduced motion.
- **Link out:** MDN @starting-style, transition-behavior, prefers-reduced-motion.
