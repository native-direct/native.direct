---
title: "The truthful loading state, with no spinner script"
series: "native-first"
order: 8
reader_question: "How do I show loading without a JavaScript spinner?"
standards:
  - ":has()"
  - "::before"
  - "@keyframes"
  - "prefers-reduced-motion"
baseline_status_with_date_and_source: ":has(): Baseline Widely available 2026-06-19. Source: webstatus.dev id:has (via browser-features.md, as of 2026-10-30). ::before, @keyframes: UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Natural Truthful Loading State) [OWN]"
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/loading.css [CODE]"
  - "https://d7460n.github.io/DHCP/ (live demo, 200 on 2026-10-30)"
  - "https://codepen.io/dragontheory/pen/JjorrKL (link loading; live status unverified) [CODE]"
  - "https://codepen.io/dragontheory/pen/NJOzdX (button loading; live status unverified) [CODE]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:has"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/::before"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@keyframes"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion"
autocss_link: "CSS — the UI runtime"
status: outline
---

# The truthful loading state, with no spinner script

**Reader question:** How do I show loading without a JavaScript spinner?

## Outline

- **Hook:** the spinner that keeps spinning after the request failed.
- **Problem:** a script spinner shows what the code believes, not what the page holds.
- **Native solution:** loading is simply the time a container is still empty; CSS can see that and show a message.
- **Code idea (described):** main without an article gets a short ::before message and a gentle pulse, turned off under reduced motion.
- **Replaces:** spinner libraries and isLoading flags.
- **Caveat:** text in CSS content is hard to translate and read inconsistently by screen readers (repos.md P5); keep it short or use real text.
- **Link out:** MDN :has(), ::before, @keyframes, prefers-reduced-motion; the live demo.
