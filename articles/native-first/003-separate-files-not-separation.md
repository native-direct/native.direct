---
title: "Separate files are not separation of concerns"
series: "native-first"
order: 3
reader_question: "My HTML, CSS and JS are in separate files. Aren't they separated?"
standards:
  - "class, id and data-* as cross-layer hooks"
  - "element and state selectors"
baseline_status_with_date_and_source: "n/a: authoring practice"
sources:
  - "https://github.com/D7460N/starter/blob/main/README.md (§ Decoupled to the point of air-gap) [OWN*: re-voice]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/AGENTS.md (§ Architecture Tests) [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Global_attributes"
  - "https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Global_attributes/data-*"
autocss_link: "Architecture Tests"
status: outline
---

# Separate files are not separation of concerns

**Reader question:** My HTML, CSS and JS are in separate files. Aren't they separated?

## Outline

- **Hook:** three files, one rename, three edits.
- **Problem:** a class, id or data-* name shared by HTML, CSS and JS is a wire between layers; cut it and two files break.
- **Native solution:** select by element, attribute meaning and state (:checked, :has(), :empty) instead of invented names.
- **Code idea (described):** the same rule written with a class hook, then with an element-and-state selector.
- **Replaces:** naming conventions used as glue (BEM-style hooks, js- prefixes).
- **His test:** four yes/no questions; any yes means the layers are still wired together.
- **Link out:** MDN global attributes and data-* pages.
