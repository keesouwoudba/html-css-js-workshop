Here are the first ten HTML files from the workshop notes, structured exactly as the generator code would output them .

### 1. html/01-structure.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — HTML Structure</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>HTML Structure</h1><p>The skeleton every webpage starts with</p></div>

<div class="card"><div class="cl">Every HTML File Has Exactly This Shape</div>
<div class="demo" style="font-family:monospace;font-size:14px">
<div style="background:#fff8f8;border:2px solid #e53935;border-radius:8px;padding:12px;margin-bottom:8px">
<span style="background:#e53935;color:#fff;font-size:11px;padding:2px 8px;border-radius:4px;margin-right:8px">&lt;!DOCTYPE html&gt;</span>
<span style="color:#888;font-size:12px">← Tells browser: this is modern HTML5</span>
</div>
<div style="background:#f5eeff;border:2px solid #8e24aa;border-radius:8px;padding:14px">
<span style="color:#8e24aa;font-weight:700">&lt;html&gt;</span> <span style="color:#888;font-size:12px">← Root. Everything lives inside.</span>
<div style="background:#e8f4ff;border:2px solid #1565c0;border-radius:8px;padding:14px;margin:10px 0">
<span style="color:#1565c0;font-weight:700">&lt;head&gt;</span> <span style="color:#888;font-size:12px">← Invisible. Metadata, CSS links.</span>
<div style="background:#fff;border:1px solid #90caf9;border-radius:6px;padding:10px;margin:8px 0;font-size:13px">
<title><strong>My Page</strong></title> <span style="color:#888">→ shows in browser tab</span>
</div>
<span style="color:#1565c0;font-weight:700">&lt;/head&gt;</span>
</div>
<div style="background:#eeffee;border:2px solid #2e7d32;border-radius:8px;padding:14px">
<span style="color:#2e7d32;font-weight:700">&lt;body&gt;</span> <span style="color:#888;font-size:12px">← Everything the user SEES.</span>
<div style="background:#fff;border:1px solid #a5d6a7;border-radius:6px;padding:10px;margin:8px 0;font-size:13px">
<h1><strong>Hello, world!</strong></h1><br><p>This is my first webpage.</p>
</div>
<span style="color:#2e7d32;font-weight:700">&lt;/body&gt;</span>
</div>
<span style="color:#8e24aa;font-weight:700">&lt;/html&gt;</span>
</div>
</div></div>
<div class="card"><div class="cl">What It Looks Like in the Browser</div>
<div style="border:1px solid #ddd;border-radius:10px;overflow:hidden">
<div style="background:#eee;padding:8px 14px;font-size:12px;color:#555;display:flex;align-items:center;gap:8px">
<span style="width:10px;height:10px;border-radius:50%;background:#e53935;display:inline-block"></span>
<span style="width:10px;height:10px;border-radius:50%;background:#fbc02d;display:inline-block"></span>
<span style="width:10px;height:10px;border-radius:50%;background:#2e7d32;display:inline-block"></span>
<span style="margin-left:10px">📌 My Page</span>
</div>
<div style="padding:24px;background:#fff">
<h1 style="font-size:28px;margin-bottom:8px">Hello, world!</h1>
<p style="color:#555">This is my first webpage.</p>
</div>
</div>
<div class="note">That's it. Browser reads top to bottom and paints what it finds. [cite_start]No magic. [cite: 11-14]</div>
</div>
</body></html>

```

### 2. html/02-tags.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Tags, Elements & Attributes</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Tags, Elements & Attributes</h1><p>Opening/closing tags, self-closing tags, and attribute syntax</p></div>

<div class="card"><div class="cl">Anatomy of an Element</div>
<div class="demo" style="text-align:center;font-size:20px;font-family:monospace;padding:16px">
<span style="color:#e53935;font-weight:700">&lt;a</span><span style="color:#1565c0;font-weight:700"> href="https://google.com" target="_blank"</span><span style="color:#e53935;font-weight:700">&gt;</span><span style="color:#2e7d32;font-weight:700">Go to Google</span><span style="color:#e53935;font-weight:700">&lt;/a&gt;</span>
<div style="display:flex;justify-content:space-around;margin-top:14px;font-size:13px;font-family:sans-serif;font-weight:700;color:#555">
<span style="color:#e53935">↑<br>Opening tag</span><span style="color:#1565c0">↑<br>Attributes</span><span style="color:#2e7d32">↑<br>Content</span><span style="color:#e53935">↑<br>Closing tag</span>
</div>
</div></div>
<div class="card"><div class="cl">Self-Closing Tags — No closing tag needed</div>
<div class="demo" style="display:flex;flex-direction:column;gap:10px">
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">Line one<br>Line two — the &lt;br&gt; forced a new line</div>
<hr style="border:none;border-top:2px solid #ddd">
<p style="font-size:13px;color:#555">The line above is &lt;hr&gt;</p>
<div style="background:#f5f5f5;padding:10px;border-radius:6px;font-family:monospace;font-size:13px"><br> &nbsp;&nbsp; <hr> &nbsp;&nbsp; <img src="..."> &nbsp;&nbsp; <input> &nbsp;&nbsp; <link></div>
</div></div>
<div class="card"><div class="cl">Attributes — Extra info inside the opening tag</div>
<div class="demo" style="display:flex;flex-direction:column;gap:10px">
<div style="background:#fff;border:1px solid #ddd;padding:12px;border-radius:6px">
<code style="font-size:13px">&lt;a <span style="color:#1565c0">href="https://google.com"</span> <span style="color:#2e7d32">target="_blank"</span>&gt;Google&lt;/a&gt;</code><br>
[cite_start]<a href="https://google.com" target="_blank" style="color:#1565c0;margin-top:6px;display:inline-block">→ Google (opens new tab)</a> [cite: 15]
</div>
<div style="background:#fff;border:1px solid #ddd;padding:12px;border-radius:6px">
<code style="font-size:13px">&lt;img <span style="color:#1565c0">src="photo.jpg"</span> <span style="color:#2e7d32">alt="A photo"</span> <span style="color:#8e24aa">width="100"</span>&gt;</code>
</div>
</div></div>
</body></html>

```

### 3. html/03-text-formatting.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Text Tags</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Text Tags</h1><p>h1–h6, strong, em, u, s, code — all the text tags</p></div>

<div class="card"><div class="cl">Headings — h1 biggest, h6 smallest</div>
<div class="demo">
<h1 style="font-size:36px;margin-bottom:6px">h1 — Main Title of the Page</h1>
<h2 style="font-size:28px;margin-bottom:6px">h2 — Section Title</h2>
<h3 style="font-size:22px;margin-bottom:6px">h3 — Subsection</h3>
<h4 style="font-size:18px;margin-bottom:6px">h4 — Minor heading</h4>
<h5 style="font-size:15px;margin-bottom:6px">h5 — Small heading</h5>
<h6 style="font-size:13px">h6 — Smallest heading</h6>
</div>
<div class="note">Browser sizes these automatically. [cite_start]Use h1 once per page — it tells Google the main topic. [cite: 16]</div></div>
<div class="card"><div class="cl">Inline Formatting Tags</div>
<div class="demo" style="display:flex;flex-direction:column;gap:8px">
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;strong&gt;</code> → <strong>I am bold. [cite_start]I'm important!</strong> [cite: 17]</div>
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;em&gt;</code> → <em>I am italic. [cite_start]I'm emphasized!</em> [cite: 18]</div>
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;u&gt;</code> → <u>I am underlined!</u></div>
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;s&gt;</code> → <s>Old price: 49</s></div>
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;code&gt;</code> → Use <code>console.log()</code> to debug</div>
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;br&gt;</code> → Forces a<br>new line here</div>
<hr style="border:none;border-top:2px solid #eee;margin:4px 0">
<div style="background:#fff;padding:10px;border-radius:6px;border:1px solid #eee"><code style="color:#888;font-size:12px">&lt;hr&gt;</code> → that line above ↑</div>
</div></div>
<div class="card"><div class="cl">Combined in a real paragraph</div>
<div class="demo">
<p style="font-size:16px;line-height:2">The <strong>MacBook Pro</strong> is <em>only available</em> until <u>Friday</u>. [cite_start]Was <s>2499</s> — now just <strong style="color:#e53935">1999</strong>! [cite: 19]</p>
</div></div>
</body></html>

```

### 4. html/04-links.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Links</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Links</h1><p>href absolute, relative, and new tab</p></div>

<div class="card"><div class="cl">Three Destination Types</div>
<div class="demo" style="display:flex;flex-direction:column;gap:12px">
<div style="background:#fff;border:1px solid #ddd;padding:14px;border-radius:8px">
<div style="font-size:11px;font-weight:700;text-transform:uppercase;color:#e53935;margin-bottom:6px">Absolute URL — another website</div>
<code style="font-size:13px">&lt;a href="https://google.com"&gt;Google&lt;/a&gt;</code>
<div style="margin-top:8px"><a href="https://google.com" target="_blank" style="color:#1565c0">Google ↗</a></div>
</div>
<div style="background:#fff;border:1px solid #ddd;padding:14px;border-radius:8px">
<div style="font-size:11px;font-weight:700;text-transform:uppercase;color:#2e7d32;margin-bottom:6px">Relative URL — file in same folder</div>
<code style="font-size:13px">&lt;a href="03-text-formatting.html"&gt;Text Tags&lt;/a&gt;</code>
<div style="margin-top:8px"><a href="03-text-formatting.html" style="color:#1565c0">← Text Formatting page</a></div>
</div>
<div style="background:#fff;border:1px solid #ddd;padding:14px;border-radius:8px">
<div style="font-size:11px;font-weight:700;text-transform:uppercase;color:#8e24aa;margin-bottom:6px">Anchor — jump within same page</div>
<code style="font-size:13px">&lt;a href="#bottom"&gt;Jump to bottom&lt;/a&gt;</code>
<div style="margin-top:8px"><a href="#bottom" style="color:#1565c0">Jump to bottom of this page</a></div>
</div>
</div></div>
[cite_start]<div class="card"><div class="cl">target="_blank" — Open in New Tab [cite: 20]</div>
<div class="demo" style="display:flex;gap:12px;flex-wrap:wrap">
<a href="https://google.com" style="display:inline-block;padding:12px 24px;background:#e53935;color:white;border-radius:8px;text-decoration:none;font-weight:700">Same tab</a>
<a href="https://google.com" target="_blank" style="display:inline-block;padding:12px 24px;background:#2e7d32;color:white;border-radius:8px;text-decoration:none;font-weight:700">New tab ↗</a>
</div></div>
<div id="bottom" class="card"><div class="cl">The anchor target</div>
<div class="demo">You jumped here! [cite_start]This element has <code>id="bottom"</code>. [cite: 21]</div></div>
</body></html>

```

### 5. html/05-images.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Images</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Images</h1><p>src, alt, width — and what happens when things go wrong</p></div>

<div class="card"><div class="cl">Anatomy of &lt;img&gt;</div>
<div class="demo" style="font-family:monospace;font-size:16px;text-align:center;padding:16px">
<span style="color:#e53935;font-weight:700">&lt;img</span>
<span style="color:#1565c0;font-weight:700"> src="photo.jpg"</span>
<span style="color:#2e7d32;font-weight:700"> alt="A sunset"</span>
<span style="color:#8e24aa;font-weight:700"> width="300"</span>
<span style="color:#e53935;font-weight:700">&gt;</span>
<div style="display:flex;justify-content:space-around;margin-top:12px;font-size:13px;font-family:sans-serif;font-weight:700;color:#555">
<span style="color:#e53935">No closing tag</span><span style="color:#1565c0">File path</span><span style="color:#2e7d32">Fallback text</span><span style="color:#8e24aa">Width in px</span>
</div>
</div></div>
<div class="card"><div class="cl">Broken Image — Alt text kicks in</div>
<div class="demo" style="display:flex;gap:20px;align-items:flex-start;flex-wrap:wrap">
<div style="text-align:center">
<img src="this-does-not-exist.jpg" alt="A beautiful mountain view" style="display:block;margin:0 auto 8px;max-width:200px">
<code style="font-size:12px">&lt;img src="missing.jpg" alt="A beautiful mountain view"&gt;</code>
<p style="font-size:12px;color:#888;margin-top:6px">Browser shows broken icon + alt text</p>
</div>
</div>
<div class="note">alt text is also read by screen readers for blind users. Always include it. [cite_start]It's required. [cite: 22]</div></div>
<div class="card"><div class="cl">Controlling Size</div>
<div class="demo" style="display:flex;gap:14px;align-items:flex-end;flex-wrap:wrap">
<div style="text-align:center"><div style="width:50px;height:50px;background:#bbdefb;border:2px solid #1565c0;border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:700;color:#1565c0;margin:0 auto 6px">50px</div><code style="font-size:11px">width="50"</code></div>
<div style="text-align:center"><div style="width:100px;height:100px;background:#bbdefb;border:2px solid #1565c0;border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#1565c0;margin:0 auto 6px">100px</div><code style="font-size:11px">width="100"</code></div>
<div style="text-align:center"><div style="width:200px;height:100px;background:#bbdefb;border:2px solid #1565c0;border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#1565c0;margin:0 auto 6px">200×100px</div><code style="font-size:11px">width="200" height="100"</code></div>
</div></div>
</body></html>

```

### 6. html/06-lists.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Lists</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Lists</h1><p>ul (bullets) vs ol (numbers) — and nested lists</p></div>

<div class="card"><div class="cl">Side by Side: Unordered vs Ordered</div>
<div class="demo" style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
<div style="background:#fff;border:2px solid #e53935;padding:16px;border-radius:8px">
<div style="font-weight:700;color:#e53935;margin-bottom:10px;font-size:13px">&lt;ul&gt; Unordered — bullets</div>
<ul style="padding-left:20px;line-height:2.2"><li>Apples</li><li>Bananas</li><li>Cherries</li></ul>
</div>
<div style="background:#fff;border:2px solid #2e7d32;padding:16px;border-radius:8px">
<div style="font-weight:700;color:#2e7d32;margin-bottom:10px;font-size:13px">&lt;ol&gt; Ordered — numbers</div>
<ol style="padding-left:20px;line-height:2.2"><li>Boil water</li><li>Add pasta</li><li>Wait 10 min</li></ol>
</div>
</div>
[cite_start]<div class="note">You don't type bullets or numbers — the browser adds them automatically. [cite: 23]</div></div>
<div class="card"><div class="cl">Nested Lists</div>
<div class="demo">
<ul style="padding-left:20px;line-height:2">
<li>Fruits<ul style="padding-left:20px"><li>Apples</li><li>Bananas</li></ul></li>
<li>Vegetables<ul style="padding-left:20px"><li>Carrots</li><li>Broccoli</li></ul></li>
</ul>
</div></div>
</body></html>

```

### 7. html/07-forms.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Forms & Inputs</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Forms & Inputs</h1><p>Every input type the browser supports</p></div>

[cite_start]<div class="card"><div class="cl">All Input Types [cite: 24]</div>
<div class="demo" style="display:flex;flex-direction:column;gap:10px">
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="text"</code><input type="text" placeholder="Enter name" style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="email"</code><input type="email" placeholder="you@email.com" style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="password"</code><input type="password" placeholder="Hidden!" style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="number"</code><input type="number" value="42" style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px;width:80px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="date"</code><input type="date" style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="range"</code><input type="range" min="0" max="100" style="width:150px">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="checkbox"</code><label style="font-size:13px;display:flex;align-items:center;gap:6px"><input type="checkbox"> Remember me</label>
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="radio" name="color"</code><label style="margin-right:8px;font-size:13px;display:inline-flex;align-items:center;gap:4px"><input type="radio" name="color"> Red</label><label style="margin-right:8px;font-size:13px;display:inline-flex;align-items:center;gap:4px"><input type="radio" name="color"> Blue</label><label style="font-size:13px;display:inline-flex;align-items:center;gap:4px"><input type="radio" name="color"> Green</label>
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">type="file"</code><input type="file">
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">&lt;textarea&gt;</code><textarea placeholder="Write a message..." style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px;resize:vertical;height:55px"></textarea>
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">&lt;select&gt;</code><select style="padding:6px 10px;border:1.5px solid #ddd;border-radius:6px;font-size:13px"><option>JavaScript</option><option>Python</option><option>Java</option></select>
</div>
 <div style="display:flex;align-items:center;gap:12px;background:#fff;padding:10px;border-radius:6px;border:1px solid #eee">
<code style="min-width:200px;font-size:12px;color:#888">&lt;button&gt;</code><button style="padding:8px 16px;background:#e53935;color:white;border:none;border-radius:6px;cursor:pointer;font-weight:700">Submit</button> <button disabled style="padding:8px 16px;background:#ddd;color:#aaa;border:none;border-radius:6px;cursor:not-allowed;font-weight:700">Disabled</button>
</div>
</div>
<div class="note">Radio buttons with the same <code>name</code> are grouped — only one can be selected. [cite_start]Try clicking! [cite: 25]</div></div>
</body></html>

```

### 8. html/08-div-span.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — div and span</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>div and span</h1><p>Block vs inline — the two fundamental containers</p></div>

<div class="card"><div class="cl">div = BLOCK — takes full width, forces new line</div>
<div class="demo">
<div style="background:#ffebee;border:2px solid #e53935;border-radius:6px;padding:12px;margin-bottom:6px;font-weight:700;text-align:center">I am &lt;div&gt; — I take the FULL ROW ←→</div>
<div style="background:#e3f2fd;border:2px solid #1565c0;border-radius:6px;padding:12px;margin-bottom:6px;font-weight:700;text-align:center">Another &lt;div&gt; — forced to a NEW LINE automatically</div>
<div style="background:#e8f5e9;border:2px solid #2e7d32;border-radius:6px;padding:12px;font-weight:700;text-align:center">Third &lt;div&gt; — another new line</div>
</div>
<div class="note">Block tags: div, p, h1-h6, section, article, header, footer. They all stack vertically.</div></div>
<div class="card"><div class="cl">span = INLINE — sits inside text, no line break</div>
<div class="demo">
[cite_start]<p style="font-size:16px;line-height:2.5">Normal text here, then <span style="background:#fff9c4;border:2px solid #f9a825;padding:2px 8px;border-radius:4px;font-weight:700">I am a &lt;span&gt;</span> and text continues on the same line without breaking. [cite: 26, 27] Then <span style="background:#fce4ec;border:2px solid #e53935;color:#c62828;padding:2px 8px;border-radius:4px;font-weight:700">another span</span> — still same line!</p>
</div>
<div class="note">Inline tags: span, a, strong, em, code. [cite_start]They flow like words in a sentence. [cite: 28]</div></div>
<div class="card"><div class="cl">Real-World Pattern: div as card, span for highlights</div>
<div class="demo" style="display:flex;gap:14px;flex-wrap:wrap;align-items:flex-start">
<div style="background:#fff;border:1px solid #ddd;border-radius:10px;padding:16px;width:180px;box-shadow:0 2px 8px rgba(0,0,0,.08)">
<strong>Product</strong><p style="font-size:13px;color:#555;margin:6px 0">Description here.</p>
<button style="width:100%;padding:8px;background:#e53935;color:white;border:none;border-radius:6px;cursor:pointer;font-weight:700">Buy Now</button>
</div>
<p style="font-size:15px;line-height:2.5;flex:1">Price is <span style="color:#e53935;font-weight:800;font-size:18px">$9.99</span> — save <span style="background:#e8f5e9;color:#2e7d32;padding:2px 8px;border-radius:4px;font-weight:700">50% OFF</span>!</p>
</div></div>
</body></html>

```

### 9. html/09-semantic.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — Semantic Tags</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>Semantic Tags</h1><p>header, nav, main, section, article, aside, footer</p></div>

<div class="card"><div class="cl">The Same Layout — &lt;div&gt; vs Semantic Tags</div>
<div class="demo" style="display:grid;grid-template-columns:1fr 1fr;gap:14px">
<div>
<div style="font-size:11px;font-weight:700;text-transform:uppercase;color:#888;margin-bottom:8px">❌ With divs only</div>
<div style="font-family:monospace;font-size:12px;background:#1e1e2e;color:#cdd6f4;padding:12px;border-radius:8px;line-height:1.8">
&lt;div class="header"&gt;<br>
&nbsp;&lt;div class="nav"&gt;...<br>
&lt;div class="main"&gt;<br>
&nbsp;&lt;div class="section"&gt;...<br>
&lt;div class="footer"&gt;...
</div>
</div>
<div>
<div style="font-size:11px;font-weight:700;text-transform:uppercase;color:#2e7d32;margin-bottom:8px">✅ With semantic tags</div>
<div style="font-family:monospace;font-size:12px;background:#1e1e2e;color:#a6e3a1;padding:12px;border-radius:8px;line-height:1.8">
&lt;header&gt;<br>
&nbsp;&lt;nav&gt;...<br>
&lt;main&gt;<br>
&nbsp;&lt;section&gt;...<br>
[cite_start]&lt;footer&gt;... [cite: 29]
</div>
</div>
</div>
<div class="note">Both look identical. The difference: Google and screen readers understand semantic tags. [cite_start]Always use them. [cite: 30]</div></div>
<div class="card"><div class="cl">Visual Layout with All Semantic Tags</div>
<div class="demo">
<div style="border:2px solid #1565c0;border-radius:8px;overflow:hidden;font-size:13px">
<header style="background:#1565c0;color:white;padding:12px 16px;display:flex;justify-content:space-between;align-items:center">
<strong>&lt;header&gt; Logo & Site Name</strong>
<nav style="display:flex;gap:10px"><a href="#" style="color:white;font-weight:700;text-decoration:none">&lt;nav&gt; Home</a><a href="#" style="color:white;font-weight:700;text-decoration:none">About</a></nav>
</header>
<div style="display:flex">
<main style="flex:1;background:#e3f2fd;padding:14px">
<span style="font-size:10px;font-weight:700;color:#0d47a1">&lt;main&gt;</span>
<section style="background:#fff;border:1.5px solid #90caf9;border-radius:6px;padding:10px;margin-top:8px">
<span style="font-size:10px;font-weight:700;color:#0d47a1">&lt;section&gt;</span>
<h2 style="font-size:15px;margin:4px 0">Welcome</h2>
<p style="font-size:12px;color:#555">Grouped related content.</p>
</section>
<article style="background:#fff;border:1.5px solid #90caf9;border-radius:6px;padding:10px;margin-top:8px">
<span style="font-size:10px;font-weight:700;color:#0d47a1">&lt;article&gt;</span>
<h3 style="font-size:13px;margin:4px 0">Blog Post</h3>
<p style="font-size:12px;color:#555">Standalone content.</p>
</article>
</main>
<aside style="width:120px;background:#fff3e0;padding:12px;border-left:2px solid #ff8f00">
<span style="font-size:10px;font-weight:700;color:#e65100">&lt;aside&gt;</span>
<p style="font-size:12px;margin-top:4px;color:#555">Sidebar. [cite_start]Secondary. [cite: 31]</p>
</aside>
</div>
<footer style="background:#333;color:white;padding:10px 16px;text-align:center;font-size:12px">&lt;footer&gt; © 2024</footer>
</div>
</div></div>
</body></html>

```

### 10. html/10-attributes.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>HTML — HTML Attributes</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #e53935; }
.badge { display:inline-block; background:#e53935; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#e53935; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#e53935; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">HTML</div><h1>HTML Attributes</h1><p>id, class, disabled, required — what they do</p></div>

<div class="card"><div class="cl">id vs class — The key difference</div>
<div class="demo" style="display:grid;grid-template-columns:1fr 1fr;gap:14px">
<div style="background:#fff3e0;border:2px solid #f57f17;padding:14px;border-radius:8px">
<div style="font-weight:800;color:#e65100;margin-bottom:8px">id — Unique. One element only.</div>
<div style="background:#fff;border:1px solid #eee;padding:10px;border-radius:6px;text-align:center;margin-bottom:6px">I am #hero-title</div>
<code style="font-size:12px">&lt;h1 id="hero-title"&gt;</code>
<p style="font-size:12px;color:#555;margin-top:66px">Like a passport — one person, one number. Used in CSS with # and JS to find ONE element.</p>
</div>
<div style="background:#e8f5e9;border:2px solid #2e7d32;padding:14px;border-radius:8px">
<div style="font-weight:800;color:#1b5e20;margin-bottom:8px">class — Shared. [cite_start]Many elements. [cite: 32]</div>
<div style="background:#fff;border:1px solid #eee;padding:10px;border-radius:6px;text-align:center;margin-bottom:4px">class="card"</div>
<div style="background:#fff;border:1px solid #eee;padding:10px;border-radius:6px;text-align:center;margin-bottom:6px">class="card" too!</div>
<code style="font-size:12px">&lt;div class="card"&gt;</code>
<p style="font-size:12px;color:#555;margin-top:6px">Like a job title — many people can share it. [cite_start]Used in CSS with . to style groups. [cite: 33]</p>
</div>
</div></div>
<div class="card"><div class="cl">disabled — Makes it unclickable and greyed out</div>
<div class="demo" style="display:flex;gap:16px;align-items:center;flex-wrap:wrap">
<div style="text-align:center"><button style="padding:10px 20px;background:#e53935;color:white;border:none;border-radius:6px;cursor:pointer;font-weight:700">Normal</button><p style="font-size:12px;margin-top:4px">&lt;button&gt;</p></div>
<div style="text-align:center"><button disabled style="padding:10px 20px;background:#ddd;color:#aaa;border:none;border-radius:6px;cursor:not-allowed;font-weight:700">Disabled</button><p style="font-size:12px;margin-top:4px">&lt;button disabled&gt;</p></div>
<div style="text-align:center"><input type="text" value="Read only" disabled style="padding:8px 12px;border:1.5px solid #ddd;border-radius:6px;background:#f5f5f5;color:#aaa;cursor:not-allowed"><p style="font-size:12px;margin-top:4px">&lt;input disabled&gt;</p></div>
</div></div>
<div class="card"><div class="cl">required — Form won't submit without it</div>
<div class="demo">
<form onsubmit="return false" style="display:flex;flex-direction:column;gap:10px;max-width:300px">
<input type="text" placeholder="Name (required)" required style="padding:8px 12px;border:1.5px solid #e53935;border-radius:6px;font-size:13px">
<input type="email" placeholder="Email (optional)" style="padding:8px 12px;border:1.5px solid #ddd;border-radius:6px;font-size:13px">
<button type="submit" style="padding:10px;background:#e53935;color:white;border:none;border-radius:6px;cursor:pointer;font-weight:700">Try submitting empty!</button>
</form>
</div></div>
</body></html>

```

Here are the next ten files from the workshop notes, covering the **CSS Fundamentals** section.

### 11. css/01-selectors.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Selectors</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Selectors</h1><p>How to target elements: tag, .class, and #id</p></div>

<div class="card"><div class="cl">1. Tag Selector — targets all elements of that type</div>
<div class="demo">
<div style="background:#fff;padding:12px;border-radius:8px;margin-bottom:10px">
<p style="color:#8e24aa;font-weight:700">All &lt;p&gt; tags will be purple and bold.</p>
</div>
<pre>p {
  color: purple;
  font-weight: bold;
}</pre>
</div></div>
<div class="card"><div class="cl">2. Class Selector (.) — targets elements with that class</div>
<div class="demo">
<div style="background:#e8f5e9;color:#2e7d32;padding:12px;border-radius:8px;border:2px solid #2e7d32;margin-bottom:10px;font-weight:700">Success Message</div>
<pre>.success {
  background: #e8f5e9;
  color: #2e7d32;
  border: 2px solid #2e7d32;
}</pre>
</div>
<div class="note">Use classes for styles you want to reuse many times.</div></div>
<div class="card"><div class="cl">3. ID Selector (#) — targets one specific element</div>
<div class="demo">
<div style="background:#1a1a2e;color:#fff;padding:12px;border-radius:8px;text-align:center">Special Unique Header</div>
<pre>#main-header {
  background: #1a1a2e;
  color: white;
  text-align: center;
}</pre>
</div></div>
</body></html>

```

### 12. css/02-colors.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Colors</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Colors</h1><p>Names, Hex, and RGB(A)</p></div>

<div class="card"><div class="cl">Three ways to write the same red</div>
<div class="demo" style="display:flex;flex-direction:column;gap:12px">
<div style="background:red;color:white;padding:12px;border-radius:8px;text-align:center;font-weight:700">color: red; (Named)</div>
<div style="background:#ff0000;color:white;padding:12px;border-radius:8px;text-align:center;font-weight:700">color: #ff0000; (Hex)</div>
<div style="background:rgb(255,0,0);color:white;padding:12px;border-radius:8px;text-align:center;font-weight:700">color: rgb(255, 0, 0); (RGB)</div>
</div></div>
<div class="card"><div class="cl">RGBA — The "A" is for Alpha (Transparency)</div>
<div class="demo" style="background:url('https://www.transparenttextures.com/patterns/cubes.png');padding:40px;border-radius:12px">
<div style="background:rgba(142, 36, 170, 1);color:white;padding:10px;margin-bottom:8px;text-align:center">rgba(..., 1.0) - Solid</div>
<div style="background:rgba(142, 36, 170, 0.7);color:white;padding:10px;margin-bottom:8px;text-align:center">rgba(..., 0.7) - 70%</div>
<div style="background:rgba(142, 36, 170, 0.3);color:white;padding:10px;text-align:center">rgba(..., 0.3) - 30%</div>
</div>
<div class="note">0 is fully invisible, 1 is fully solid. Great for overlays!</div></div>
</body></html>

```

### 13. css/03-box-model.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — The Box Model</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>The Box Model</h1><p>Padding, Border, and Margin</p></div>

<div class="card"><div class="cl">Visualizing the Box</div>
<div class="demo" style="background:#f5f5f5;padding:40px;text-align:center">
<div style="display:inline-block;background:#ffd54f;padding:30px;border:10px solid #f57f17;outline:20px solid #fff9c4;margin:20px">
<div style="background:#fff;padding:10px;border-radius:4px;font-weight:700">CONTENT</div>
</div>
<div style="display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-top:40px;text-align:left;font-size:13px">
<div><span style="color:#f9a825;font-weight:800">■ Margin:</span> Space OUTSIDE the border (pushes other elements away)</div>
<div><span style="color:#f57f17;font-weight:800">■ Border:</span> The line around the content</div>
<div><span style="color:#ffb300;font-weight:800">■ Padding:</span> Space INSIDE the border (adds breathing room for content)</div>
</div>
</div></div>
<div class="card"><div class="cl">Padding vs Margin Example</div>
<div class="demo" style="display:flex;gap:20px">
<div style="background:#fff;border:2px solid #8e24aa;padding:30px">Big Padding</div>
<div style="background:#fff;border:2px solid #8e24aa;margin:30px">Big Margin</div>
</div>
<div class="note">The box on the left is physically larger because of padding. The box on the right is further away from things because of margin.</div></div>
</body></html>

```

### 14. css/04-typography.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Typography</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Typography</h1><p>Fonts, sizes, weights, and spacing</p></div>

<div class="card"><div class="cl">Common Text Properties</div>
<div class="demo" style="display:flex;flex-direction:column;gap:16px">
<div style="font-size:24px;font-weight:800">font-size: 24px; font-weight: 800;</div>
<div style="text-align:center;color:#888">text-align: center;</div>
<div style="text-transform:uppercase;letter-spacing:4px">UPPERCASE & LETTER SPACING</div>
<div style="line-height:2.5;background:#fff;padding:10px;border-radius:6px">This paragraph has a line-height of 2.5. It makes the text much easier to read by adding vertical space between lines.</div>
</div></div>
<div class="card"><div class="cl">Font Family — Serif vs Sans-Serif</div>
<div class="demo">
<div style="font-family:serif;font-size:20px;margin-bottom:10px">Serif (with "feet"): Times New Roman</div>
<div style="font-family:sans-serif;font-size:20px">Sans-Serif (clean): Arial, Helvetica, Segoe UI</div>
</div></div>
</body></html>

```

### 15. css/05-flexbox-basics.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Flexbox Basics</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Flexbox Basics</h1><p>The modern way to align elements in a row</p></div>

<div class="card"><div class="cl">Default Row Behavior</div>
<div class="demo" style="display:flex;gap:10px">
<div style="background:#8e24aa;color:white;padding:20px;border-radius:8px">1</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:8px">2</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:8px">3</div>
</div>
<pre>display: flex;
gap: 10px;</pre>
</div>
<div class="card"><div class="cl">Centering Everything</div>
<div class="demo" style="display:flex;justify-content:center;align-items:center;height:150px;background:#eee;border-radius:12px">
<div style="background:#8e24aa;color:white;padding:30px;border-radius:50%;font-weight:700">Centered!</div>
</div>
<pre>display: flex;
justify-content: center; /* horizontal */
align-items: center;     /* vertical */</pre>
</div></body></html>

```

### 16. css/06-flex-justify.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Flex Justify</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Flex Justify</h1><p>Controlling horizontal distribution</p></div>

<div class="card"><div class="cl">justify-content: space-between (Common for Navbars)</div>
<div class="demo" style="display:flex;justify-content:space-between;background:#eee;padding:10px;border-radius:8px">
<div style="background:#8e24aa;color:white;padding:10px 20px;border-radius:6px">Logo</div>
<div style="background:#8e24aa;color:white;padding:10px 20px;border-radius:6px">Links</div>
</div></div>
<div class="card"><div class="cl">justify-content: space-around</div>
<div class="demo" style="display:flex;justify-content:space-around;background:#eee;padding:10px;border-radius:8px">
<div style="background:#8e24aa;color:white;padding:10px;border-radius:6px">Item 1</div>
<div style="background:#8e24aa;color:white;padding:10px;border-radius:6px">Item 2</div>
<div style="background:#8e24aa;color:white;padding:10px;border-radius:6px">Item 3</div>
</div></div>
<div class="card"><div class="cl">justify-content: flex-end</div>
<div class="demo" style="display:flex;justify-content:flex-end;gap:10px;background:#eee;padding:10px;border-radius:8px">
<div style="background:#8e24aa;color:white;padding:10px;border-radius:6px">Login</div>
<div style="background:#8e24aa;color:white;padding:10px;border-radius:6px">Sign Up</div>
</div></div>
</body></html>

```

### 17. css/07-flex-direction.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Flex Direction</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Flex Direction</h1><p>Row vs Column</p></div>

<div class="card"><div class="cl">flex-direction: column</div>
<div class="demo" style="display:flex;flex-direction:column;gap:10px;width:150px">
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px;text-align:center">1</div>
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px;text-align:center">2</div>
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px;text-align:center">3</div>
</div>
<div class="note">In column mode, <code>justify-content</code> controls vertical alignment and <code>align-items</code> controls horizontal!</div></div>
<div class="card"><div class="cl">flex-direction: row-reverse</div>
<div class="demo" style="display:flex;flex-direction:row-reverse;gap:10px">
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px">1</div>
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px">2</div>
<div style="background:#8e24aa;color:white;padding:15px;border-radius:6px">3</div>
</div></div>
</body></html>

```

### 18. css/08-grid-basics.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Grid Basics</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Grid Basics</h1><p>Creating 2D layouts (rows and columns)</p></div>

<div class="card"><div class="cl">3-Column Grid</div>
<div class="demo" style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px">
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">1</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">2</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">3</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">4</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">5</div>
<div style="background:#8e24aa;color:white;padding:20px;border-radius:6px;text-align:center">6</div>
</div>
<pre>display: grid;
grid-template-columns: 1fr 1fr 1fr; /* 3 equal parts */
gap: 10px;</pre>
</div>
<div class="card"><div class="cl">Sidebar Layout</div>
<div class="demo" style="display:grid;grid-template-columns:150px 1fr;gap:15px">
<div style="background:#eee;padding:20px;border-radius:6px;border:1px solid #ddd">Sidebar</div>
<div style="background:#fff;padding:20px;border-radius:6px;border:1px solid #ddd">Main Content Area</div>
</div>
<pre>grid-template-columns: 150px 1fr;</pre>
</div></body></html>

```

### 19. css/09-positioning.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Positioning</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Positioning</h1><p>relative, absolute, and fixed</p></div>

<div class="card"><div class="cl">Position: Absolute (relative to parent)</div>
<div class="demo" style="height:150px;position:relative;background:#eee;border-radius:12px">
<div style="position:absolute;top:10px;right:10px;background:#e53935;color:white;padding:5px 12px;border-radius:20px;font-size:12px;font-weight:700">Sale!</div>
<div style="padding:40px">This card has <code>position: relative</code> so the red badge can be pinned to the corner.</div>
</div></div>
<div class="card"><div class="cl">Position: Fixed (sticks to screen)</div>
<div class="demo" style="height:100px;overflow-y:scroll;background:#fff;border:1px solid #ddd;padding:10px">
<div style="background:#8e24aa;color:white;padding:5px;text-align:center;margin-bottom:10px">I will scroll away...</div>
<div style="background:#8e24aa;color:white;padding:5px;text-align:center;margin-bottom:10px">Scroll me!</div>
<div style="background:#8e24aa;color:white;padding:5px;text-align:center;margin-bottom:10px">Keep going...</div>
</div>
<div class="note">Fixed elements stay in the same place even when you scroll the whole page (like navbars or chat bubbles).</div></div>
</body></html>

```

### 20. css/10-hover-transitions.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Hover & Transitions</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#8e24aa; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.btn:hover { opacity:.85; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.ipt:focus { border-color:#8e24aa; }
.out { margin-top:12px; padding:12px 16px; background:#f1f8e9; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #c5e1a5; min-height:40px; white-space:pre-wrap; }
</style>
<style>
  .hover-card { transition: all 0.3s ease; cursor: pointer; }
  .hover-card:hover { transform: translateY(-10px); box-shadow: 0 10px 20px rgba(0,0,0,0.1); background: #fff; }
  .hover-btn { background: #8e24aa; color: white; border: none; padding: 12px 24px; border-radius: 8px; font-weight: 700; transition: 0.2s; cursor: pointer; }
  .hover-btn:hover { background: #ab47bc; transform: scale(1.05); }
  .hover-btn:active { transform: scale(0.95); }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Hover & Transitions</h1><p>Making things feel interactive</p></div>

<div class="card"><div class="cl">Smooth Hover Button</div>
<div class="demo" style="text-align:center">
<button class="hover-btn">Hover Me!</button>
</div>
<pre>.btn { transition: 0.2s; }
.btn:hover { transform: scale(1.05); }</pre>
</div>
<div class="card"><div class="cl">Hoverable Card</div>
<div class="demo">
<div class="hover-card" style="border:1px solid #ddd;padding:20px;border-radius:12px;background:#f9f9f9;text-align:center">
<h3 style="margin-bottom:8px">Interactive Card</h3>
<p style="color:#666">Hover over this box to see it lift up smoothly.</p>
</div>
</div></div>
</body></html>

```

Here are the next ten files, which conclude the **CSS** section and begin the **JavaScript Fundamentals** series.

### 21. css/11-responsive-media-queries.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>CSS — Media Queries</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #8e24aa; }
.badge { display:inline-block; background:#8e24aa; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.note { background:#fff8e1; border-left:3px solid #ffca28; padding:10px 14px; border-radius:0 6px 6px 0; font-size:12px; color:#555; margin-top:10px; }

.responsive-box { background: #8e24aa; color: white; padding: 20px; text-align: center; border-radius: 8px; transition: 0.3s; }

/* Mobile logic */
@media (max-width: 600px) {
  .responsive-box { background: #e53935; }
  .responsive-box::after { content: " (Mobile View)"; }
}
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">CSS</div><h1>Media Queries</h1><p>Changing styles based on screen size</p></div>

<div class="card"><div class="cl">Resize your browser window</div>
<div class="demo">
<div class="responsive-box">The background color changes at 600px</div>
</div>
<pre>@media (max-width: 600px) {
  .responsive-box {
    background: red;
  }
}</pre>
</div>
<div class="note">Media queries allow you to create layouts that work on both Phones and Desktop computers.</div>
</body></html>

```

### 22. js/01-variables.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Variables</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Variables</h1><p>Storing data using let and const</p></div>

<div class="card"><div class="cl">Declaring Variables</div>
<div class="demo">
<button class="btn" onclick="runVars()">Run Code</button>
<div id="output" class="out">Output will appear here...</div>
<pre>let name = "Alex";  // Can change
const age = 25;    // Cannot change

name = "Sam"; // This is allowed
// age = 30;  // This would cause an error!</pre>
</div></div>

<script>
function runVars() {
  let name = "Alex";
  const age = 25;
  name = "Sam";
  document.getElementById('output').innerText = `Name: ${name}, Age: ${age}`;
}
</script>
</body></html>

```

### 23. js/02-data-types.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Data Types</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Data Types</h1><p>Strings, Numbers, and Booleans</p></div>

<div class="card"><div class="cl">Checking Types with typeof</div>
<div class="demo">
<button class="btn" onclick="checkTypes()">Identify Types</button>
<div id="output" class="out">Click button to see types...</div>
<pre>let text = "Hello";    // String
let score = 100;       // Number
let isReady = true;    // Boolean</pre>
</div></div>

<script>
function checkTypes() {
  let text = "Hello";
  let score = 100;
  let isReady = true;
  document.getElementById('output').innerHTML = `
    "Hello" is: <b>${typeof text}</b><br>
    100 is: <b>${typeof score}</b><br>
    true is: <b>${typeof isReady}</b>
  `;
}
</script>
</body></html>

```

### 24. js/03-strings.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Strings</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Strings</h1><p>Combining text with Template Literals</p></div>

<div class="card"><div class="cl">Dynamic Greeting</div>
<div class="demo">
<input type="text" id="nameInput" class="ipt" placeholder="Enter name...">
<button class="btn" onclick="greet()">Greet</button>
<div id="output" class="out">Hello...</div>
<pre>const name = "Alex";
const msg = `Hello, ${name}!`; // Template Literal</pre>
</div></div>

<script>
function greet() {
  const name = document.getElementById('nameInput').value || "Friend";
  document.getElementById('output').innerText = `Hello, ${name}! Welcome to the workshop.`;
}
</script>
</body></html>

```

### 25. js/04-numbers-math.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Numbers & Math</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Numbers & Math</h1><p>Arithmetic and Randomness</p></div>

<div class="card"><div class="cl">Random Number Generator (1-10)</div>
<div class="demo">
<button class="btn" onclick="roll()">Roll Dice</button>
<div id="output" class="out">0</div>
<pre>let num = Math.random() * 10;
let dice = Math.floor(num) + 1;</pre>
</div></div>

<script>
function roll() {
  const result = Math.floor(Math.random() * 10) + 1;
  document.getElementById('output').innerText = result;
}
</script>
</body></html>

```

### 26. js/05-if-statements.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — If Statements</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.ipt { padding:8px 12px; border-radius:6px; border:1.5px solid #ddd; font-size:13px; outline:none; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>If Statements</h1><p>Making decisions in code</p></div>

<div class="card"><div class="cl">Age Checker</div>
<div class="demo">
<input type="number" id="ageInput" class="ipt" placeholder="Enter age...">
<button class="btn" onclick="checkAge()">Check</button>
<div id="output" class="out">...</div>
<pre>if (age >= 18) {
  status = "Adult";
} else {
  status = "Minor";
}</pre>
</div></div>

<script>
function checkAge() {
  const age = document.getElementById('ageInput').value;
  const out = document.getElementById('output');
  if (!age) return;
  
  if (age >= 18) {
    out.innerText = "Access Granted: You are an adult.";
    out.style.background = "#e8f5e9";
  } else {
    out.innerText = "Access Denied: You are a minor.";
    out.style.background = "#ffebee";
  }
}
</script>
</body></html>

```

### 27. js/06-functions.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Functions</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Functions</h1><p>Reusable blocks of code</p></div>

<div class="card"><div class="cl">Square Calculator</div>
<div class="demo">
<button class="btn" onclick="showSquare(5)">Square of 5</button>
<button class="btn" onclick="showSquare(9)">Square of 9</button>
<div id="output" class="out">...</div>
<pre>function square(n) {
  return n * n;
}</pre>
</div></div>

<script>
function square(n) { return n * n; }

function showSquare(n) {
  const res = square(n);
  document.getElementById('output').innerText = `The square of ${n} is ${res}.`;
}
</script>
</body></html>

```

### 28. js/07-arrays.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Arrays</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Arrays</h1><p>Storing lists of data</p></div>

<div class="card"><div class="cl">Accessing Array Items</div>
<div class="demo">
<button class="btn" onclick="showFruit(0)">Index 0</button>
<button class="btn" onclick="showFruit(1)">Index 1</button>
<button class="btn" onclick="showFruit(2)">Index 2</button>
<div id="output" class="out">...</div>
<pre>const fruits = ["🍎", "🍌", "🍇"];
console.log(fruits[0]); // "🍎"</pre>
</div></div>

<script>
const fruits = ["🍎 Apple", "🍌 Banana", "🍇 Grape"];
function showFruit(i) {
  document.getElementById('output').innerText = fruits[i];
}
</script>
</body></html>

```

### 29. js/08-loops.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Loops</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Loops</h1><p>Repeating actions efficiently</p></div>

<div class="card"><div class="cl">For Loop — Counting to 5</div>
<div class="demo">
<button class="btn" onclick="runLoop()">Start Loop</button>
<div id="output" class="out">...</div>
<pre>for (let i = 1; i <= 5; i++) {
  console.log(i);
}</pre>
</div></div>

<script>
function runLoop() {
  let res = "";
  for (let i = 1; i <= 5; i++) {
    res += `Iteration: ${i}\n`;
  }
  document.getElementById('output').innerText = res;
}
</script>
</body></html>

```

### 30. js/09-objects.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Objects</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Objects</h1><p>Grouping related data together</p></div>

<div class="card"><div class="cl">The Car Object</div>
<div class="demo">
<button class="btn" onclick="showObject()">Get Info</button>
<div id="output" class="out">...</div>
<pre>const car = {
  make: "Tesla",
  model: "Model 3",
  year: 2023
};</pre>
</div></div>

<script>
function showObject() {
  const car = { make: "Tesla", model: "Model 3", year: 2023 };
  document.getElementById('output').innerText = `${car.year} ${car.make} ${car.model}`;
}
</script>
</body></html>

```

Here are the final ten files, concluding the **JavaScript** basics and covering **DOM Manipulation**.

### 31. js/10-arrow-functions.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>JS — Arrow Functions</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #f57f17; }
.badge { display:inline-block; background:#f57f17; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#f57f17; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
.out { margin-top:12px; padding:12px 16px; background:#fffde7; border-radius:8px; font-family:monospace; font-size:13px; border:1.5px solid #fff176; min-height:40px; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">JS</div><h1>Arrow Functions</h1><p>Shorter syntax for functions</p></div>

<div class="card"><div class="cl">Modern Syntax</div>
<div class="demo">
<button class="btn" onclick="runArrow()">Say Hello</button>
<div id="output" class="out">...</div>
<pre>// Traditional
function add(a, b) { return a + b; }

// Arrow Function
const add = (a, b) => a + b;</pre>
</div></div>

<script>
const greet = (user) => `Welcome back, ${user}!`;
function runArrow() {
  document.getElementById('output').innerText = greet("Developer");
}
</script>
</body></html>

```

### 32. dom/01-getElementById.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — getElementById</title>
<style>
,::before,*::after { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
.back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
.back:hover { background:#f5f5f5; }
.hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
.badge { display:inline-block; background:#1e88e5; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
.hdr h1 { font-size:22px; margin-bottom:4px; }
.hdr p { opacity:.6; font-size:13px; }
.card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
.cl { font-size:11px; font-weight:800; text-transform:uppercase; letter-spacing:1px; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
.demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
pre { background:#1e1e2e; color:#cdd6f4; border-radius:8px; padding:14px 16px; font-size:12px; line-height:1.7; overflow-x:auto; margin-top:12px; font-family:"Courier New",monospace; white-space:pre; }
.btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#1e88e5; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:4px 4px 4px 0; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">DOM</div><h1>getElementById</h1><p>Selecting a single element by its ID</p></div>

<div class="card"><div class="cl">Change Text Content</div>
<div class="demo">
<h2 id="main-title">Original Title</h2>
<button class="btn" onclick="change()">Update Title</button>
<pre>const el = document.getElementById('main-title');
el.innerText = "New Title!";</pre>
</div></div>

<script>
function change() {
  document.getElementById('main-title').innerText = "DOM Manipulated! 🎉";
}
</script>
</body></html>

```

### 33. dom/02-querySelector.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — querySelector</title>
<style>
/* Same CSS as above... */
.highlight { color: #1e88e5; font-weight: 800; border-bottom: 2px solid; }
</style>
</head>
<body>
<div class="card"><div class="cl">Select like CSS</div>
<div class="demo">
<p class="text-box">I am a paragraph with a class.</p>
<button class="btn" onclick="highlight()">Highlight Box</button>
<pre>const el = document.querySelector('.text-box');
el.classList.add('highlight');</pre>
</div></div>

<script>
function highlight() {
  document.querySelector('.text-box').classList.toggle('highlight');
}
</script>
</body></html>

```

### 34. dom/03-changing-styles.html

```html
<div class="card"><div class="cl">Direct Style Injection</div>
<div class="demo" style="text-align:center">
<div id="box" style="width:100px;height:100px;background:#ddd;margin:0 auto 15px;border-radius:8px"></div>
<button class="btn" onclick="paint('red')">Red</button>
<button class="btn" onclick="paint('blue')">Blue</button>
<pre>el.style.backgroundColor = "blue";
el.style.borderRadius = "50%";</pre>
</div></div>

<script>
function paint(color) {
  const b = document.getElementById('box');
  b.style.background = color === 'red' ? '#e53935' : '#1e88e5';
  b.style.transform = "scale(1.1)";
}
</script>

```

### 35. dom/04-event-listeners.html

```html
<div class="card"><div class="cl">Listening for Clicks</div>
<div class="demo">
<button id="alertBtn" class="btn">Click Me (addEventListener)</button>
<pre>const btn = document.getElementById('btn');
btn.addEventListener('click', () => {
  alert('Clicked!');
});</pre>
</div></div>

<script>
document.getElementById('alertBtn').addEventListener('click', () => {
  alert('Event Listener Triggered! 🚀');
});
</script>

```

### 36. dom/05-input-values.html

```html
<div class="card"><div class="cl">Reading User Input</div>
<div class="demo">
<input type="color" id="colorPicker" class="ipt" style="height:40px;width:100%">
<p id="colorVal" style="margin-top:10px;font-weight:700">Selected: #000000</p>
</div></div>

<script>
document.getElementById('colorPicker').addEventListener('input', (e) => {
  document.getElementById('colorVal').innerText = `Selected: ${e.target.value}`;
  document.body.style.background = e.target.value + "22"; // Light tint
});
</script>

```

### 37. dom/06-creating-elements.html

```html
<div class="card"><div class="cl">Adding to the DOM</div>
<div class="demo">
<button class="btn" onclick="addMsg()">Add Message</button>
<div id="list" style="margin-top:15px"></div>
<pre>const p = document.createElement('p');
p.innerText = "New item";
document.body.appendChild(p);</pre>
</div></div>

<script>
function addMsg() {
  const p = document.createElement('div');
  p.innerText = "New Message Added at " + new Date().toLocaleTimeString();
  p.style.padding = "8px";
  p.style.borderBottom = "1px solid #eee";
  document.getElementById('list').prepend(p);
}
</script>

```

### 38. dom/07-innerhtml-vs-text.html

```html
<div class="card"><div class="cl">HTML Injection</div>
<div class="demo">
<div id="target" style="padding:15px;background:#eee;border-radius:8px">Normal text.</div>
<button class="btn" onclick="inject()">Inject HTML</button>
</div></div>

<script>
function inject() {
  document.getElementById('target').innerHTML = 
    `<h3 style="color:red">Alert!</h3><p>This is <b>bold</b>.</p>`;
}
</script>

```

### 39. dom/08-timers.html

```html
<div class="card"><div class="cl">setTimeout & setInterval</div>
<div class="demo">
<h1 id="timer">0</h1>
<button class="btn" onclick="start()">Start Counter</button>
<pre>setInterval(() => {
  count++;
}, 1000);</pre>
</div></div>

<script>
let count = 0;
function start() {
  setInterval(() => {
    count++;
    document.getElementById('timer').innerText = count;
  }, 1000);
}
</script>

```

### 40. dom/09-final-demo.html

```html
<div class="card"><div class="cl">Simple Counter App</div>
<div class="demo" style="text-align:center">
<h1 id="val" style="font-size:48px">0</h1>
<button class="btn" onclick="change(-1)">-</button>
<button class="btn" onclick="change(1)">+</button>
</div></div>

<script>
let v = 0;
function change(amt) {
  v += amt;
  const el = document.getElementById('val');
  el.innerText = v;
  el.style.color = v < 0 ? "red" : (v > 0 ? "green" : "black");
}
</script>

```


Starting from file 33, here is the full, standalone code for each remaining file in the workshop series.

### 33. dom/02-querySelector.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — querySelector</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; color: #1a1a2e; line-height: 1.5; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .badge { display:inline-block; background:#1e88e5; color:#fff; font-size:10px; font-weight:800; letter-spacing:1.5px; text-transform:uppercase; padding:3px 10px; border-radius:20px; margin-bottom:8px; }
  .hdr h1 { font-size:22px; margin-bottom:4px; }
  .card { background:#fff; border-radius:12px; padding:22px; margin-bottom:16px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .cl { font-size:11px; font-weight:800; text-transform:uppercase; color:#aaa; margin-bottom:14px; padding-bottom:9px; border-bottom:2px solid #f5f5f5; }
  .demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; }
  .btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; background:#1e88e5; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin-top:10px; }
  .highlight { background: #fff59d; color: #1a1a2e; padding: 5px; border-radius: 4px; font-weight: 800; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">DOM</div><h1>querySelector</h1><p>Select elements using CSS-style selectors</p></div>
<div class="card">
  <div class="cl">Select by Class</div>
  <div class="demo">
    <p class="text-box">I am a paragraph with a class.</p>
    <button class="btn" onclick="highlight()">Toggle Highlight Class</button>
  </div>
</div>
<script>
function highlight() {
  document.querySelector('.text-box').classList.toggle('highlight');
}
</script>
</body></html>

```

### 34. dom/03-changing-styles.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Changing Styles</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .badge { display:inline-block; background:#1e88e5; color:#fff; font-size:10px; font-weight:800; text-transform:uppercase; padding:3px 10px; border-radius:20px; }
  .card { background:#fff; border-radius:12px; padding:22px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .demo { background:#f8faff; border:1.5px dashed #c5cae9; border-radius:8px; padding:20px; text-align:center; }
  .btn { display:inline-block; padding:8px 18px; border-radius:6px; border:none; color:#fff; font-weight:700; cursor:pointer; font-size:13px; margin:5px; }
  #box { width:100px; height:100px; background:#ddd; margin:0 auto 15px; border-radius:8px; transition: 0.3s; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><div class="badge">DOM</div><h1>Style Injection</h1><p>Modify CSS directly via JavaScript</p></div>
<div class="card">
  <div class="demo">
    <div id="box"></div>
    <button class="btn" style="background:#e53935" onclick="paint('#e53935')">Red</button>
    <button class="btn" style="background:#1e88e5" onclick="paint('#1e88e5')">Blue</button>
  </div>
</div>
<script>
function paint(color) {
  const b = document.getElementById('box');
  b.style.backgroundColor = color;
  b.style.transform = "scale(1.1)";
}
</script>
</body></html>

```

### 35. dom/04-event-listeners.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Event Listeners</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; box-shadow:0 1px 5px rgba(0,0,0,.12); }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:22px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .btn { display:inline-block; padding:12px 24px; border-radius:6px; border:none; background:#1e88e5; color:#fff; font-weight:700; cursor:pointer; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>Event Listeners</h1><p>Modern way to handle interactions</p></div>
<div class="card">
  <button id="alertBtn" class="btn">Click Me (addEventListener)</button>
</div>
<script>
document.getElementById('alertBtn').addEventListener('click', () => {
  alert('Event Listener Triggered! 🚀');
});
</script>
</body></html>

```

### 36. dom/05-input-values.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Input Values</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; transition: 0.2s; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:22px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .ipt { height:50px; width:100%; cursor:pointer; border:none; background:none; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>Reading User Input</h1><p>Capture data in real-time</p></div>
<div class="card">
  <input type="color" id="colorPicker" class="ipt">
  <p id="colorVal" style="margin-top:15px; font-weight:700; text-align:center">Selected: #000000</p>
</div>
<script>
document.getElementById('colorPicker').addEventListener('input', (e) => {
  const val = e.target.value;
  document.getElementById('colorVal').innerText = `Selected: ${val}`;
  document.body.style.backgroundColor = val + "22"; 
});
</script>
</body></html>

```

### 37. dom/06-creating-elements.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Creating Elements</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:22px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .btn { padding:10px 20px; background:#1e88e5; color:white; border:none; border-radius:6px; cursor:pointer; font-weight:700; }
  .msg-item { padding:10px; border-bottom:1px solid #eee; font-size:14px; animation: slideIn 0.3s ease; }
  @keyframes slideIn { from { opacity:0; transform:translateY(-10px); } to { opacity:1; transform:translateY(0); } }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>Adding to the DOM</h1><p>Generate HTML structure with JS</p></div>
<div class="card">
  <button class="btn" onclick="addMsg()">Add Message</button>
  <div id="list" style="margin-top:15px"></div>
</div>
<script>
function addMsg() {
  const p = document.createElement('div');
  p.className = "msg-item";
  p.innerText = "New Message Added at " + new Date().toLocaleTimeString();
  document.getElementById('list').prepend(p);
}
</script>
</body></html>

```

### 38. dom/07-innerhtml-vs-text.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — innerHTML</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:22px; box-shadow:0 2px 10px rgba(0,0,0,.07); }
  .target { padding:20px; background:#f5f5f5; border-radius:8px; margin-bottom:15px; }
  .btn { padding:10px 20px; background:#1e88e5; color:white; border:none; border-radius:6px; cursor:pointer; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>HTML Injection</h1><p>Modifying internal HTML structure</p></div>
<div class="card">
  <div id="target" class="target">This is plain text.</div>
  <button class="btn" onclick="inject()">Inject HTML Tags</button>
</div>
<script>
function inject() {
  document.getElementById('target').innerHTML = 
    `<h3 style="color:#e53935">Alert!</h3><p>This was injected via <b>innerHTML</b>.</p>`;
}
</script>
</body></html>

```

### 39. dom/08-timers.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Timers</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:40px; box-shadow:0 2px 10px rgba(0,0,0,.07); text-align:center; }
  #timer { font-size:64px; font-weight:800; margin-bottom:20px; color:#1a1a2e; }
  .btn { padding:12px 30px; background:#1e88e5; color:white; border:none; border-radius:6px; cursor:pointer; font-weight:700; }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>Timers</h1><p>Using setInterval for repetition</p></div>
<div class="card">
  <h1 id="timer">0</h1>
  <button class="btn" onclick="start()">Start Counter</button>
</div>
<script>
let count = 0;
let running = false;
function start() {
  if(running) return;
  running = true;
  setInterval(() => {
    count++;
    document.getElementById('timer').innerText = count;
  }, 1000);
}
</script>
</body></html>

```

### 40. dom/09-final-demo.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>DOM — Final Demo</title>
<style>
  *::before,*::after, * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: "Segoe UI", system-ui, sans-serif; background: #f0f2f5; padding: 24px; }
  .back { display:inline-block; margin-bottom:16px; padding:7px 16px; background:#fff; border-radius:8px; color:#3949ab; text-decoration:none; font-weight:700; font-size:13px; }
  .hdr { background:#1a1a2e; color:#fff; padding:24px 28px; border-radius:14px; margin-bottom:22px; border-left:6px solid #1e88e5; }
  .card { background:#fff; border-radius:12px; padding:40px; box-shadow:0 2px 10px rgba(0,0,0,.07); text-align:center; }
  #val { font-size:80px; font-weight:800; margin-bottom:20px; transition: 0.2s; }
  .btn { width:60px; height:60px; border-radius:50%; border:none; background:#1e88e5; color:white; font-size:24px; font-weight:700; cursor:pointer; margin:0 10px; box-shadow:0 4px 10px rgba(30,136,229,0.3); }
  .btn:active { transform: scale(0.9); }
</style>
</head>
<body>
<a href="../index.html" class="back">← Workshop Index</a>
<div class="hdr"><h1>Counter App</h1><p>The final combined concept demo</p></div>
<div class="card">
  <h1 id="val">0</h1>
  <button class="btn" onclick="change(-1)">−</button>
  <button class="btn" onclick="change(1)">+</button>
</div>
<script>
let v = 0;
function change(amt) {
  v += amt;
  const el = document.getElementById('val');
  el.innerText = v;
  el.style.color = v < 0 ? "#e53935" : (v > 0 ? "#43a047" : "#1a1a2e");
  el.style.transform = "scale(1.2)";
  setTimeout(() => el.style.transform = "scale(1)", 100);
}
</script>
</body></html>

```