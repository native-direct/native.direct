---
title: "Self-host your fonts instead of linking Google Fonts"
series: "zero-dependencies"
order: 25
reader_question: "Why not just use the Google Fonts link?"
standards:
  - "@font-face"
  - "font-display"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/css/fonts.css [CODE]"
  - "https://github.com/Autocss-com/autocss/issues/100 [AI-written issue: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@font-face"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@font-face/font-display"
autocss_link: "Stack"
status: outline
---

# Self-host your fonts instead of linking Google Fonts

**Reader question:** Why not just use the Google Fonts link?

## Outline

- **Problem:** a font link is a third-party request on every page load.
- **Native solution:** serve the font files yourself with @font-face and pick a font-display value.
- **Caveat:** two of his own CSS files still import Google Fonts (repos.md P7); fix before citing them.
- **Link out:** MDN @font-face and font-display.
