---
title: "Never send HTML in your JSON"
series: "native-first"
order: 9
reader_question: "Is it OK for the API to return HTML strings?"
standards:
  - "JSON as data only"
  - "Node.textContent"
  - "Element.innerHTML (what to avoid)"
baseline_status_with_date_and_source: "textContent: Baseline Widely available, across browsers since July 2015. Source: MDN page banner, read 2026-10-30 via MDN MCP"
sources:
  - "https://github.com/Autocss-com/ai/blob/main/AGENTS.md (§ JSON — data only) [AI-INST: topic only]"
  - "https://github.com/Autocss-com/ai/blob/main/.agents/skills/json/references/forbidden.md [AI-INST: topic only]"
  - "https://github.com/D7460N/starter/blob/main/README.md (forbidden-pattern table) [OWN*: re-voice]"
references:
  - "https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/JSON"
  - "https://developer.mozilla.org/en-US/docs/Web/API/Node/textContent"
  - "https://developer.mozilla.org/en-US/docs/Web/API/Element/innerHTML"
  - "https://dom.spec.whatwg.org/#dom-node-textcontent"
autocss_link: "JSON — data only"
status: outline
---

# Never send HTML in your JSON

**Reader question:** Is it OK for the API to return HTML strings?

## Outline

- **Hook:** the quick API that returned ready-made markup.
- **Problem:** HTML in data ties the server to one design and forces innerHTML, which MDN warns can open the door to XSS.
- **Native solution:** send plain values; the page already has the structure; write text with textContent.
- **Code idea (described):** two payloads side by side (markup string vs plain fields) and the one line that fills an element with textContent.
- **Replaces:** server-made fragments in API responses, and sanitizer code written only to clean them.
- **Link out:** MDN JSON guide, textContent, innerHTML; the DOM spec.
