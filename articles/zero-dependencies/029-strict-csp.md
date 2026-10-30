---
title: "Less JavaScript, smaller attack surface: a strict CSP from day one"
series: "zero-dependencies"
order: 29
reader_question: "How does an architecture reduce XSS risk?"
standards:
  - "Content-Security-Policy"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/D7460N/starter/blob/main/README.md (§ Secure by design: forbidden-pattern table, CSP block) [OWN*]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (opening quote) [OWN]"
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/security/references/csp.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP"
  - "https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Content-Security-Policy"
autocss_link: "JavaScript — data transport only"
status: outline
---

# Less JavaScript, smaller attack surface: a strict CSP from day one

**Reader question:** How does an architecture reduce XSS risk?

## Outline

- **Problem:** inline scripts, on* attributes and innerHTML force a loose security policy.
- **Native solution:** drop those patterns and a strict CSP fits from day one.
- **Link out:** MDN CSP guide and header reference.
