---
title: "URLPattern: route matching without a router library"
series: "data-flow"
order: 77
reader_question: "Can I match URLs like /posts/:id without a library?"
standards:
  - "URLPattern"
baseline_status_with_date_and_source: "Baseline Newly available 2025-09-15. Source: webstatus.dev id:urlpattern; web.dev Baseline 2025 (via browser-features.md, as of 2026-10-30)"
sources:
  - "none in repos.md"
references:
  - "https://developer.mozilla.org/docs/Web/API/URLPattern"
  - "https://urlpattern.spec.whatwg.org/"
autocss_link: "none (conflict: AutoCSS routes with radio inputs)"
status: outline
---

# URLPattern: route matching without a router library

**Reader question:** Can I match URLs like /posts/:id without a library?

## Outline

- **Problem:** route-matching libraries for a handful of URL shapes.
- **Native solution:** URLPattern matches and extracts parts of a URL natively.
- **Link out:** MDN URLPattern; the spec.
