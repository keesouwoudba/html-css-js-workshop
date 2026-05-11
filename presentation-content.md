# Workshop Slides — Full Text Breakdown (Updated)

---

> **Global note for all slides:** If a slide's content is too long to fit comfortably, split it into two slides and add a **"Next →"** button at the bottom of the first that reveals or navigates to the second. Never crowd a slide — breathing room is part of teaching.

---

## SLIDE 1 — Title Slide

**Layout:** Centered vertically and horizontally. Title large, subtitle smaller beneath it. Workshop info at the very bottom.

**Title:** Building for the Web: HTML, CSS & JavaScript

**Subtitle:** A hands-on workshop

**Bottom:** _Today we build something real._

---

## SLIDE 2 — The Big Picture

**Layout:** Title at top. Three items stacked vertically in the center, each with an emoji, bold label, and one-line description. Italic note pinned to the bottom.

**Title:** Three languages. Three jobs.

🦴 **HTML** — The skeleton. Pure content and structure. Text, buttons, images. No color, no layout, no behavior. Just: what is on the page.

🎨 **CSS** — The stylist. Takes that skeleton and makes it look good. Colors, fonts, layout, spacing.

🧠 **JavaScript** — The brain. The only real programming language of the three. Makes the page react to what the user does.

_When you open Google: the search box is HTML. The rounded corners are CSS. The suggestions appearing as you type — that's JavaScript._

---

## SLIDE 3 — How They Connect

**Layout:** Title at top. File list left-aligned in a code block, centered on the page. Explanation text below it. Live example block beneath that — full width, scrollable if needed.

**Title:** One page, three files

```
index.html      ← the page itself
styles.css      ← linked from HTML
script.js       ← linked from HTML
```

HTML is the entry point. CSS and JavaScript are attached to it. The browser loads `index.html`, sees the links, fetches the other files, and applies them.

> 📌 _Here should be a live code block: a minimal index.html with link to styles.css and script.js, showing all three files side by side and the rendered result in the browser._

---

---

# PART 1 — HTML

---

## SLIDE 4 — The HTML File

**Layout:** Title at top. Code block centered and takes up ~55% of the slide width. Bullet list of explanations to the right of the code block OR stacked below if space is tight. "Run this" note at very bottom in a distinct color.

**Title:** Every webpage is just a text file

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Page</title>
    <link rel="stylesheet" href="styles.css" />
    <script src="script.js" defer></script>
  </head>
  <body>
    <h1>Hello, world!</h1>
    <p>This is my first page.</p>
  </body>
</html>
```

- `<!DOCTYPE html>` — tells the browser: use modern HTML
- `<head>` — invisible zone: title, CSS links, JS links
- `<body>` — everything the user actually sees
- `<title>` — the text in the browser tab

> 📌 _Run this live. Point to the tab showing the title. Point to the body showing the text._

---

## SLIDE 5 — Tags & Attributes

**Layout:** Title at top. Short paragraph explanation. Two code blocks side by side — first showing a basic tag, second showing a tag with attributes. Brief attribute explanation below.

**Title:** How HTML is written

Every HTML instruction is a **tag**: `<p>` to open, `</p>` to close.

```html
<p>This is a paragraph.</p>
<a href="https://google.com" target="_blank">Go to Google</a>
```

**Attributes** give extra information to a tag:

- `href` — where the link goes
- `target="_blank"` — open in new tab

_If you forget an attribute, the element still shows — it just won't behave correctly._

---

## SLIDE 6 — Text Tags

**Layout:** Title at top. Code block on the left side taking ~50% width. To the right: brief explanation of each tag group (headings, formatting, breaks). Note at bottom.

**Title:** Putting text on a page

```html
<h1>Main Title</h1>
<h2>Section Title</h2>
<h3>Smaller Section</h3>
<p>A paragraph of text.</p>

<strong>Bold</strong>
<em>Italic</em>
<u>Underline</u>
<s>Strikethrough</s>

<br />
← line break
<hr />
← horizontal line
```

`h1` through `h6` are headings. The browser gives them size automatically — no CSS needed. `strong`, `em`, `u`, `s` are inline formatters — they wrap around words inside text.

> 📌 _Live code: write all of these, show the result. Ask: what happens if we use h1 twice? Nothing technically breaks — but it's bad practice for SEO._

---

## SLIDE 7 — Links & Images

**Layout:** Title at top. Code block centered. Explanations as two bullet groups below: one for `<a>`, one for `<img>`. Note at bottom.

**Title:** Connecting pages and showing pictures

```html
<a href="https://google.com">Go to Google</a>
<a href="about.html">Go to About page</a>

<img src="photo.jpg" alt="A sunset photo" />
```

**Links `<a>`:**

- `href` is the destination — a URL or a relative file path
- Relative means: look for this file next to the current HTML file

**Images `<img>`:**

- No closing tag needed
- `src` is the path to the image file
- `alt` is what shows if image fails, and what screen readers read

> 📌 _Live: create two HTML files, link between them. Drop an image in the folder and display it._

---

## SLIDE 8 — div and span

**Layout:** Title at top. Two-column layout below:

- **Left column (~55%):** explanation text + code blocks (one for div, one for span)
- **Right column (~45%):** the image displayed vertically centered, max-height constrained so it doesn't overpower the slide. Add a small caption beneath it: _"div vs span — visual difference"_

Image: `https://images.squarespace-cdn.com/content/v1/62d7afdd0711b76729174013/295d89b3-7d36-41bc-b280-d5443c29507f/divspan.png?format=500w`

**Title:** The most used tags in the world

`<div>` and `<span>` have zero visual meaning on their own. They're blank containers you use to group things and apply CSS to.

```html
<div class="card">
  <h2>Product Name</h2>
  <p>Description here.</p>
</div>

<p>The price is <span class="price">$9.99</span> today only.</p>
```

- **`<div>`** — block level. Takes up full width. Starts on a new line. Think of it as a box.
- **`<span>`** — inline. Sits inside text without breaking the line. Think of it as a highlighter pen.

> 📌 _Live: three divs stacked. Then a paragraph with a span coloring one word._

---

## SLIDE 9 — id and class

**Layout:** Title at top. Code block centered. Two-column explanation below — left: id, right: class. Brief note at bottom in italics.

**Title:** How you target elements from CSS and JS

```html
<h1 id="mainTitle">Hello</h1>

<div class="card">Card One</div>
<div class="card">Card Two</div>
<div class="card featured">Card Three</div>
```

| `id`                  | `class`                |
| --------------------- | ---------------------- |
| Unique — one per page | Shared — many elements |
| Like a name badge     | Like a team uniform    |
| Used with `#` in CSS  | Used with `.` in CSS   |

One element can have multiple classes, space-separated: `class="card featured"`

_This will make complete sense in 10 minutes when we reach CSS selectors._

---

## SLIDE 10 — Lists & Forms _(reference slide)_

**Layout:** Title at top. Code block centered showing all examples. Short explanation below. Reference link in a visually distinct box or highlighted text at the very bottom.

**Title:** Lists and Form inputs — a quick introduction

```html
<ul>
  <li>Item</li>
  ← unordered (bullets)
</ul>

<ol>
  <li>Step 1</li>
  ← ordered (numbered)
</ol>

<input type="text" placeholder="Your name" />
<input type="email" />
<input type="checkbox" />
<button>Submit</button>
<textarea></textarea>
<select>
  <option>Option A</option>
</select>
```

These are the building blocks of every form you'll ever see on the web. We won't go deep today — forms get interesting when connected to a backend, which is its own topic entirely.

**If you want to explore every input type with explanations and live examples, it's all waiting for you at: [study guide link]**

---

## SLIDE 11 — Semantic Tags _(reference slide)_

**Layout:** Title at top. Code block left-aligned. Short explanation right or below. Reference link in distinct box at bottom.

**Title:** Writing HTML that means something

Semantic tags work exactly like `<div>` — same behavior, just a more descriptive name.

```html
<header>
  ← top of page
  <nav>
    ← navigation links
    <main>
      ← main content
      <section>
        ← a chunk of content
        <article>
          ← standalone piece (blog post, card)
          <aside>
            ← sidebar
            <footer>← bottom of page</footer>
          </aside>
        </article>
      </section>
    </main>
  </nav>
</header>
```

The page looks identical whether you use `<div>` or `<header>`. The difference is that Google's crawler and screen readers for blind users can understand the structure of your page.

We won't focus on this today, but it's good practice in real projects. **Full guide at: [study guide link]**

---

---

# PART 2 — CSS

---

## SLIDE 12 — Connecting CSS

**Layout:** Title at top. Two code blocks side by side — left: the HTML link tag, right: the CSS file content. Short explanation below. Note at bottom.

**Title:** How CSS reaches HTML

```html
<!-- In your <head> -->
<link rel="stylesheet" href="styles.css" />
```

```css
/* styles.css */
p {
  color: blue;
  font-size: 20px;
}
```

One line in HTML and the browser applies every rule in that CSS file to the entire page.

**The syntax:** selector → curly braces → property: value → semicolon after every value.

> 📌 _Live: create styles.css, link it, change paragraph color. Show how removing the link removes all styles instantly._

---

## SLIDE 13 — Selectors

**Layout:** Title at top. Code block centered, takes ~60% of slide width. Brief explanation paragraph below. Note at bottom.

**Title:** Telling CSS what to style

```css
p {
} /* every <p> */
.card {
} /* everything with class="card" */
#title {
} /* the element with id="title" */
h1,
h2,
h3 {
} /* multiple at once */
.card p {
} /* only <p> elements INSIDE .card */

button:hover {
} /* only when mouse is over it */
button:active {
} /* only while being clicked */
```

The priority rule: `id` beats `class`, `class` beats tag name. When two rules conflict, the more specific one wins.

> 📌 _Live: style all paragraphs blue. Add a class to one and make it red. Show the class wins._

---

## SLIDE 14 — Colors

**Layout:** Title at top. Code block centered. Short paragraph explanation below. Note at bottom.

**Title:** Four ways to say "red"

```css
color: red; /* name */
color: rgb(255, 0, 0); /* red, green, blue — each 0 to 255 */
color: rgba(255, 0, 0, 0.5); /* same + transparency: 0=invisible, 1=solid */
color: #ff0000; /* hex — same as RGB, just shorter */
```

All four produce the same result. Use whichever feels readable. `rgba` is especially useful when you want partial transparency — like a dark overlay on a hero image.

> 📌 _Live: four divs, same red written four different ways. They look identical._

---

## SLIDE 15 — Backgrounds

**Layout:** Title at top. Code block on the left (~55%). To the right: a visual showing cover vs contain behavior (placeholder image in a fixed box). Explanation below the code.

**Title:** Filling elements with color or image

```css
background-color: lightblue;
background-color: rgba(0, 0, 0, 0.5);

background-image: url("photo.jpg");
background-size: cover; /* fills the space, crops if needed */
background-size: contain; /* fits inside, may leave gaps */
background-position: center;
```

`background-size: cover` is your go-to for hero sections and card backgrounds. Think of fitting a photo into a frame — the frame always fills, and the edges crop if needed.

> 📌 _Live: a div with fixed width and height, background image. Toggle cover vs contain. See the difference._

---

## SLIDE 16 — Text & Fonts

**Layout:** Title at top. Code block left, taking ~55% width. Bullet explanation list on the right for font-family stack and text-decoration note. Note at bottom. If too crowded, split into Slide 16a (font-family, size, weight, style, color) and Slide 16b (alignment, decoration, transform, spacing) with a Next → button.

**Title:** Controlling how text looks

```css
font-family: Roboto, Arial, sans-serif;
font-size: 16px;
font-weight: normal; /* or: bold */
font-style: italic;
color: black;

text-align: left / center / right;
text-decoration: none;
text-decoration: underline;
text-decoration: line-through;

text-transform: uppercase / lowercase / capitalize;
line-height: 1.5;
```

`font-family` with multiple values is a safety net — try the first, fall back to the next if unavailable. `text-decoration: none` is something you'll write constantly: it removes the default underline from `<a>` tags.

> 📌 _Live: import a Google Font, apply it. Toggle text-align. Show text-decoration: none on a link._

---

## SLIDE 17 — Sizing

**Layout:** Title at top. Code block centered. Explanation below. The live demo note links to a **separate page** that opens in a new tab — show this as a clearly styled button or link: "Open live demo →". Do NOT inline the demo on this slide.

**Title:** Setting width and height

```css
width: 200px; /* fixed — always 200px */
width: 50%; /* relative — 50% of the parent's width */
width: 100vw; /* 100% of the browser window width */
max-width: 600px; /* never wider than this */

height: 100px;
height: 100vh; /* 100% of the browser window height */
min-height: 200px;
```

`max-width` is something you'll use in almost every project. It lets an element shrink on small screens but prevents it from stretching to 2000px on a huge monitor.

> 📌 **[Open live demo →]** _(opens in a new tab — a resizable div with width: 50% and max-width: 400px. Resize the browser window and watch it shrink but stop at 400px.)_

---

## SLIDE 18 — The Box Model _(split across 2 slides)_

---

### SLIDE 18a — Box Model: Concept

**Layout:** Title at top. Text explanation in center-left. The MDN box model image on the right, constrained to ~45% slide width, vertically centered. The image is horizontal/rectangular so give it full width within its column. Caption beneath: _"Source: MDN Web Docs"_

Image: `https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Box_model/boxmodel.png`

**Title:** The Box Model — Every element is a box

This is one of the most important concepts in CSS. Every element — every button, div, paragraph — is a rectangle made of four layers:

```
[ margin   ]      ← space OUTSIDE, pushes other elements away
  [ border ]      ← the outline
    [ padding ]   ← space INSIDE, between content and border
      [ content ] ← the actual text or image
```

> **Next →** _(button at bottom right to go to Slide 18b)_

---

### SLIDE 18b — Box Model: Code

**Layout:** Title at top. Code block centered taking ~65% width. Two key callout notes below — one for box-sizing trap, one for the reset rule. Note at bottom.

**Title:** The Box Model — Writing it in CSS

```css
padding: 10px 20px 30px 40px; /* top right bottom left */
padding-top: 10px;
padding-right: 20px;
padding-bottom: 30px;
padding-left: 40px;

margin: 10px 20px 30px 40px;
margin: auto; /* centers the element horizontally */

border: 1px solid black;
border: 2px dashed red;
border: none;
border-radius: 5px;
border-radius: 50%;

box-sizing: border-box; /* ← always add this */
```

⚠️ **The trap:** a div with `width: 200px` and `padding: 20px` ends up being 240px wide by default. `box-sizing: border-box` fixes this — padding counts _inside_ the stated width.

Put this at the top of every CSS file:

```css
* {
  box-sizing: border-box;
}
```

> 📌 _Live: show broken behavior without border-box. Add it, see the fix. Open DevTools and show the box model diagram._

---

## SLIDE 19 — Display

**Layout:** Title at top. Code block centered. Key callout below: the none vs opacity difference in a small two-column comparison box. Note at bottom.

**Title:** Block, inline, and none

```css
display: block; /* full width, new line (default: div, p, h1) */
display: inline; /* sits in text, no width/height control (span, a) */
display: inline-block; /* inline but you CAN set width and height */
display: none; /* completely removed — not just invisible */
display: flex; /* flexbox — next slide */
```

| `display: none`              | `opacity: 0`                         |
| ---------------------------- | ------------------------------------ |
| Element vanishes completely  | Element invisible but space reserved |
| Other elements close the gap | Other elements do NOT move           |

> 📌 _Live: three divs. Set display: none on the middle one. The third div jumps up to fill the gap._

---

## SLIDE 20 — Flexbox _(split across 2 slides)_

---

### SLIDE 20a — Flexbox: Container

**Layout:** Title at top. Short concept paragraph. Code block centered (~60% width). Three live demo link buttons at the bottom in a row, each opening a new tab. Label them clearly.

**Title:** Flexbox — The layout system you'll use every day

Before Flexbox, centering something vertically in CSS was notoriously painful. Flexbox solved layout.

You apply it to a **container**. It controls how the children inside are arranged.

```css
display: flex;

flex-direction: row; /* children left to right — default */
flex-direction: column; /* children top to bottom */

justify-content: center;
justify-content: space-between;
justify-content: flex-start;
justify-content: flex-end;
justify-content: space-around;
justify-content: space-evenly;

align-items: center;
align-items: flex-start;
align-items: stretch;

gap: 16px;
```

> 📌 **Live demos — open each in a new tab:**
>
> **[Demo 1: justify-content →]** _(three divs in a row, toggle every justify-content value)_
>
> **[Demo 2: align-items →]** _(fixed-height container, toggle every align-items value)_
>
> **[Demo 3: flex-direction →]** _(toggle row vs column, show how justify/align axes swap)_

> **Next →** _(button to Slide 20b)_

---

### SLIDE 20b — Flexbox: Children

**Layout:** Title at top. Code block centered. Short explanation below. Note at bottom.

**Title:** Flexbox — Controlling individual items

```css
/* Applied to the children inside the flex container */
flex: 1; /* take equal share of remaining space */
flex: 2; /* take twice the space of a flex: 1 item */
flex-shrink: 0; /* don't shrink even if container is too small */
```

```html
<div style="display: flex;">
  <div style="width: 100px;">Fixed</div>
  <div style="flex: 1;">Takes remaining space</div>
  <div style="flex: 2;">Takes twice as much</div>
</div>
```

A sidebar layout in one line: fixed-width sidebar on the left, `flex: 1` content area on the right.

> 📌 _Live: build a sidebar layout using flex: 1. Then show a navigation bar with logo on left and links pushed right using `margin-left: auto` on the last item._

---

## SLIDE 21 — Position: relative & absolute

**Layout:** Title at top. Code blocks for relative and absolute separated with a label each. The card+badge example at the bottom as both code AND a rendered visual block side by side. Note at bottom.

**Title:** Placing elements precisely

```css
position: relative; /* stays in flow — becomes a reference point for children */

position: absolute; /* removed from flow — positioned relative to nearest
                        non-static parent */
top: 0;
right: 0;
bottom: 0;
left: 0;
```

**The most common pattern:** `relative` on parent + `absolute` on child = place something in a corner.

```html
<div
  style="position: relative; width: 200px; height: 200px; background: lightblue;"
>
  <span
    style="position: absolute; top: 5px; right: 5px;
               background: red; color: white; padding: 2px 8px;"
  >
    NEW
  </span>
  Card content
</div>
```

> 📌 _Live: build this badge. Then remove position: relative from the parent — watch the badge fly to the page corner. That's the moment people understand position._

---

## SLIDE 22 — Position: fixed & sticky _(reference slide)_

**Layout:** Title at top. Two sections stacked: fixed (top half) and sticky (bottom half) each with a one-line explanation and a link to the live interactive demo. Keep text minimal.

**Title:** Two more position values worth knowing

**`position: fixed`** — the element is pulled out of the flow and stuck to the browser window. It doesn't scroll. Classic use: a navigation bar that always stays at the top.

> 📌 _Here should be a scrollable demo page: lots of content with a fixed nav at the top. Scroll and see the nav stay put._

---

**`position: sticky`** — acts completely normal as you scroll, until the element hits a threshold — say, the top of the screen — then it stops there and sticks while the rest scrolls under it. Classic use: section headings that stay visible while their section is in view.

> 📌 _Here should be a scrollable demo page: multiple sections with sticky `<h2>` headings._

These are useful patterns but take a little time to internalize. **If you want to explore both with interactive examples, head to: [study guide link]**

---

## SLIDE 23 — Opacity, Shadows, Cursor _(reference slide)_

**Layout:** Title at top. Three sections stacked. Each has: label, one-line explanation, a small inline visual example block. Reference link at bottom in distinct styling.

**Title:** A few small but useful properties

**`opacity`** — controls transparency. `1` = fully visible. `0` = invisible but still takes up space.

---

**`box-shadow`** — adds a shadow behind an element:

```css
box-shadow: 2px 4px 8px rgba(0, 0, 0, 0.2);
/*           ↑    ↑    ↑         ↑
           right down blur  color+transparency  */
```

> 📌 _Here should be three cards side by side: no shadow, soft shadow (large blur), hard shadow (zero blur). So they can see the difference visually._

---

**`cursor: pointer`** — shows the hand cursor on hover. Always add this to anything you make clickable via JavaScript. Divs don't get the pointer cursor automatically — only real buttons do.

We won't go deep on these today. **Full explanation and interactive examples at: [study guide link]**

---

---

# PART 3 — JAVASCRIPT

---

## SLIDE 24 — JavaScript in the Browser

**Layout:** Title at top. Short paragraph center. One-line code block showing the script tag. Bullet explanation below. Note at bottom.

**Title:** The only language that runs in the browser

JavaScript is not Java. The name was a 1995 marketing decision. Every browser has a JS engine built in — Chrome uses V8, Firefox uses SpiderMonkey. Your code compiles and runs right inside the tab.

```html
<script src="script.js" defer></script>
```

`defer` means: load the file, but wait until HTML is fully parsed before running. This prevents JS from running before the elements it needs to touch actually exist.

> 📌 _Live: create script.js. Add `console.log("hello")`. Open DevTools → Console (F12). Show it._

---

## SLIDE 25 — Variables

**Layout:** Title at top. Code block centered. Short explanation below for let vs const. Red callout box: "Don't use var." Note at bottom.

**Title:** Storing values

```js
let name = "Alice"; // can be reassigned
const PI = 3.14; // cannot be reassigned — throws an error if you try

let num = 42;
let text = "hello";
let flag = true;
let nothing = null;
let notDefined; // declared but no value — undefined
```

Use `const` by default. Only switch to `let` when you know you'll need to reassign. If you try to reassign a `const`, JavaScript throws an error immediately — which is actually helpful, it means you made a mistake.

⛔ **Don't use `var`** — it's old and has unexpected scoping behavior. Forget it exists.

> 📌 _Live: declare a const. Try reassigning it. Show the error in the console._

---

## SLIDE 26 — Strings & Template Literals

**Layout:** Title at top. Code block centered. Small method list below in two columns. Math object callout at bottom as a reference box with link.

**Title:** Working with text

```js
let name = "Alice";

// Old way — verbose
let greeting = "Hello " + name + "!";

// Modern way — template literals with backticks
let greeting = `Hello ${name}!`;
let math = `Two plus two is ${2 + 2}`;
```

Essential string methods:

```js
name.length; // 5
name.toUpperCase(); // "ALICE"
name.includes("lic"); // true
name.trim(); // removes leading/trailing whitespace
```

📦 **The Math object** works just like Java's — `Math.round()`, `Math.floor()`, `Math.random()` and so on. **Full list of Math methods at: [study guide link]**

> 📌 _Live: template literal with a name variable. Change the name. See the string update._

---

## SLIDE 27 — Booleans & Comparison

**Layout:** Title at top. Code block centered. Key callout in a highlighted box below: === vs ==. Note at bottom.

**Title:** Always use ===

```js
5 === "5"; // false — strict: checks value AND type
5 == "5"; // true  — loose: converts types to match

5 !== 3; // true — not equal (strict)
5 > 3 / 5 < 3 / 5 >= 5 / 5 <= 4;

true && true; // AND
true || false; // OR
!true; // NOT — flips to false
```

⚠️ Use `===` always. The double equals `==` does type coercion — JS tries to make things equal by converting types, which leads to `0 == false` being `true`. With `===` you get: same value AND same type. No surprises.

> 📌 _Live: `console.log(0 == false)` → true. `console.log(0 === false)` → false. That's the bug `===` prevents._

---

## SLIDE 28 — Conditionals & Loops

**Layout:** Title at top. Two-column layout: left = conditionals (if/else + ternary), right = loops (for, while, for...of). Note at bottom. If too crowded, split with Next → button.

**Title:** Same syntax as Java

```js
if (age >= 18) {
  console.log("Adult");
} else if (age >= 13) {
  console.log("Teenager");
} else {
  console.log("Child");
}

let label = age >= 18 ? "Adult" : "Minor";
```

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}

let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}

// New: for...of — clean loop over arrays
for (let fruit of fruits) {
  console.log(fruit);
}
```

You know all of this from Java. The only new thing is `for...of` — it gives you each value directly, no index needed.

---

## SLIDE 29 — Functions

**Layout:** Title at top. Code block centered showing all three styles (declaration, arrow, shorthand) each labeled. Short explanation below. Note at bottom.

**Title:** Arrow functions are the modern standard

```js
// Declaration — classic
function greet(name) {
  return "Hello " + name;
}

// Arrow function — modern, preferred
const greet = (name) => {
  return "Hello " + name;
};

// Shorthand — single expression, no braces or return needed
const greet = (name) => "Hello " + name;

// Default parameter
const greet = (name = "stranger") => "Hello " + name;
greet(); // "Hello stranger"
greet("Alice"); // "Hello Alice"
```

Use arrow functions. They're shorter and handle `this` correctly when working with the DOM — which matters in the next section.

> 📌 _Live: write a function that takes two numbers and returns the sum. Call it. Log the result._

---

## SLIDE 30 — Arrays _(split across 2 slides)_

---

### SLIDE 30a — Arrays: Basics

**Layout:** Title at top. Code block centered. Short explanation below. Next → button.

**Title:** Arrays — Ordered lists of values

```js
let fruits = ["apple", "banana", "cherry"];

fruits[0]; // "apple" — zero-indexed
fruits.length; // 3

fruits.push("mango"); // add to end
fruits.pop(); // remove from end

fruits.includes("cherry"); // true
fruits.indexOf("banana"); // 1 — position in array

fruits.join(", "); // "apple, banana, cherry" — array to string

let copy = [...fruits]; // spread operator — creates a copy
```

> **Next →**

---

### SLIDE 30b — Arrays: map, filter, forEach

**Layout:** Title at top. Code block centered. Short explanation for each method below. Note at bottom.

**Title:** The three methods you'll use constantly

```js
// forEach — run something for each item
fruits.forEach((fruit) => console.log(fruit));

// map — transform every item, returns a new array (same length)
fruits.map((fruit) => fruit.toUpperCase());
// → ["APPLE", "BANANA", "CHERRY"]

// filter — keep only items that match, returns a new array (shorter)
fruits.filter((fruit) => fruit.length > 5);
// → ["banana", "cherry"]
```

`map` and `filter` don't change the original array. They always return a new one.

> 📌 _Live: `[1,2,3,4,5].filter(n => n % 2 === 0).map(n => n _ 10)` — chain them. Output: [20, 40]\*

---

## SLIDE 31 — Objects

**Layout:** Title at top. Code block centered. Explanation of `this` below in a callout. Note at bottom.

**Title:** Key-value collections

```js
let person = {
  name: "Alice",
  age: 25,
  isStudent: true,
  greet: function () {
    return "Hi, I'm " + this.name;
  },
};

person.name; // "Alice" — dot notation
person["name"]; // "Alice" — bracket notation
person.name = "Bob"; // update existing
person.email = "b@b.com"; // add new property

"name" in person; // true — check if key exists
```

`this` inside a method refers to the object itself. `this.name` means "my own `name` property." Think of it as the object talking about itself.

> 📌 _Live: create a product object: name, price, inStock. Write a `describe()` method that returns a string._

---

## SLIDE 32 — console

**Layout:** Title at top. Short code block. One-sentence explanation per method. Small practical tip at the bottom.

**Title:** Your best debugging tool

```js
console.log("Hello"); // print anything
console.log(myVariable); // inspect a variable's value
console.error("oh no"); // shows in red
console.warn("be careful"); // shows in yellow
```

When something doesn't work, `console.log` everything. Check what value a variable actually holds at that moment. This is how every developer debugs, every day.

> 📌 _Open DevTools → Console. Show log, error, warn. Show clicking an error jumps to the line in the file._

---

---

# PART 4 — THE DOM

---

## SLIDE 33 — What is the DOM?

**Layout:** Title at top. Explanation paragraph left (~55%). DOM tree diagram or DevTools screenshot on the right. The flow arrow at the very bottom: HTML → browser parses → DOM tree → JavaScript changes it → browser re-renders.

**Title:** How JavaScript sees your page

When the browser loads your HTML, it parses it and builds a **tree of objects** in memory. That tree is the DOM — Document Object Model.

Every element becomes an object. The `<body>` is an object. The `<h1>` inside it is an object. They're linked as a tree — parents, children, siblings.

JavaScript has access to this tree through a global object called `document`. When you call `document.querySelector("h1")`, JS walks into the tree and hands you that object. Once you have it, you can read it, change it, delete it, or create new ones.

**User does something → JavaScript runs → DOM changes → browser re-renders**

> 📌 _Open DevTools → Elements tab on any live page. Show the DOM tree. Click an element, hover over it — the browser highlights it._

---

## SLIDE 34 — Selecting Elements

**Layout:** Title at top. Code block centered. Short explanation below. Note at bottom.

**Title:** querySelector — your entry point to everything

```js
// Returns the FIRST match — or null if nothing found
document.querySelector("p"); // by tag
document.querySelector(".card"); // by class
document.querySelector("#title"); // by id
document.querySelector(".card p"); // nested — p inside .card

// Returns ALL matches as a NodeList
document.querySelectorAll(".card");
document.querySelectorAll("li");

// Loop over all matches
document.querySelectorAll("li").forEach((item) => {
  console.log(item.textContent);
});
```

The syntax is the exact same as CSS selectors. If you can write it in CSS, you can use it here.

> 📌 _Live: three divs with class card. querySelector gets the first. querySelectorAll gets all three. Log them and expand in console._

---

## SLIDE 35 — Reading & Changing Content

**Layout:** Title at top. Code block centered. Two-item callout below: textContent safe, innerHTML powerful-but-careful. Note at bottom.

**Title:** Getting and setting what's inside an element

```js
const title = document.querySelector("h1");

// Text only — safe
title.textContent; // read
title.textContent = "New Title"; // write

// HTML inside — powerful
title.innerHTML; // read
title.innerHTML = "<em>New</em> Title"; // write — renders HTML
```

**Rule:** use `textContent` for user-generated content. Use `innerHTML` when you control the content and need to inject HTML tags. Setting `innerHTML` with user input is a security risk.

> 📌 _Live: a heading with a button. On click, change textContent. Then try innerHTML with an em tag inside the string._

---

## SLIDE 36 — Attributes

**Layout:** Title at top. Code block centered. Short list explanation below. Note at bottom.

**Title:** Reading and writing HTML attributes

```js
const link = document.querySelector("a");

link.getAttribute("href");
link.setAttribute("href", "https://example.com");
link.removeAttribute("disabled");
link.hasAttribute("disabled"); // true or false

// Direct shortcuts for common attributes
link.href / link.src / link.id;
link.value; // current value of an input
link.checked; // true/false for checkboxes
link.disabled;
```

> 📌 _Live: a button that starts disabled. After 3 seconds (`setTimeout`), `removeAttribute("disabled")` — button activates._

---

## SLIDE 37 — Changing CSS via JavaScript

**Layout:** Title at top. Two labeled sections: Option 1 (inline style) and Option 2 (classList) each with a code block. Preferred pattern highlighted at the bottom in a box. Note at bottom.

**Title:** Two approaches — inline vs class

```js
// Option 1: Inline style — camelCase property names
box.style.color = "red";
box.style.backgroundColor = "blue";
box.style.display = "none";
box.style.display = ""; // empty string removes it

// Option 2: classList — the preferred approach
box.classList.add("active");
box.classList.remove("active");
box.classList.toggle("active"); // add if absent, remove if present
box.classList.contains("active"); // true or false
```

✅ **The preferred pattern:** all visual rules live in CSS, JS only adds/removes classes.

```css
/* styles.css */
.hidden {
  display: none;
}
```

```js
/* script.js */
box.classList.toggle("hidden");
```

> 📌 _Live: button toggles a box visible/hidden using classList.toggle. Show how the CSS rule does the visual work._

---

## SLIDE 38 — Creating & Removing Elements

**Layout:** Title at top. Code block centered labeled with three clear steps (1. Create 2. Configure 3. Insert). Remove at the bottom. Warning callout about forgetting step 3. Note at bottom.

**Title:** Building the DOM from JavaScript

Three steps, every time:

```js
// 1. Create — in memory, NOT on the page yet
const card = document.createElement("div");

// 2. Configure
card.textContent = "New Card";
card.classList.add("card");

// 3. Insert into the page — NOW the user sees it
document.body.appendChild(card);
document.querySelector(".list").appendChild(card);
document.querySelector(".list").prepend(card); // at the start

// Remove
card.remove();
```

⚠️ If you forget step 3, the element exists in memory but the user never sees it.

> 📌 _Live: input + button. On click, create a li, set textContent to input.value, append to ul. Clear the input._

---

## SLIDE 39 — Events

**Layout:** Title at top. Code block centered. Event list below in two columns (mouse events left, keyboard/input right). Note at bottom. If crowded, split with Next →.

**Title:** Reacting to what the user does

```js
const button = document.querySelector("button");

button.addEventListener("click", () => {
  console.log("clicked");
});

// The event object — passed automatically
button.addEventListener("click", (event) => {
  console.log(event.target); // the element that was clicked
});
```

Common events:

| Mouse        | Keyboard / Input |
| ------------ | ---------------- |
| `click`      | `keydown`        |
| `dblclick`   | `keyup`          |
| `mouseenter` | `input`          |
| `mouseleave` | `change`         |
|              | `submit`         |

> 📌 _Live: addEventListener on keydown for the entire document. Log event.key. Type anything — watch the console._

---

## SLIDE 40 — Input Values

**Layout:** Title at top. Code block centered. Short explanation below. Note at bottom.

**Title:** Reading what the user typed

```js
const input = document.querySelector("input");

input.value; // what the user typed — always a string
input.value = ""; // clear the input
input.disabled = true;

const checkbox = document.querySelector("input[type='checkbox']");
checkbox.checked; // true or false
checkbox.checked = true; // check it programmatically
```

`input.value` is a live property. Every time the user types a character, `.value` updates. You don't need an event to read it — just read it when you need it (usually inside a button click handler).

> 📌 _Live: input + button. Button logs input.value. Show it has the current text even without an input event._

---

## SLIDE 41 — Final Project: To-Do List

**Layout:** Title at top. HTML and JS code blocks side by side. Below them: a list of "what this uses" as badges or checkmarks. Note at bottom: "Build live, step by step."

**Title:** Let's build something

```html
<input type="text" id="taskInput" placeholder="Add a task..." />
<button id="addBtn">Add</button>
<ul id="taskList"></ul>
```

```js
const input = document.querySelector("#taskInput");
const button = document.querySelector("#addBtn");
const list = document.querySelector("#taskList");

button.addEventListener("click", () => {
  if (input.value.trim() === "") return;

  const li = document.createElement("li");
  li.textContent = input.value;

  li.addEventListener("click", () => li.remove());

  list.appendChild(li);
  input.value = "";
});
```

✅ HTML structure &nbsp; ✅ CSS classes &nbsp; ✅ querySelector &nbsp; ✅ createElement &nbsp; ✅ appendChild &nbsp; ✅ addEventListener &nbsp; ✅ input.value &nbsp; ✅ classList

> 📌 _Build this live, piece by piece. Start with just the HTML. Add JS one step at a time. Style it at the end._

---

## SLIDE 42 — What's Next

**Layout:** Title at top. Four items in a 2x2 grid. Study guide link in a distinct highlighted box at the bottom center.

**Title:** You now know how the web works.

🧱 **CSS Frameworks** — Tailwind, Bootstrap: pre-written CSS you can use without writing it yourself

⚡ **JavaScript Async** — Fetching data from APIs, loading content without page refresh

⚛️ **Frameworks** — React, Vue: smarter ways to build bigger UIs with components

🖥️ **Backend** — Node.js, databases: the server side of the web

---

**Everything we covered today, plus all the topics we pointed to during the workshop, is written out with explanations and live examples at:**

## 🔗 [study guide link]

---

That's all 42 slides (41 + the box model split). Every slide has layout instructions, the four specific updates you requested are in place, and reference slides each have their own intro, example placeholder, and handoff line.
