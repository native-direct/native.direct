---
title: "Upgrade purgatory: what a package really costs later"
series: "native-first"
order: 4
reader_question: "What's wrong with just installing a package?"
standards:
  - "Web compatibility: browsers keep old standards working (principle)"
  - "Baseline as the safe-to-use signal"
baseline_status_with_date_and_source: "n/a: about dependencies, not one feature"
sources:
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Minimal Third Party Dependencies, first-person) [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ TL;DR) [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/blob/main/README.md (TL;DR) [OWN]"
  - "https://github.com/dragontheory/THOR/blob/master/README.md (commented intro) [OWN]"
references:
  - "https://web.dev/baseline"
autocss_link: "Stack"
status: outline
---

# Upgrade purgatory: what a package really costs later

**Reader question:** What's wrong with just installing a package?

## Outline

- **Hook:** [his story] one upgrade that stalled a project he worked on.
- **Problem:** each package brings its own release schedule, security fixes and breaking changes that someone else decides.
- **Native solution:** features that ship in browsers need no upgrade work from you; Baseline says when one is safe to use everywhere.
- **Code idea (described):** no code; a short before-you-install checklist (does HTML or CSS already do this? is it Baseline?).
- **Replaces:** install-first habits.
- **Caveat:** no unmeasured speed or size claims (repos.md P3, P4).
- **Link out:** web.dev Baseline.
