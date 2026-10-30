---
title: "User-resizable panels without a drag library"
series: "native-components"
order: 59
reader_question: "Can users resize a panel without a drag library?"
standards:
  - "resize"
baseline_status_with_date_and_source: "UNVERIFIED: not in research files; check the MDN banner or webstatus.dev before publishing"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/7 [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/issues/25 [OWN]"
  - "https://github.com/dragontheory/tmp (layout.css, --main-resize-h) [CODE]"
  - "https://codepen.io/dragontheory/pen/JjLvxwO (live status unverified) [CODE]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/resize"
autocss_link: "CSS — the UI runtime"
status: outline
---

# User-resizable panels without a drag library

**Reader question:** Can users resize a panel without a drag library?

## Outline

- **Problem:** drag-to-resize libraries for one panel.
- **Native solution:** the resize property plus overflow gives users a native handle.
- **Link out:** MDN resize.
