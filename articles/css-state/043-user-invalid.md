---
title: "Form validation without a library: :user-invalid"
series: "css-state"
order: 43
reader_question: "How do I show errors only after the user has typed?"
standards:
  - ":user-valid / :user-invalid"
  - ":invalid"
  - "form:has(:invalid)"
baseline_status_with_date_and_source: ":user-valid / :user-invalid: Baseline Widely available 2026-05-02 (Newly 2023-11-02). Source: webstatus.dev id:user-pseudos (via browser-features.md, as of 2026-10-30)"
sources:
  - "https://github.com/D7460N/DHCP/blob/main/assets/css/forms.css (incl. form:has(:invalid)) [CODE]"
  - "https://github.com/D7460N-ai/D7460N.ai/blob/main/.agents/skills/css/references/inputs.md [AI-INST: topic only]"
references:
  - "https://developer.mozilla.org/docs/Web/CSS/Reference/Selectors/:user-invalid"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:invalid"
  - "https://drafts.csswg.org/selectors-4/#user-pseudos"
autocss_link: "CSS — the UI runtime"
status: outline
---

# Form validation without a library: :user-invalid

**Reader question:** How do I show errors only after the user has typed?

## Outline

- **Problem:** validation libraries and touched flags just to delay error styles.
- **Native solution:** :user-invalid waits for user input; form:has(:invalid) can also flag the submit area.
- **Caveat:** forms.css keys on data-dirty, which nothing sets (repos.md P6); don't copy that part.
- **Link out:** MDN :user-invalid and :invalid; the spec.
