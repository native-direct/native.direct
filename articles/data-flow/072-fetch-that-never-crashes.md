---
title: "A fetch() helper that never crashes the UI"
series: "data-flow"
order: 72
reader_question: "How should a fetch helper handle failure?"
standards:
  - "fetch()"
  - "Response.ok"
baseline_status_with_date_and_source: "fetch(): Baseline Widely available, across browsers since March 2017 (some parts vary). Source: MDN page banner, read 2026-10-30 via MDN MCP"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/assets/js/fetch-json.js (returns null on failure) [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Window/fetch"
  - "https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch"
autocss_link: "JavaScript — data transport only"
status: outline
---

# A fetch() helper that never crashes the UI

**Reader question:** How should a fetch helper handle failure?

## Outline

- **Problem:** fetch does not reject on 404 or 500 (MDN), so naive code treats error pages as data.
- **Native solution:** check response.ok, return nothing on failure, let CSS show the empty state, and fix the API rather than mocking around it.
- **Link out:** MDN fetch() and Using Fetch.
