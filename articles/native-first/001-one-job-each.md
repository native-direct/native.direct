---
title: "HTML, CSS and JavaScript: one job each"
series: "native-first"
order: 1
reader_question: "What does separation of concerns mean on the front end?"
standards:
  - "HTML: structure and meaning"
  - "CSS: presentation and UI state"
  - "JavaScript: moving data"
baseline_status_with_date_and_source: ":has(): Baseline Widely available, across browsers since December 2023 (MDN, read 2026-10-30). fetch(): across browsers since March 2017 (MDN browser data, read 2026-10-30)."
sources:
  - "https://github.com/dragontheory/D7460N/blob/main/README.md (Governing Principles) [OWN]"
  - "https://github.com/dragontheory/D7460N-with-db/blob/main/README.md (Separation of Interests) [OWN]"
  - "https://github.com/D7460N/D7460N.dev/blob/main/ADD.md (§ Separation of Concerns) [OWN]"
references:
  - "https://developer.mozilla.org/en-US/docs/Web/HTML (states the three roles)"
  - "https://developer.mozilla.org/en-US/docs/Glossary/MVC (names separation of concerns)"
  - "https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:has"
  - "https://www.w3.org/2001/tag/doc/leastPower.html (W3C TAG, The Rule of Least Power)"
autocss_link: "Stack"
tested: "Chromium (Playwright) 2026-10-30: JavaScript on and off, keyboard arrows. Firefox, Safari, JAWS: not yet"
status: draft (rev 2: facts and technique separated, per his rule)
---

# HTML, CSS and JavaScript: one job each

MDN defines three roles: HTML for the meaning and structure of content, CSS for presentation, JavaScript for behavior. This technique holds each language to one job and narrows JavaScript to moving data. The files share no names except HTML's own elements.

## Facts

| # | Fact | Source |
|---|---|---|
| 1 | HTML defines the meaning and structure of web content. CSS describes appearance. JavaScript describes functionality and behavior. | [MDN: HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) |
| 2 | Separating business logic from display is called separation of concerns. MDN credits it with better division of labor and easier maintenance. | [MDN: MVC](https://developer.mozilla.org/en-US/docs/Glossary/MVC) |
| 3 | The W3C TAG's Rule of Least Power: use the least powerful language that can do the job. | [W3C TAG](https://www.w3.org/2001/tag/doc/leastPower.html) |
| 4 | A class, ID or `data-*` attribute used as a selector is a dependency. Renaming it in the HTML breaks every CSS rule and script that uses it. | Selector matching |
| 5 | Element names and state pseudo-classes (`:checked`, `:empty`, `:has()`) are defined by the HTML and CSS specs, not by your project. | HTML and Selectors specs |
| 6 | `:has()` selects an element by what it contains. | [MDN: :has()](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:has) |

## Technique

| Layer | Job | Never |
|---|---|---|
| HTML | Structure and meaning | `class`, `id`, `data-*`, event attributes |
| CSS | Presentation and all UI state | Depend on anything a script adds |
| JavaScript | Fetch data, write text into existing elements | Show, hide or style anything |

The shared contract is HTML's own element names (facts 4 and 5). Invented names are not part of it. I call this gap between layers the air gap.

## Example: four files

A topic picker. Choose a topic, see its summary.

**index.html**

```html
<main>
  <form>
    <fieldset>
      <legend>Pick a topic</legend>
      <label><input type="radio" name="topic" value="html"> HTML</label>
      <label><input type="radio" name="topic" value="css"> CSS</label>
      <label><input type="radio" name="topic" value="js"> JavaScript</label>
    </fieldset>
  </form>
  <article>
    <h2></h2>
    <p></p>
  </article>
</main>
<script type="module" src="topics.js"></script>
```

**topics.css**

```css
@layer topics {
  article:has(> h2:empty) {
    display: none;
  }

  label:has(> :checked) {
    font-weight: bold;
  }
}
```

**topics.js**

```js
const form = document.querySelector("form");

form.oninput = async (event) => {
  const response = await fetch(`${event.target.value}.json`);
  const topic = await response.json();

  document.querySelector("article h2").textContent = topic.title;
  document.querySelector("article p").textContent = topic.summary;
};
```

**css.json** (one of three data files)

```json
{ "title": "CSS", "summary": "Decides how it looks and which state shows." }
```

### What each file references

| File | References | Does not reference |
|---|---|---|
| index.html | Its own elements | Any CSS rule or script |
| topics.css | Element names, `:checked`, `:empty`, `:has()` | The script, the data |
| topics.js | Element names, the data's keys | Any style or visibility rule |
| css.json | Its own values | The page |

## Results

Tested in Chromium, 2026-10-30.

| Case | Result |
|---|---|
| Page load | Article hidden: `article:has(> h2:empty)` matches |
| Topic chosen | Script writes text. The selector stops matching. Article shows |
| Label state | Checked label turns bold. CSS only |
| Arrow keys | Selection moves between topics. Data updates |
| JavaScript off | Radios and bold label work. Empty article stays hidden |
| Console | No errors |

## What follows from the structure

- **Restyle:** edit topics.css. topics.js has no reference to it, so it needs no change.
- **New data source:** change the fetch URL. The HTML and CSS need no change.
- **Parallel work:** the CSS and the data code share only the HTML. One person can own each. I call these swim lanes.
- **Dependencies:** none. No library, no build step.

## Check your code

1. **HTML:** does changing this markup force a CSS or script change?
2. **CSS:** does a rule depend on a class, ID or anything a script adds?
3. **JavaScript:** does the script show, hide or style anything?
4. **Data:** does the response contain HTML or styling hints?

Each yes is a dependency between layers. The target is four nos.

## Browser support

- `:has()`: Baseline Widely available. Works across browsers since December 2023 ([MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/:has)).

  [![Browser support table for the CSS :has() pseudo-class, from caniuse.com, updated daily](https://caniuse.bitsofco.de/image/css-has.png)](https://caniuse.com/css-has)

- `fetch()`: works across browsers since March 2017 ([MDN](https://developer.mozilla.org/en-US/docs/Web/API/Window/fetch)).

  [![Browser support table for the Fetch API, from caniuse.com, updated daily](https://caniuse.bitsofco.de/image/fetch.png)](https://caniuse.com/fetch)

- The rest is long-supported HTML.

**Next:** [Least Power: HTML first, then CSS, then JavaScript](002-least-power.md) · [Separate files are not separation of concerns](003-separate-files-not-separation.md)

> **[SIGN-UP LINE: email course link goes here once the tool is chosen.]**

---

## Review notes (delete before publishing)

| Item | Status |
|---|---|
| Rev 2 | Rewritten to your rule: facts first (each sourced), then the technique, then tested results. Opinions and generalizations removed ("most code…", "usually", "the work is in the wires", "less to maintain") |
| Your story | Skipped (your call, Oct 30) |
| Support images | caniuse live images (option B, your call Oct 30): no script, updated daily by caniuse.bitsofco.de. Image URLs follow the site's documented pattern; my reader could not open them, so check both render. Each image links to its caniuse page. The text line above each image carries the fact for screen readers |
| Sign-up line (bottom) | Needed. Depends on the email tool decision |
| Facts 4 and 5 | Stated from how selectors and the specs work, no single page cited. Add a spec link if you want one |
| Your tests still to run | Firefox, Safari, JAWS |
| Error handling | None in the snippet (one idea per article). A failed fetch leaves the article hidden. The "no dead ends" article covers it |
| Claims left out | Source READMEs' "100 to 1K times faster" and "50% less code": no proof on file |
| W3C link | Latest-version URL taken from the W3C's dated 2006 copy, which points to it. My reader could not open the latest URL directly |
| "I call this" lines | "Air gap" and "swim lanes" are your named ideas. Keep, rename or cut |
| AI disclosure | Your call |
