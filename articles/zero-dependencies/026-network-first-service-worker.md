---
title: "A network-first service worker in one small file"
series: "zero-dependencies"
order: 26
reader_question: "How do I keep a site fresh online and working offline?"
standards:
  - "Service Worker API"
  - "Cache API"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/Autocss-com/cdn/blob/main/sw.js [CODE, AI-co]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API"
autocss_link: "JavaScript — data transport only"
status: outline
---

# A network-first service worker in one small file

**Reader question:** How do I keep a site fresh online and working offline?

## Outline

- **Problem:** cache-first workers serve stale pages; frameworks hide the worker inside a plugin.
- **Native solution:** one small network-first worker: try the network, fall back to the cache when offline.
- **Caveat:** sw.js uses addEventListener, which conflicts with his no-addEventListener rule (repos.md P7, autocss#133); explain or fix.
- **Link out:** MDN Service Worker API.
