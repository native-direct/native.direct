# native.direct: article index

Status: outlines only, for review. Date: 2026-10-30.

Counts: first series 15 · backlog 77 in 10 series · files 92.

How to read:
- Baseline status is as of 2026-10-30 unless a file says otherwise. UNVERIFIED = check before publishing.
- Reuse codes from `repos.md`: OWN = his prose (paraphrase) · OWN* = AI-polished (re-voice) · AI-DOC / AI-INST = topic only · CODE = show, credit, verify · CREDIT = name and link the original author.
- Short source names: ADD = https://github.com/D7460N/D7460N.dev/blob/main/ADD.md · DB#n = https://github.com/dragontheory/D7460N-with-db/issues/n · DBR = https://github.com/dragontheory/D7460N-with-db/blob/main/README.md · D7R = https://github.com/dragontheory/D7460N/blob/main/README.md · THOR = https://github.com/dragontheory/THOR/blob/master/README.md · STR = https://github.com/D7460N/starter/blob/main/README.md · CDN = https://github.com/Autocss-com/cdn · DHCP = https://github.com/D7460N/DHCP · AI = https://github.com/Autocss-com/ai
- Full URLs, references and outlines are in each file.

## First series: Native first

Publish in this order. SoC and dependency-free basics first; four Baseline-new features mixed in (006, 011, 013, 014).

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 001 | HTML, CSS and JavaScript: one job each | What does separation of concerns mean on the front end? | Native first | HTML / CSS / JS roles · n/a | D7R; DBR; ADD [OWN] | [001](articles/native-first/001-one-job-each.md) |
| 002 | Least Power: HTML first, then CSS, then JavaScript | How do I choose which language should build a feature? | Native first | Rule of Least Power · n/a | D7R; ADD; DBR [OWN] | [002](articles/native-first/002-least-power.md) |
| 003 | Separate files are not separation of concerns | My HTML, CSS and JS are in separate files. Aren't they separated? | Native first | class / id / data-* coupling · n/a | STR [OWN*]; AI/AGENTS.md [AI-INST] | [003](articles/native-first/003-separate-files-not-separation.md) |
| 004 | Upgrade purgatory: what a package really costs later | What's wrong with just installing a package? | Native first | Dependency cost · Baseline as signal | ADD; DBR; THOR [OWN] | [004](articles/native-first/004-upgrade-purgatory.md) |
| 005 | Same app, built with and without React: what changed | What actually changes when you build without a framework? | Native first | Dependency and line counts · n/a | DHCP#66 [OWN]; DHCP, DHCP-React, DHCP-React-2 [CODE] | [005](articles/native-first/005-same-app-with-and-without-react.md) |
| 006 | CSS nesting is widely available: drop the preprocessor | Do I still need Sass just to nest my CSS? | Native first | CSS nesting · Widely 2026-06-11 | browser-features.md | [006](articles/native-first/006-css-nesting.md) |
| 007 | Inputs fetch data; CSS decides what shows | Why shouldn't a click handler show and hide things? | Native first | :has() · Widely 2026-06-19 | DB#36; DBR [OWN]; DHCP layout.css [CODE] | [007](articles/native-first/007-inputs-fetch-data.md) |
| 008 | The truthful loading state, with no spinner script | How do I show loading without a JavaScript spinner? | Native first | :has() + ::before · Widely 2026-06-19 | ADD [OWN]; DHCP loading.css [CODE] | [008](articles/native-first/008-truthful-loading-state.md) |
| 009 | Never send HTML in your JSON | Is it OK for the API to return HTML strings? | Native first | JSON + textContent · Widely (since 2015, MDN) | AI/AGENTS.md, json skill [AI-INST]; STR [OWN*] | [009](articles/native-first/009-no-html-in-json.md) |
| 010 | Ship the structure once, then stream only the data | Why preload the HTML and send only the content? | Native first | HTML shell + fetch() · Widely (since 2017, MDN) | ADD [OWN]; Autocss-com/id, bible [CODE] | [010](articles/native-first/010-ship-structure-stream-data.md) |
| 011 | @scope is Baseline: scoped styles without BEM or build tools | How do I keep a component's styles from leaking without naming schemes? | Native first | @scope · Newly 2026-03-24 | browser-features.md; AI/AGENTS.md [AI-INST] | [011](articles/native-first/011-css-scope.md) |
| 012 | The details element: the accordion you already have | Do I need a library for an accordion? | Native first | &lt;details&gt; · Widely (since 2020, MDN) | CDN disclosure.css [CODE] | [012](articles/native-first/012-details-accordion.md) |
| 013 | The Popover API: menus and notices without a library | What is the popover attribute, and what can it replace? | Native first | popover · Newly 2025-01-27 | CDN notifications.css [CODE]; menu skill [AI-INST] | [013](articles/native-first/013-popover-api.md) |
| 014 | field-sizing: text boxes that grow without a script | How do I make a textarea grow with its content without JavaScript? | Native first | field-sizing · Newly 2026-06-16 | DHCP forms.css [CODE] | [014](articles/native-first/014-field-sizing.md) |
| 015 | A light, dark and accent theme switcher with zero JavaScript | How do I offer light, dark and accent choices with CSS alone? | Native first | light-dark() + :has() · Newly 2024 / Widely 2026 | color-themes-system [CODE]; DB#4 [OWN] | [015](articles/native-first/015-theme-switcher-zero-js.md) |

## Backlog, by series

Order inside the backlog is not a commitment. Baseline-watch items publish when a status changes, on one stable URL each.

### Separation of concerns (7)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 016 | The self-aware UI: content decides what shows | How can a panel know it has data? | Separation of concerns | :has(), :empty · Widely 2026-06-19 / UNVERIFIED | DB#5; ADD [OWN] | [016](articles/separation-of-concerns/016-self-aware-ui.md) |
| 017 | Developer swim lanes: front end and back end in parallel | How do front-end and back-end developers work in parallel without collisions? | Separation of concerns | JSON contract · n/a | DB#37; ADD [OWN] | [017](articles/separation-of-concerns/017-developer-swim-lanes.md) |
| 018 | Refaced, not replaced: redesign without a rewrite | Why does a redesign usually turn into a rewrite? | Separation of concerns | CSS-only presentation · n/a | ADD [OWN] | [018](articles/separation-of-concerns/018-refaced-not-replaced.md) |
| 019 | Framework-first or user-first: which end do you build from? | Should a project start from the framework or from the user? | Separation of concerns | Architecture direction · n/a | ADD [OWN] | [019](articles/separation-of-concerns/019-framework-first-vs-user-first.md) |
| 020 | Four yes/no questions that prove your layers are decoupled | How do I check whether my layers are actually separate? | Separation of concerns | SoC self-test · n/a | AI/AGENTS.md [AI-INST] | [020](articles/separation-of-concerns/020-four-decoupling-tests.md) |
| 021 | One UI, many datasets: a data-agnostic front end | Can one front end render completely different data? | Separation of concerns | Data-agnostic UI · n/a | D7460N-data [OWN*]; dragontheory/data [OWN] | [021](articles/separation-of-concerns/021-one-ui-many-datasets.md) |
| 022 | Call your UI like a font: host it once, use it everywhere | Can a presentation layer be hosted once and used by many sites? | Separation of concerns | Cross-origin CSS/modules · UNVERIFIED | starter compare3, CDN README [OWN*]; id, react [CODE] | [022](articles/separation-of-concerns/022-call-your-ui-like-a-font.md) |

### Zero dependencies (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 023 | Opinionated means someone else decides | What does an opinionated framework cost you? | Zero dependencies | Framework defaults · n/a | ADD [OWN] | [023](articles/zero-dependencies/023-opinionated-means-someone-else-decides.md) |
| 024 | Double-click index.html: starting with no build step | Do I need a build step to start a project? | Zero dependencies | No build + import maps · Widely 2025-09-27 | tmp, GL2, DHCP READMEs [OWN] | [024](articles/zero-dependencies/024-no-build-step.md) |
| 025 | Self-host your fonts instead of linking Google Fonts | Why not just use the Google Fonts link? | Zero dependencies | @font-face · UNVERIFIED | CDN fonts.css [CODE] | [025](articles/zero-dependencies/025-self-host-fonts.md) |
| 026 | A network-first service worker in one small file | How do I keep a site fresh online and working offline? | Zero dependencies | Service worker · UNVERIFIED | CDN sw.js [CODE] | [026](articles/zero-dependencies/026-network-first-service-worker.md) |
| 027 | PWA basics: a website that installs like an app | What does a PWA give users? | Zero dependencies | Manifest + service worker · UNVERIFIED | ADD [OWN] | [027](articles/zero-dependencies/027-pwa-basics.md) |
| 028 | Measure before you claim: honest front-end performance numbers | Is CSS really 100 to 1000 times faster than JavaScript? | Zero dependencies | Performance budgets · n/a | DBR; ADD; DHCP README [OWN] | [028](articles/zero-dependencies/028-measure-before-you-claim.md) |
| 029 | Less JavaScript, smaller attack surface: a strict CSP from day one | How does an architecture reduce XSS risk? | Zero dependencies | CSP · UNVERIFIED | STR [OWN*]; ADD [OWN] | [029](articles/zero-dependencies/029-strict-csp.md) |
| 030 | Testing a no-build site with a headless browser | How do I test a site that has no toolchain? | Zero dependencies | Headless tests · n/a | CDN test/ [CODE] | [030](articles/zero-dependencies/030-headless-browser-tests.md) |

### Semantic HTML (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 031 | Div-less HTML: what to use instead of div and span | What replaces div and span? | Semantic HTML | Landmark elements · UNVERIFIED | ADD [OWN]; DHCP STYLEGUIDE [OWN*] | [031](articles/semantic-html/031-div-less-html.md) |
| 032 | Classless CSS: styling by meaning, not by names | Can I style a site with no classes? | Semantic HTML | Classless selectors · n/a | ADD [OWN]; color-themes-system [CODE] | [032](articles/semantic-html/032-classless-css.md) |
| 033 | Custom element names without JavaScript | Can I invent a tag like app-logo without customElements.define? | Semantic HTML | Custom element names · UNVERIFIED | ADD; DBR [OWN]; CDN index [CODE] | [033](articles/semantic-html/033-custom-element-names.md) |
| 034 | The semantic app shell: header, nav, main, aside, footer | What does an app skeleton look like in plain semantic HTML? | Semantic HTML | Landmarks · UNVERIFIED | DHCP STYLEGUIDE [OWN*]; CDN index [CODE] | [034](articles/semantic-html/034-semantic-app-shell.md) |
| 035 | Forms done right: fieldset, legend and label | How do I structure an accessible form? | Semantic HTML | fieldset / legend / label · UNVERIFIED | DHCP forms.md [OWN*] | [035](articles/semantic-html/035-forms-fieldset-legend-label.md) |
| 036 | Lists or tables? Picking the right element for a data grid | Should a data grid be a list or a table? | Semantic HTML | table vs list · UNVERIFIED | responsive tables.css, CDN index [CODE] | [036](articles/semantic-html/036-lists-or-tables.md) |
| 037 | Native first, ARIA second | When do I need ARIA at all? | Semantic HTML | Native semantics vs ARIA · n/a | STR; DHCP accessibility.md [OWN*] | [037](articles/semantic-html/037-native-first-aria-second.md) |
| 038 | One meta tag against the dark-mode flash | How do I stop the white flash before my CSS loads? | Semantic HTML | meta color-scheme · UNVERIFIED | DB#4 [OWN]; color-themes-system [CODE] | [038](articles/semantic-html/038-color-scheme-meta.md) |

### CSS state and logic (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 039 | :empty: show it when the data arrives | How do I hide containers that have no content yet? | CSS state and logic | :empty · UNVERIFIED | DHCP CSS README [OWN*]; CDN layout.css [CODE] | [039](articles/css-state/039-empty-pseudo-class.md) |
| 040 | Empty and error states written in CSS | What should users see when data never arrives? | CSS state and logic | :empty::before · UNVERIFIED | DHCP fallbacks.css [CODE] | [040](articles/css-state/040-empty-error-states.md) |
| 041 | Radio buttons as a router, keyboard and screen-reader safe | Can I switch views with no JavaScript and keep them accessible? | CSS state and logic | :checked + :has() · Widely 2026-06-19 / UNVERIFIED | DHCP routing.md [OWN*]; D7460N styles.css, wc [CODE] | [041](articles/css-state/041-radio-router.md) |
| 042 | Layout that counts its children | Can CSS adapt to how many items a row has? | CSS state and logic | Quantity queries · Widely 2026-06-19 / UNVERIFIED | D7460N styles.css [CODE]; ADD [OWN] | [042](articles/css-state/042-quantity-queries.md) |
| 043 | Form validation without a library: :user-invalid | How do I show errors only after the user has typed? | CSS state and logic | :user-invalid · Widely 2026-05-02 | DHCP forms.css [CODE] | [043](articles/css-state/043-user-invalid.md) |
| 044 | Feature detection without Modernizr: @supports selector() | How do I detect support for a CSS feature? | CSS state and logic | @supports selector() · UNVERIFIED | DHCP _browser-support.css [CODE]; ADD [OWN] | [044](articles/css-state/044-feature-detection-supports.md) |
| 045 | Cascade layers: make your defaults easy to override | How do I keep my base styles from fighting everyone else's? | CSS state and logic | @layer · UNVERIFIED | ADD; DB#1 [OWN]; CDN [CODE] | [045](articles/css-state/045-cascade-layers.md) |
| 046 | Zero-specificity resets with :where() | How do I write a reset that anything can override? | CSS state and logic | :where() · UNVERIFIED | CDN inputs, media, reset.css [CODE] | [046](articles/css-state/046-where-resets.md) |

### Layout (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 047 | Holy Grail layout in one grid container | How do I build header, nav, main, aside and footer with one grid? | Layout | CSS Grid areas · UNVERIFIED | DHCP layout docs [OWN*]; CDN layout.css [CODE] | [047](articles/layout/047-holy-grail-one-grid.md) |
| 048 | Squishy layout: let content set the height | How do I avoid hard-coded heights and height-polling scripts? | Layout | Intrinsic height · UNVERIFIED | ADD [OWN]; tmp [CODE] | [048](articles/layout/048-squishy-layout.md) |
| 049 | Only one thing scrolls: scroll containment for app shells | Why does my whole page scroll when only the list should? | Layout | Scroll containers · UNVERIFIED | DHCP CSS docs [OWN*]; ADD [OWN] | [049](articles/layout/049-only-one-thing-scrolls.md) |
| 050 | Master/detail without the ping-pong | How do I stop users bouncing between list and detail pages? | Layout | Grid + :has() · Widely 2026-06-19 | THOR; ADD [OWN]; DHCP layout.css [CODE] | [050](articles/layout/050-master-detail.md) |
| 051 | Intrinsic design: stop thinking in breakpoints | What is intrinsic design, and why skip width breakpoints? | Layout | clamp() / min() / max() · UNVERIFIED | ADD [OWN] | [051](articles/layout/051-intrinsic-design.md) |
| 052 | Container queries or media queries: which one, when | When do I query the container instead of the viewport? | Layout | @container · Widely 2025-08-14 | ADD [OWN]; chained-css-style-queries [CODE] | [052](articles/layout/052-container-vs-media-queries.md) |
| 053 | Logical properties: margin-inline instead of margin-left | Why use margin-inline instead of margin-left? | Layout | Logical properties · UNVERIFIED | ADD [OWN] | [053](articles/layout/053-logical-properties.md) |
| 054 | Full-height app shells on phones: dvh, not 100vh | Why does 100vh break on phones? | Layout | dvh · Widely 2025-06-05 | CDN layout.css, tmp [CODE] | [054](articles/layout/054-dvh-app-shell.md) |

### Native components (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 055 | Animating details open and closed with CSS only | How do I animate a disclosure with CSS? | Native components | ::details-content · Newly 2025-09-16 | CDN disclosure.css [CODE] | [055](articles/native-components/055-animate-details.md) |
| 056 | Styled scrollbars that don't hijack scrolling | How do I style a scrollbar safely? | Native components | scrollbar-color · Newly 2025-12-12 | CDN scrolling.css [CODE]; DB#10 [OWN] | [056](articles/native-components/056-styled-scrollbars.md) |
| 057 | Fade in on first paint with @starting-style | How do I animate an element as it appears, with no script? | Native components | @starting-style · Newly 2024-08-06 | CDN transitions.css [CODE] | [057](articles/native-components/057-starting-style-fade-in.md) |
| 058 | Brand native checkboxes and radios in one line: accent-color | How do I color checkboxes and radios to match my brand? | Native components | accent-color · UNVERIFIED | DHCP a11y.css, color-themes-system [CODE] | [058](articles/native-components/058-accent-color.md) |
| 059 | User-resizable panels without a drag library | Can users resize a panel without a drag library? | Native components | resize · UNVERIFIED | DB#7, DB#25 [OWN]; tmp [CODE] | [059](articles/native-components/059-resizable-panels.md) |
| 060 | Edit in place with contenteditable: when it is enough | When is contenteditable a reasonable editor? | Native components | plaintext-only · Newly 2025-03-04 | DB#25 [OWN]; responsive editable.css [CODE] | [060](articles/native-components/060-contenteditable.md) |
| 061 | The dialog element: modals without a modal library | Do I need a library to build an accessible modal? | Native components | &lt;dialog&gt; · Widely 2024-09-14 | browser-features.md | [061](articles/native-components/061-dialog-element.md) |
| 062 | Invoker commands: buttons that open dialogs with no script | Can a button open a dialog or popover without JavaScript? | Native components | Invoker commands · Newly 2025-12-12 | browser-features.md | [062](articles/native-components/062-invoker-commands.md) |

### Accessibility (8)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 063 | Accessibility is not usability | If my site passes an audit, is it usable? | Accessibility | WCAG vs usability · n/a | ADD; a11y README [OWN] | [063](articles/accessibility/063-accessibility-not-usability.md) |
| 064 | Access problem or usability problem? A decision tree | How do I classify an issue I found? | Accessibility | Triage tree · n/a | a11y README [OWN] | [064](articles/accessibility/064-access-or-usability-decision-tree.md) |
| 065 | Style focus with :focus-visible, never outline: none | How do I style focus without hurting keyboard users? | Accessibility | :focus-visible · UNVERIFIED | ADD [OWN]; CDN a11y.css [CODE] | [065](articles/accessibility/065-focus-visible.md) |
| 066 | No dead ends: every empty or error state needs a way out | What should every error or empty page offer? | Accessibility | No dead ends · n/a | ADD [OWN] | [066](articles/accessibility/066-no-dead-ends.md) |
| 067 | Respect the user's OS settings: motion, contrast, colors | Which user preferences should CSS honor? | Accessibility | User preference media features · UNVERIFIED | STR [OWN*]; CDN color-scheme.css [CODE] | [067](articles/accessibility/067-respect-os-settings.md) |
| 068 | The hidden-input pattern and its screen-reader traps | I hid the checkbox that drives my CSS. Did I break screen readers? | Accessibility | Visually hidden input · n/a | autocss#101; CDN index [CODE] | [068](articles/accessibility/068-hidden-input-traps.md) |
| 069 | Keyboard first: a requirement, not a feature | Is keyboard support a feature or a requirement? | Accessibility | Keyboard access · n/a | DB#40, DB#41; THOR; D7R [OWN] | [069](articles/accessibility/069-keyboard-first.md) |
| 070 | inert: switch off part of a page without a focus-trap library | How do I make a region unreachable while a dialog is open? | Accessibility | inert · Widely 2025-10-11 | browser-features.md | [070](articles/accessibility/070-inert-attribute.md) |

### Data flow (JavaScript as transport) (7)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 071 | One event for everything: oninput | Do I need event listeners everywhere? | Data flow (JavaScript as transport) | input event · UNVERIFIED | CDN app.js, oninput.js [CODE] | [071](articles/data-flow/071-one-event-oninput.md) |
| 072 | A fetch() helper that never crashes the UI | How should a fetch helper handle failure? | Data flow (JavaScript as transport) | fetch() · Widely (since 2017, MDN) | CDN fetch-json.js [CODE] | [072](articles/data-flow/072-fetch-that-never-crashes.md) |
| 073 | JSON keys become element names | How can data map to markup without templates? | Data flow (JavaScript as transport) | Key to tag name · UNVERIFIED | CDN to-tag-name.js [CODE] | [073](articles/data-flow/073-json-keys-element-names.md) |
| 074 | textContent, not innerHTML | Why is innerHTML dangerous? | Data flow (JavaScript as transport) | textContent · Widely (since 2015, MDN) | security skill [AI-INST]; STR [OWN*] | [074](articles/data-flow/074-textcontent-not-innerhtml.md) |
| 075 | A component pool in a template element | How can a page clone only approved elements? | Data flow (JavaScript as transport) | &lt;template&gt; · UNVERIFIED | CDN pool.html [CODE] | [075](articles/data-flow/075-template-component-pool.md) |
| 076 | Come back exactly where you left off with localStorage | How should an app remember user state? | Data flow (JavaScript as transport) | localStorage · UNVERIFIED | DB#30, DB#38 [OWN] | [076](articles/data-flow/076-resume-where-you-left-off.md) |
| 077 | URLPattern: route matching without a router library | Can I match URLs like /posts/:id without a library? | Data flow (JavaScript as transport) | URLPattern · Newly 2025-09-15 | browser-features.md | [077](articles/data-flow/077-urlpattern.md) |

### Maintainability (6)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 078 | The CSS I wrote ten years ago still works | Why are standards a safer long-term bet than libraries? | Maintainability | Web compatibility · n/a | ADD [OWN] | [078](articles/maintainability/078-ten-year-old-css.md) |
| 079 | Why rebuild the same GUI for every client? | Why rebuild the same UI for every new dataset? | Maintainability | Template reuse · n/a | THOR [OWN] | [079](articles/maintainability/079-reinvent-gui.md) |
| 080 | Ramp-up time and the bus factor: keep markup flat | Why do minimal nesting and no obfuscation matter? | Maintainability | Flat markup · n/a | THOR; fishbowl glossary [OWN] | [080](articles/maintainability/080-bus-factor.md) |
| 081 | No abstraction without a reason: when DRY hurts | Is DRY always good? | Maintainability | Abstraction cost · n/a | AI/AGENTS.md [AI-INST] | [081](articles/maintainability/081-no-abstraction-without-reason.md) |
| 082 | Documentation in three tiers: article, README, comments | How should a project document itself? | Maintainability | Docs tiers · n/a | DHCP#44 [OWN] | [082](articles/maintainability/082-docs-three-tiers.md) |
| 083 | The perfect storm: why native-first is ready now | Why is now the moment to go native? | Maintainability | Support milestones · n/a | ADD [OWN] | [083](articles/maintainability/083-perfect-storm.md) |

### Baseline watch (9)

| # | Title | Reader question | Series | Key standard / feature (Baseline) | Main sources | File |
|---|---|---|---|---|---|---|
| 084 | align-content in plain blocks: center without flex or grid | How do I vertically center content in a plain block? | Baseline watch | align-content (block) · Widely 2026-10-16 | browser-features.md | [084](articles/baseline-watch/084-align-content-block.md) |
| 085 | alpha(): change a color's opacity without Sass | How do I make a color token semi-transparent without duplicating it? | Baseline watch | alpha() · Newly 2026-09-14 | browser-features.md | [085](articles/baseline-watch/085-alpha-function.md) |
| 086 | revert-rule: undo one rule without !important | How do I roll back a property without piling on overrides? | Baseline watch | revert-rule · Newly 2026-09-14 | color-themes-system [CODE] | [086](articles/baseline-watch/086-revert-rule.md) |
| 087 | sibling-index() and sibling-count(): stagger without scripts | How do I stagger items without writing an index in JavaScript? | Baseline watch | sibling-index() · Newly 2026-08-18 | D7460N styles.css [CODE] | [087](articles/baseline-watch/087-sibling-index-count.md) |
| 088 | contrast-color(): readable text on any background | How do I pick black or white text for any brand color automatically? | Baseline watch | contrast-color() · Newly 2026-04-10 | DB#4 [OWN] | [088](articles/baseline-watch/088-contrast-color.md) |
| 089 | The Custom Highlight API: highlight text without wrapper spans | How do I highlight search matches without wrapping them in spans? | Baseline watch | Custom highlights · Newly 2026-03-24 | browser-features.md | [089](articles/baseline-watch/089-custom-highlight-api.md) |
| 090 | Same-document view transitions: animate state changes natively | How do I animate between two states of a page without an animation library? | Baseline watch | View transitions · Newly 2025-10-14 | browser-features.md | [090](articles/baseline-watch/090-view-transitions-same-document.md) |
| 091 | content-visibility: skip rendering what nobody can see yet | How do I speed up a long page without virtual-scroll scripts? | Baseline watch | content-visibility · Newly 2025-09-15 | browser-features.md | [091](articles/baseline-watch/091-content-visibility.md) |
| 092 | Container style queries: variant state without scripts | How do I style children from a parent's custom property value? | Baseline watch | Style queries · Newly 2026-05-19 | DHCP diag.css [CODE]; ADD [OWN] | [092](articles/baseline-watch/092-container-style-queries.md) |

## Not indexed yet (pool)

- From `repos.md` (by its row number): #22, #24, #31, #34, #37, #38, #40, #48, #50, #57, #58, #62, #63, #66, #70, #77, #78, #81, #82, #87, #88, #93, #103, M4, M7, M9, M10, M12.
- Merged into indexed rows: #16 → semantic-html 033 · #29 → css-state 041 · #36 → css-state 043 · #42 → css-state 045 · #44 → baseline-watch 086 · #51 → layout 050 · #54 → layout 052 · #76 → accessibility 067 · #92 → zero-dependencies 028.
- From `browser-features.md`, Baseline but not indexed: light-dark() with images, overflow-anchor, ariaNotify(), autocorrect, progress(), declarative shadow DOM, loading=lazy, linear(), name-only container queries, the search element, subgrid, text-indent hanging, shape(), :active-view-transition, Navigation API, root font units, scrollend, view-transition-class, abs()/sign(), print-color-adjust, relative color syntax, text-wrap: balance.
- Not Baseline yet (watch list, not articles): scroll-driven animations and scoped custom element registries (Baseline flip pending, UNVERIFIED), anchor positioning, customizable select, interpolate-size, CSS carousels, scroll-state queries, @function, if(), text-wrap: pretty, cross-document view transitions, and the other non-Baseline rows in `browser-features.md`.
