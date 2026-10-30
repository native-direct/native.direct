---
title: "Testing a no-build site with a headless browser"
series: "zero-dependencies"
order: 30
reader_question: "How do I test a site that has no toolchain?"
standards:
  - "Headless browser regression tests"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/test/README.md [CODE, AI-co]"
  - "https://github.com/Autocss-com/cdn/blob/main/test/package.json (playwright-core) [CODE, AI-co]"
references:
  - "none in research files"
autocss_link: "Stack"
status: outline
---

# Testing a no-build site with a headless browser

**Reader question:** How do I test a site that has no toolchain?

## Outline

- **Problem:** no build sounds like no tests.
- **Native solution:** a headless browser opens the real pages and checks them.
- **Caveat:** playwright-core is a dev-only dependency; say so plainly.
