---
title: "Developer swim lanes: front end and back end in parallel"
series: "separation-of-concerns"
order: 17
reader_question: "How do front-end and back-end developers work in parallel without collisions?"
standards:
  - "JSON contract as the boundary between teams"
baseline_status_with_date_and_source: "n/a: principle or pattern, not one browser feature"
sources:
  - "https://github.com/dragontheory/D7460N-with-db/issues/37 [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Infrastructure: better defined developer swimlanes, FFE/FBE/BFE/BBE) [OWN]"
references:
  - "https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/JSON"
autocss_link: "JSON — data only"
status: outline
---

# Developer swim lanes: front end and back end in parallel

**Reader question:** How do front-end and back-end developers work in parallel without collisions?

## Outline

- **Problem:** when one component file holds markup, style and data calls, teams wait on each other.
- **Native solution:** the JSON contract is the lane line; each lane ships on its own. Define his four lanes (FFE, FBE, BFE, BBE) in plain words.
- **Link out:** MDN JSON guide.
