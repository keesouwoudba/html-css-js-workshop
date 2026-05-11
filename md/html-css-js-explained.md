This will be long. Give me a moment to write it all out properly.

---

# Workshop Script: HTML, CSS & JavaScript

---

# BEFORE WE START — The Big Picture

Before we write a single line of code, let's understand what we're actually working with. Because these three technologies — HTML, CSS, and JavaScript — are not the same thing. They do completely different jobs, and they were invented at different times for different reasons.

**HTML** is the skeleton. It's just text with special tags around it that tell the browser: this is a heading, this is a paragraph, this is a button. If you strip everything else away, HTML is just the raw content and structure of a page. No colors, no layout, no behavior. Just content.

**CSS** is the stylist. It looks at that skeleton and says: make this heading blue, make that button rounded, put these two boxes side by side. CSS has no logic. It doesn't know what a "click" is. It just describes appearance.

**JavaScript** is the brain. It's an actual programming language — the only one that runs natively inside the browser. It can read the page, change it, react to what the user does, talk to servers. Everything dynamic on the web is JavaScript.

So when you open Google.com: the text, the input box, the buttons — that's HTML. The colors, spacing, fonts — CSS. When you start typing and suggestions appear — JavaScript.

They work together, but they are completely separate. Keep that mental model. It'll save you a lot of confusion.

---
---

# PART 1 — HTML

---

## The HTML File

Every webpage you've ever visited is, at its core, an HTML file. A text file with a `.html` extension. The browser opens it, reads it top to bottom, and paints what it finds onto the screen.

Every HTML file starts the same way:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello, world!</h1>
    <p>This is my first webpage.</p>
  </body>
</html>
```

**`<!DOCTYPE html>`** — This first line is not a tag. It's a declaration. You're telling the browser: "hey, this is a modern HTML5 document." Without it, browsers fall back into a weird legacy mode. Always include it.

**`<html>`** — Everything lives inside this. It's the root, the wrapper around the entire page.

**`<head>`** — Think of this as the backstage. Everything in here is invisible to the user. The page title, links to CSS files, font imports. The browser reads it, uses it, but doesn't display it.

**`<body>`** — This is the stage. Everything visible — text, images, buttons — goes here.

**`<title>`** — That text you see in the browser tab. Not on the page, just in the tab.

> **Run this.** Save it as `index.html`, open in a browser. Notice the title in the tab. Notice the heading is bigger than the paragraph — automatically, with zero CSS.

---

## Tags, Elements, Attributes

HTML works with **tags**. A tag is a word in angle brackets: `<p>`. Most tags come in pairs — an opening tag and a closing tag with a slash: `</p>`. Everything between them is the content.

```html
<p>This is a paragraph.</p>
```

The combination of opening tag, content, and closing tag is called an **element**.

Some elements don't have content and don't need a closing tag:

```html
<br>    <!-- a line break -->
<hr>    <!-- a horizontal line -->
<img src="photo.jpg" alt="a photo">
```

**Attributes** are extra information you add to a tag. They live inside the opening tag and follow the pattern `name="value"`:

```html
<a href="https://google.com" target="_blank">Go to Google</a>
```

Here `href` tells the browser where the link goes. `target="_blank"` says: open it in a new tab. The text "Go to Google" is what the user sees and clicks.

> **Run this.** Make an anchor tag. Click it. Change `target="_blank"` to see the difference.

---

## Text Tags

Headings in HTML go from `<h1>` to `<h6>`. `h1` is the biggest, most important heading — like the title of a book. `h6` is the smallest. The browser gives them sizes automatically. That's not CSS, that's just the browser's default style.

```html
<h1>Main Title</h1>
<h2>Section Title</h2>
<h3>Subsection</h3>
<p>A regular paragraph of text.</p>
<strong>This text is bold.</strong>
<em>This text is italic.</em>
<u>This text is underlined.</u>
<s>This text has a strikethrough.</s>
<br>
<hr>
```

`<strong>` means "this is important." The browser renders it bold. `<em>` means "emphasis" — italic. `<u>` is underline. `<s>` is strikethrough, like a deleted price. These aren't just visual — they carry semantic meaning. A screen reader for blind users will actually read `<strong>` text with more emphasis.

> **Run this.** See how each tag affects the text differently.

---

## Links

The anchor tag `<a>` is how the web works. The web is literally a web of documents connected by links. Every link you've ever clicked is an `<a>` tag.

```html
<a href="https://google.com">Go to Google</a>
<a href="https://google.com" target="_blank">Open in new tab</a>
<a href="about.html">Go to my About page</a>
```

`href` stands for "hypertext reference." It's the destination. It can be an absolute URL like `https://google.com`, or a relative path like `about.html` — which means "look for a file called about.html next to this file."

> **Run this.** Create two HTML files in the same folder. Link between them with a relative path.

---

## Images

```html
<img src="photo.jpg" alt="A sunset photo">
<img src="images/photo.jpg" alt="A sunset photo">
```

`<img>` has no closing tag. `src` is the path to the image file — either relative (next to your HTML file) or absolute (a full URL). `alt` is the text shown if the image doesn't load. It's also what screen readers read for blind users. Always include it.

> **Run this.** Drop any image file next to your HTML file, reference it by name. Notice what happens if you mistype the filename.

---

## Lists

Two kinds: unordered (bullet points) and ordered (numbered). Both use `<li>` for list items inside them.

```html
<ul>
  <li>Apples</li>
  <li>Bananas</li>
  <li>Cherries</li>
</ul>

<ol>
  <li>Boil water</li>
  <li>Add pasta</li>
  <li>Wait 10 minutes</li>
</ol>
```

`<ul>` is "unordered list" — bullets. `<ol>` is "ordered list" — numbers. The browser handles the bullets and numbers automatically. You don't type them.

> **Run this.** Notice the browser auto-numbers your `<ol>` items.

---

## Forms & Inputs

Forms are how users give you information. A search bar, a login form, a checkout page — all forms.

```html
<input type="text" placeholder="Enter your name">
<input type="email" placeholder="Enter email">
<input type="password" placeholder="Password">
<input type="number" placeholder="Your age">
<input type="checkbox"> Remember me
<input type="radio" name="color"> Red
<input type="radio" name="color"> Blue
<input type="date">
<input type="file">

<textarea placeholder="Write a message..."></textarea>

<select>
  <option value="js">JavaScript</option>
  <option value="py">Python</option>
</select>

<button>Click me</button>
<button type="submit">Submit</button>
```

`type` tells the browser what kind of input. `type="password"` automatically hides the characters. `type="email"` validates email format on mobile. `placeholder` is that greyed-out hint text. For radio buttons, give them the same `name` — that's how the browser knows they're in the same group and only one can be selected.

`<textarea>` is a multi-line text box. `<select>` is a dropdown. Both are their own elements, not `<input>`.

> **Run this.** Notice how `type="password"` hides characters. Notice the date picker. Notice only one radio can be selected.

---

## div and span

`<div>` and `<span>` are containers with no visual meaning on their own. They're blank boxes you use to group things and apply CSS to.

```html
<div class="card">
  <h2>Product Name</h2>
  <p>Product description here.</p>
  <button>Buy Now</button>
</div>

<p>The price is <span class="price">$9.99</span> today only.</p>
```

The key difference: `<div>` is **block-level** — it takes up the full width and starts on a new line. `<span>` is **inline** — it sits inside text without breaking the line. Think of `<div>` as a box, `<span>` as a highlighter pen on a word.

> **Run this.** Notice the div creates a visual block. The span changes just the word inside the paragraph.

---

## Semantic Tags

These are `<div>` alternatives that carry meaning. They work exactly the same way as a div — they're just containers. But their name tells the browser, search engines, and screen readers what role that section plays.

```html
<header>
  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
  </nav>
</header>

<main>
  <section>
    <h1>Welcome</h1>
    <p>This is the homepage.</p>
  </section>
  <article>
    <h2>Blog Post Title</h2>
    <p>Post content here.</p>
  </article>
</main>

<aside>
  <p>Related links</p>
</aside>

<footer>
  <p>© 2024 My Website</p>
</footer>
```

`<header>` — top of the page or a section. `<nav>` — navigation links. `<main>` — the main content. `<section>` — a grouped section of content. `<article>` — standalone content like a blog post or a card. `<aside>` — sidebar, supplementary content. `<footer>` — bottom of the page.

Google's crawler reads these to understand your page structure. A screen reader uses them to help a blind user navigate. Functionally identical to div — semantically far superior.

> **Run this.** The page looks the same as with divs. That's the point — the benefit is invisible to the eye, not the machine.

---

## HTML Attributes

A quick reference of the most common attributes:

```html
id="uniqueName"     <!-- one element on the whole page — used in CSS (#id) and JS -->
class="cardStyle"   <!-- shared across many elements — used in CSS (.class) -->
href="..."          <!-- destination for links -->
src="..."           <!-- file path for images and scripts -->
alt="..."           <!-- fallback text for images -->
placeholder="..."   <!-- hint text in inputs -->
type="..."          <!-- input type: text, email, checkbox, etc. -->
disabled            <!-- disables the element (no value needed) -->
required            <!-- makes form field mandatory (no value needed) -->
```

> **Run this.** Add `disabled` to a button. Notice it becomes greyed out and unclickable.

---
---

# PART 2 — CSS

---

## What CSS Is

HTML gives you content. CSS gives you control over how it looks. CSS is a completely separate language — different syntax, different file, different job.

The fundamental concept of CSS is simple: you pick an element (or elements), and you describe how they should look.

```css
p {
  color: blue;
  font-size: 20px;
}
```

"All paragraphs should have blue text and a font size of 20 pixels." That's it. That's CSS.

---

## How to Connect CSS to HTML

Three ways. You should know all three, but use Option 1 in real projects.

```html
<!-- Option 1: External file — keep CSS separate (recommended) -->
<link rel="stylesheet" href="styles.css">

<!-- Option 2: Style tag inside <head> — fine for small experiments -->
<style>
  p { color: blue; }
</style>

<!-- Option 3: Inline — directly on the element. Avoid this. -->
<p style="color: blue;">Text</p>
```

Option 3 gets messy fast. If you have 50 paragraphs and want to change the color, you'd have to edit all 50. With Option 1, you change one file.

---

## Selectors

A selector is how CSS decides which elements to style.

```css
/* By tag name — targets ALL paragraphs */
p {
  color: blue;
}

/* By class — targets everything with class="card" */
.card {
  background-color: white;
}

/* By id — targets the ONE element with id="title" */
#title {
  font-size: 32px;
}

/* Everything on the page */
* {
  box-sizing: border-box;
}

/* Multiple selectors at once */
h1, h2, h3 {
  font-weight: bold;
}

/* Nested — only <p> tags INSIDE .card */
.card p {
  color: gray;
}
```

The difference between class and id: a class can be used on many elements, an id must be unique — one per page. Think of class as a category ("all employees"), id as a unique name badge ("only John Smith").

Hover and active are called **pseudo-classes** — they only apply under specific conditions:

```css
button:hover {
  background-color: darkblue; /* only when mouse is over the button */
}

button:active {
  background-color: black; /* only while the button is being clicked */
}
```

> **Run this.** Write `.card { background-color: lightyellow; }`. Apply it to two divs and watch both change.

---

## Colors

CSS has four ways to express color. They're all valid. Pick whichever you prefer.

```css
/* 1. By name — simple, but limited to ~140 named colors */
color: red;
color: white;
color: black;
color: transparent;

/* 2. RGB — Red, Green, Blue. Each value from 0 to 255 */
color: rgb(255, 0, 0);       /* pure red */
color: rgb(0, 0, 255);       /* pure blue */
color: rgb(0, 0, 0);         /* black */
color: rgb(255, 255, 255);   /* white */

/* 3. RGBA — same as RGB but with an Alpha (transparency) value from 0 to 1 */
color: rgba(255, 0, 0, 0.5); /* red, 50% transparent */
color: rgba(0, 0, 0, 0.2);   /* very faint black overlay */

/* 4. Hex — same as RGB, just written in base-16 shorthand */
color: #FF0000;  /* red */
color: #000000;  /* black */
color: #FFFFFF;  /* white */
color: #0096FF;  /* a nice blue */
```

RGBA is especially useful for overlays, shadows, and subtle backgrounds. When you want a faint shadow that blends with any background color, `rgba(0,0,0,0.2)` — a 20% opaque black — works on everything.

> **Run this.** Create 4 divs with the same red expressed four different ways. They should all look identical.

---

## Backgrounds

```css
/* Solid color */
background-color: red;
background-color: rgb(0, 150, 255);
background-color: transparent;

/* Image */
background-image: url("photo.jpg");
background-size: cover;      /* fill the container, crop if needed */
background-size: contain;    /* fit the image inside, may leave gaps */
background-size: 100% 100%;  /* stretch to fill, may distort */
background-position: center; /* center the image in the container */
```

`background-size: cover` is the one you'll use 90% of the time for hero images and card backgrounds. It fills the space and crops intelligently. Think of it like fitting a photo into a frame — the photo fills the frame, and the edges get cut if needed.

> **Run this.** Give a `<div>` a fixed width and height, set `background-image` and `background-size: cover`. Try changing to `contain`. See the difference.

---

## Text & Fonts

```css
/* Font family — browser tries each one in order, uses first available */
font-family: Arial;
font-family: Roboto, Arial, sans-serif;

/* Size */
font-size: 16px;

/* Weight */
font-weight: normal;  /* regular text */
font-weight: bold;    /* bold text */

/* Style */
font-style: italic;

/* Color */
color: black;

/* Alignment */
text-align: left;
text-align: center;
text-align: right;
text-align: justify;

/* Decoration */
text-decoration: none;          /* removes underline — useful on links */
text-decoration: underline;
text-decoration: line-through;  /* strikethrough */

/* Transform */
text-transform: uppercase;
text-transform: lowercase;
text-transform: capitalize;     /* capitalizes first letter of each word */

/* Spacing */
line-height: 1.5;    /* 1.5x the font-size — good for readability */
letter-spacing: 2px; /* space between each character */
```

`font-family` with multiple values is called a font stack. The browser tries "Roboto" first. If that's not installed, it falls back to "Arial". If that's not available, it uses any generic `sans-serif` font. This is a safety net.

`text-decoration: none` is something you'll write constantly — by default, `<a>` tags have an underline. Most designs don't want it. You remove it with this.

> **Run this.** Try `text-transform: uppercase` on a heading — notice you didn't change the HTML, just how it displays.

---

## Sizing

```css
/* Width */
width: 200px;    /* fixed — always 200px regardless of screen */
width: 50%;      /* relative — 50% of the parent container's width */
width: 100vw;    /* 100% of the viewport (screen) width */
min-width: 100px; /* never smaller than this */
max-width: 600px; /* never larger than this */

/* Height */
height: 100px;
height: 100vh;    /* 100% of the viewport height */
min-height: 200px;
max-height: 500px;
```

`px` is pixels — exact, fixed. `%` is relative to the parent. `vw` and `vh` are relative to the browser window itself. A div with `width: 100vw; height: 100vh` takes up the entire screen — useful for full-screen hero sections.

`max-width` is something you'll use constantly. Set `max-width: 1200px` on a container and it'll never stretch wider than 1200px on huge monitors, but it'll shrink fine on smaller screens.

> **Run this.** Set `width: 100%` on a div inside another div. Then set `max-width: 400px`. Resize the browser window.

---

## Box Model

This is one of the most important concepts in CSS. Every single element on a page — every button, div, paragraph — is a rectangle. And that rectangle has four layers:

1. **Content** — the actual text or image
2. **Padding** — breathing room inside the element, between content and border
3. **Border** — the outline
4. **Margin** — space outside the element, pushing other elements away

```css
/* Padding: space INSIDE — order is top, right, bottom, left */
padding: 10px 20px 30px 40px;
padding-top: 10px;
padding-right: 20px;
padding-bottom: 30px;
padding-left: 40px;

/* Margin: space OUTSIDE */
margin: 10px 20px 30px 40px;
margin-top: 10px;
margin-right: 20px;
margin-bottom: 30px;
margin-left: 40px;
margin: auto;  /* centers the element horizontally */

/* Border — shorthand: width, style, color */
border: 1px solid black;
border: 2px dashed red;
border: none;

/* Rounded corners */
border-radius: 5px;   /* slightly rounded */
border-radius: 50%;   /* perfect circle — only if width equals height */

/* CRITICAL: box-sizing */
box-sizing: border-box; /* padding is INCLUDED in the stated width */
```

Here's the trap beginners fall into. You set `width: 200px` on a div. Then you add `padding: 20px`. Suddenly the element is 240px wide. That's the default behavior — padding is added *on top of* the width. `box-sizing: border-box` fixes this: the padding is counted *within* the 200px. Put this on every element at the top of every CSS file:

```css
* {
  box-sizing: border-box;
}
```

> **Run this.** Create two identical divs, same width and padding. Add `box-sizing: border-box` to only one. See the size difference.

---

## Display

Every HTML element has a default display value. Changing it is one of the most powerful things you can do in CSS.

```css
display: block;         /* takes up full width, starts on a new line (div, p, h1) */
display: inline;        /* sits inside text, no width/height control (span, a) */
display: inline-block;  /* inline BUT you can set width and height */
display: none;          /* element is completely gone — not just invisible */
display: flex;          /* flexbox — covered next */
```

The difference between `display: none` and `opacity: 0` is important:
- `display: none` — element is removed from the page entirely, other elements fill its space
- `opacity: 0` — element is invisible but still takes up space, like a ghost

> **Run this.** Add `display: none` to a div in the middle of three divs. Watch the surrounding elements close the gap.

---

## Opacity

```css
opacity: 1;    /* fully visible — default */
opacity: 0.5;  /* 50% transparent */
opacity: 0;    /* invisible but still takes up space */
```

`opacity` affects the entire element including its children. If you want only the background to be transparent, use `rgba()` on the background color instead of opacity.

> **Run this.** Set a button to `opacity: 0.3`. Notice it's faded but still clickable and still takes up space.

---

## Flexbox

Before flexbox, centering something vertically in CSS was a notoriously annoying problem. Flexbox solved it. Flexbox is a layout system — you apply it to a container and it controls how its children are arranged.

The mental model: you have a container, and inside it you have items. Flexbox lets you control how those items are distributed along two axes — the main axis (by default, horizontal) and the cross axis (vertical).

Apply to the **container**:

```css
display: flex;

/* Direction — which way items flow */
flex-direction: row;           /* left to right — default */
flex-direction: row-reverse;   /* right to left */
flex-direction: column;        /* top to bottom */
flex-direction: column-reverse;/* bottom to top */

/* Justify-content — alignment along the MAIN axis */
justify-content: flex-start;   /* pack items to the start — default */
justify-content: flex-end;     /* pack items to the end */
justify-content: center;       /* center all items */
justify-content: space-between;/* equal gaps between items, none on edges */
justify-content: space-around; /* equal space around each item */
justify-content: space-evenly; /* perfectly equal space everywhere */

/* Align-items — alignment along the CROSS axis */
align-items: stretch;      /* items stretch to fill height — default */
align-items: flex-start;   /* items align to top */
align-items: flex-end;     /* items align to bottom */
align-items: center;       /* items vertically centered */

/* Gap between items */
gap: 10px;
gap: 10px 20px; /* row-gap | column-gap */
```

Apply to the **children** (flex items):

```css
flex: 1;        /* take up equal share of remaining space */
flex: 2;        /* take up twice the space of an item with flex: 1 */
flex-shrink: 0; /* don't shrink even if container is too small */
```

> **Run this.** Three divs inside a container. Add `display: flex`. Try every `justify-content` value. Then try `align-items: center` with a fixed `height` on the container. That's how you vertically center things.

---

## Position

By default, elements just stack vertically, top to bottom. Position lets you break out of that.

```css
position: static;    /* default — element is in normal flow, ignores top/left/etc */

position: relative;  /* element stays in normal flow, BUT you can nudge it */
top: 10px;           /* pushes it 10px down from where it would naturally be */
left: 20px;          /* pushes it 20px right */
/* NOTE: the space it originally occupied is still reserved */

position: absolute;  /* removed from normal flow entirely */
                     /* positioned relative to the nearest parent that has
                        a non-static position (usually position: relative) */
top: 0;
right: 0;
/* Use this for: tooltips, badges, overlay buttons, dropdowns */

position: fixed;     /* like absolute but anchored to the browser WINDOW */
                     /* it doesn't scroll — it stays put */
top: 0;
left: 0;
/* Use this for: sticky navigation bars, floating chat buttons */

position: sticky;    /* hybrid — acts like relative while scrolling normally,
                        then "sticks" once it hits the threshold you set */
top: 0;
/* Use this for: table headers, section headings that stick while in view */
```

The most important pattern: if you want to position something **inside** a parent element (a badge on a card, a close button in a modal), set `position: relative` on the parent and `position: absolute` on the child.

```html
<div style="position: relative; width: 200px; height: 200px; background: lightblue;">
  <span style="position: absolute; top: 5px; right: 5px; background: red; color: white; padding: 2px 6px;">
    NEW
  </span>
  Card content
</div>
```

> **Run this.** The badge sticks to the top-right corner of the card regardless of content. Try removing `position: relative` from the parent — the badge escapes to the page corner.

---

## Shadow & Cursor

```css
/* Box shadow: horizontal-offset vertical-offset blur color */
box-shadow: 2px 4px 8px rgba(0, 0, 0, 0.2);
/* 2px right, 4px down, 8px blur, 20% transparent black */

cursor: pointer; /* shows the hand icon — always add this to custom clickable elements */
```

The hand cursor is important for UX. When users hover over something clickable, they expect to see a hand. Buttons have it by default. Divs and spans you make clickable with JavaScript don't — you have to add it manually.

> **Run this.** Create a card with `box-shadow`. Then try removing the blur (`0` instead of `8px`) for a hard shadow effect.

---
---

# PART 3 — JAVASCRIPT

---

## What JavaScript Is

You know Java. JavaScript is not Java. The name was a marketing decision from 1995. They share curly braces and some syntax, but they're different languages with different purposes.

JavaScript is the only programming language that runs natively in browsers. Every browser — Chrome, Firefox, Safari — has a JavaScript engine built in. V8 in Chrome. SpiderMonkey in Firefox. These engines compile your JavaScript to machine code and execute it.

JavaScript was originally just for small page interactions. Today it runs servers (Node.js), mobile apps, desktop apps, and machine learning models. But in this workshop, we care about one thing: making web pages interactive.

---

## Variables

```js
let name = "Alice";   // can be reassigned later
const PI = 3.14;      // cannot be reassigned — throws an error if you try

// Data types
let num = 42;
let text = "hello";
let flag = true;        // boolean
let nothing = null;     // explicitly nothing
let notDefined;         // undefined — declared but no value yet
```

`let` vs `const` — use `const` by default. Only switch to `let` when you know you'll need to reassign. This is a habit that prevents bugs. If you try to reassign a `const`, JavaScript will throw an error immediately, which is exactly what you want — it means you made a mistake.

Don't use `var`. It's the old way and has weird scoping rules. Forget it exists.

> **Run this.** Open the browser console (F12). Type `const x = 5; x = 10;` — watch it throw an error.

---

## Strings

```js
let name = "Alice";

// Template literal — the modern, clean way to build strings
let greeting = `Hello ${name}, welcome!`;
let math = `Two plus two is ${2 + 2}`;

// Methods
name.length           // 5 — number of characters
name.toUpperCase()    // "ALICE"
name.includes("lic")  // true — does the string contain "lic"?
name.trim()           // removes whitespace from start and end
```

Template literals use backticks (`` ` ``), not quotes. The `${}` syntax lets you embed any JavaScript expression — a variable, a calculation, a function call. This replaces `"Hello " + name + "!"` which is verbose and error-prone.

> **Run this.** `let price = 9.99; console.log(`Price is $${price}`);`

---

## Numbers

```js
let x = 10;
let y = 3;

x + y     // 13
x - y     // 7
x * y     // 30
x / y     // 3.333...
x % y     // 1  — remainder (modulo) — "10 divided by 3 leaves 1 over"
x ** y    // 1000 — power: 10 to the 3rd

// Math object — built-in math utilities
Math.round(4.6)    // 5 — rounds to nearest integer
Math.floor(4.9)    // 4 — always rounds DOWN
Math.ceil(4.1)     // 5 — always rounds UP
Math.abs(-5)       // 5 — absolute value
Math.max(1, 5, 3)  // 5 — largest value
Math.min(1, 5, 3)  // 1 — smallest value
Math.random()      // random decimal between 0 and 1
```

`Math.random()` is very commonly used. To get a random integer from 0 to 9: `Math.floor(Math.random() * 10)`.

> **Run this.** `console.log(Math.floor(Math.random() * 100))` — run it several times. Different number each time.

---

## Booleans & Comparison

```js
// Always use === (strict equality — checks value AND type)
5 === 5      // true
5 === "5"    // false — number vs string
5 !== 3      // true — not equal

5 > 3        // true
5 < 3        // false
5 >= 5       // true
5 <= 4       // false

// Logical operators — same as Java
true && true     // AND — both must be true
true || false    // OR — at least one must be true
!true            // NOT — flips it: false
```

Use `===` not `==`. The double equals `==` does type coercion — JavaScript tries to convert types to make things equal, which leads to bizarre bugs like `0 == false` being `true`. `===` is strict: same value AND same type. Always.

> **Run this.** `console.log(0 == false)` then `console.log(0 === false)`. One is true, one is false. This is why we use `===`.

---

## Conditionals

```js
let age = 20;

if (age >= 18) {
  console.log("Adult");
} else if (age >= 13) {
  console.log("Teenager");
} else {
  console.log("Child");
}

// Ternary — shorthand for a simple if/else in one line
let label = age >= 18 ? "Adult" : "Minor";
// reads as: "if age >= 18, label is Adult, otherwise label is Minor"
```

The ternary operator is useful when you want to assign a value based on a condition. It's not for complex logic — keep it simple, one condition.

> **Run this.** Change the `age` value. Watch the output change.

---

## Loops

You know these from Java. The syntax is identical.

```js
// Classic for loop
for (let i = 0; i < 5; i++) {
  console.log(i);  // 0, 1, 2, 3, 4
}

// While loop
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}

// For...of — cleaner way to loop over an array
let fruits = ["apple", "banana", "cherry"];
for (let fruit of fruits) {
  console.log(fruit);
}
```

`for...of` is the one you'll use most in practice. It gives you each *value* in the array directly. No index to manage, no length to check.

> **Run this.** Loop from 1 to 10 and log whether each number is odd or even using `% 2`.

---

## Functions

```js
// Function declaration — hoisted, can be called before it's defined
function greet(name) {
  return "Hello " + name;
}

// Arrow function — modern syntax, preferred in almost all cases
const greet = (name) => {
  return "Hello " + name;
};

// Arrow shorthand — if the body is a single expression, drop the braces and return
const greet = (name) => "Hello " + name;

// Default parameter — if no argument is passed, use this default
const greet = (name = "stranger") => "Hello " + name;

// Multiple parameters
const add = (a, b) => a + b;

// No parameters
const sayHi = () => console.log("Hi!");

// Calling functions
console.log(greet("Alice"));  // "Hello Alice"
console.log(greet());         // "Hello stranger"
```

Arrow functions are not just shorter syntax. They also handle `this` differently from regular functions — which matters when working with the DOM. For now, just know: arrow functions are the default choice in modern JavaScript.

> **Run this.** Write a function `multiply(a, b)` that returns `a * b`. Call it with several values.

---

## Arrays

An array is an ordered list of values. In JavaScript, one array can hold mixed types — numbers, strings, objects, other arrays. You'll mostly use them with one type at a time.

```js
let fruits = ["apple", "banana", "cherry"];

// Access by index — zero-based
fruits[0]          // "apple"
fruits[2]          // "cherry"
fruits.length      // 3

// Add and remove
fruits.push("mango")    // add to the END — returns new length
fruits.pop()            // remove from the END — returns removed item

// Check
fruits.indexOf("banana")  // 1 — returns index, or -1 if not found
fruits.includes("cherry") // true

// Convert
fruits.join(", ")  // "apple, banana, cherry" — array to string

// Iterate
fruits.forEach((fruit) => console.log(fruit))       // runs a function on each item

// Transform — returns a NEW array
fruits.map((fruit) => fruit.toUpperCase())           // ["APPLE", "BANANA", "CHERRY"]
fruits.filter((fruit) => fruit.length > 5)           // ["banana", "cherry"]

// Copy
let copy = [...fruits];  // spread operator — creates a shallow copy
```

`map` and `filter` are the most important array methods. `map` transforms every item — same length, different values. `filter` removes items that don't match — shorter array, same type of values.

> **Run this.** `[1, 2, 3, 4, 5].filter(n => n % 2 === 0)` — gives you only even numbers. Then `.map(n => n * 10)` on the result.

---

## Objects

An object is a collection of key-value pairs. If an array is a list, an object is a record. Think of it like a row in a database: one entity with multiple properties.

```js
let person = {
  name: "Alice",
  age: 25,
  isStudent: true,
  greet: function() {
    return "Hi, I'm " + this.name;
  }
};

// Read properties
person.name       // "Alice" — dot notation
person["name"]    // "Alice" — bracket notation (useful for dynamic keys)

// Set or add properties
person.name = "Bob";
person.email = "bob@example.com";  // creates a new property if it doesn't exist

// Check if a key exists
"name" in person  // true
```

`this` inside a method refers to the object itself. `this.name` inside `greet()` means "the name property of this same object." This is how objects have their own context.

> **Run this.** Create an object for a car: make, model, year. Add a method `describe()` that returns a string describing the car.

---

## console

```js
console.log("Hello")        // print anything to the browser console
console.log(myVariable)     // inspect a variable
console.error("oh no")      // shows in red — use for errors
console.warn("be careful")  // shows in yellow — use for warnings
```

The browser console (F12 → Console) is your best friend when debugging. When something doesn't work, `console.log` everything. Check what value a variable actually has at that moment.

---
---

# PART 4 — THE DOM

---

## What the DOM Is

When the browser loads your HTML file, it doesn't just display it. It parses it — reads it character by character — and builds a tree of objects in memory. That tree is the DOM: the Document Object Model.

Every element in your HTML becomes an object in that tree. The `<body>` is an object. The `<h1>` inside it is an object. The text inside the `<h1>` is an object. They're all linked — parents, children, siblings.

JavaScript has access to this tree through a global object called `document`. `document` is the entry point to your entire page. When you say `document.querySelector("h1")`, you're asking JavaScript to walk into that tree and find the first `<h1>` object and give it to you.

Once you have that object, you can read it, change it, delete it, or create new ones. That's how interactivity works. A click happens → JavaScript runs → JavaScript changes the DOM → the browser re-renders the changed part.

---

## Selecting Elements

```js
// querySelector — returns the FIRST matching element (or null if none found)
document.querySelector("p")          // first <p> on the page
document.querySelector(".card")      // first element with class="card"
document.querySelector("#title")     // the element with id="title"
document.querySelector(".card p")    // first <p> inside a .card

// querySelectorAll — returns ALL matching elements as a NodeList
document.querySelectorAll("p")       // every <p>
document.querySelectorAll(".card")   // every .card

// Iterating over querySelectorAll results
document.querySelectorAll("li").forEach((item) => {
  console.log(item.textContent);
});
```

`querySelector` uses the exact same syntax as CSS selectors. If you know CSS selectors, you already know how to select DOM elements.

`querySelectorAll` returns a NodeList — it looks like an array and you can loop over it with `forEach`, but it's not quite a full array. Calling `.forEach()` on it works. `.map()` does not without converting first.

> **Run this.** `console.log(document.querySelector("h1"))` — see the element object in the console. Expand it.

---

## Reading & Changing Content

```js
const title = document.querySelector("h1");

// textContent — the raw text, no HTML
title.textContent            // "Hello World"
title.textContent = "New Title";  // changes what the user sees

// innerHTML — the HTML inside the element
title.innerHTML              // "<strong>Hello</strong> World"
title.innerHTML = "<strong>Bold Title</strong>";  // renders HTML
```

`textContent` is safe — it treats everything as plain text. If you set `textContent = "<strong>bold</strong>"` the user will literally see the `<strong>` tags as text.

`innerHTML` is powerful but potentially dangerous. If you insert user-supplied content with `innerHTML`, malicious users can inject scripts. For user-generated content, always use `textContent`.

> **Run this.** Select a heading. Change its `textContent`. Then try `innerHTML` with a `<em>` tag inside the string.

---

## Attributes

```js
const link = document.querySelector("a");

link.getAttribute("href")               // get any attribute
link.setAttribute("href", "https://example.com")  // set any attribute
link.removeAttribute("disabled")         // delete attribute
link.hasAttribute("disabled")            // true or false

// Shorthand direct access for common attributes
link.href
link.src
link.id
link.value          // current value of an input
link.checked        // true/false for checkboxes
link.disabled       // true/false
link.placeholder
```

> **Run this.** Select an input, `console.log(input.value)` after typing something in it. The value updates live.

---

## Changing CSS via JavaScript

Two ways: inline styles (direct) or class manipulation (cleaner).

```js
const box = document.querySelector(".box");

// Option 1: Inline style — camelCase for CSS properties
box.style.color = "red";
box.style.backgroundColor = "blue";   // background-color → backgroundColor
box.style.fontSize = "20px";
box.style.display = "none";
box.style.display = "";               // empty string removes the inline style

// Option 2: Classes — preferred approach
// Keep all visual rules in CSS, toggle classes with JS
box.classList.add("active");
box.classList.remove("active");
box.classList.toggle("active");        // adds if absent, removes if present
box.classList.contains("active");      // returns true or false
box.className = "box card highlighted"; // replaces ALL classes
```

The class approach is cleaner. You put all visual logic in CSS (`.active { background: green; }`), and JavaScript just adds or removes that class. Separation of concerns — CSS handles looks, JS handles behavior.

> **Run this.** Write a CSS class `.hidden { display: none; }`. In JS, `classList.toggle("hidden")` on a button click. You now have a show/hide toggle.

---

## Creating & Removing Elements

```js
// 1. Create — creates an element in memory, not yet on the page
const newDiv = document.createElement("div");

// 2. Configure it
newDiv.textContent = "I was created by JavaScript";
newDiv.classList.add("card");

// 3. Insert it into the DOM
document.body.appendChild(newDiv);              // at the end of body
document.querySelector(".list").appendChild(newDiv);  // inside .list

document.querySelector(".list").prepend(newDiv);  // at the START
document.querySelector(".list").append(newDiv);   // at the END

// Remove
newDiv.remove();  // removes itself from the DOM
```

The three steps every time: create → configure → insert. If you forget the insert step, the element exists in memory but the user never sees it.

> **Run this.** Create a `<p>` element, give it text, append it to the body. Then add a button that calls `.remove()` on it.

---

## Events

An event is something that happens — a click, a key press, a form submission. JavaScript can listen for these and run code when they occur.

```js
const button = document.querySelector("button");

// addEventListener: element, event name, callback function
button.addEventListener("click", () => {
  console.log("Button was clicked");
});

// The event object — passed automatically to your callback
button.addEventListener("click", (event) => {
  console.log(event.target);     // the element that triggered the event
  event.preventDefault();        // stops default browser behavior (e.g. form submit, link follow)
  event.stopPropagation();       // stops event from bubbling up to parent elements
});
```

Common event types:

```js
"click"        // mouse click
"dblclick"     // double click
"mouseenter"   // mouse enters element area
"mouseleave"   // mouse leaves element area

"keydown"      // key pressed down — fires repeatedly if held
"keyup"        // key released

"input"        // input value changes — fires on every keystroke
"change"       // input value committed (on blur, or selection change)

"submit"       // form submitted
"load"         // page fully loaded
"scroll"       // user scrolls
"resize"       // browser window resized
```

> **Run this.** Add a `keydown` listener to `document`. Log `event.key`. Type on the keyboard — see what gets logged.

---

## Working with Inputs

```js
const input = document.querySelector("input");

input.value             // get what the user typed
input.value = "Hello";  // programmatically set the value
input.disabled = true;  // disable the input

const checkbox = document.querySelector("input[type='checkbox']");
checkbox.checked           // true or false
checkbox.checked = true;   // check it programmatically
```

> **Run this.** Input + button. On click, log `input.value`. See the live value.

---

## Patterns — Putting It All Together

**Toggle show/hide:**
```js
const box = document.querySelector(".box");
const btn = document.querySelector("button");

btn.addEventListener("click", () => {
  box.classList.toggle("hidden");
});
```
```css
.hidden { display: none; }
```

**Build a live list:**
```html
<input type="text" id="taskInput" placeholder="Add a task">
<button id="addBtn">Add</button>
<ul id="taskList"></ul>
```
```js
const input = document.querySelector("#taskInput");
const button = document.querySelector("#addBtn");
const list = document.querySelector("#taskList");

button.addEventListener("click", () => {
  if (input.value.trim() === "") return; // don't add empty items

  const li = document.createElement("li");
  li.textContent = input.value;
  list.appendChild(li);
  input.value = "";
});
```

**Delete on click:**
```js
document.querySelectorAll("li").forEach((li) => {
  li.addEventListener("click", () => {
    li.remove();
  });
});
```

> **This is your final demo.** Build the to-do list live. It uses HTML structure, CSS for style, and every DOM concept covered: selecting, creating, appending, events, input values. Everything lands in one place.

---
