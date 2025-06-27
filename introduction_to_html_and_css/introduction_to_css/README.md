# 🎨 **Introduction to CSS**

CSS (Cascading Style Sheets) is used to style and layout web pages — for example, to change fonts, colors, spacing, and positioning.

---

## ✅ **HTML Elements**

Before applying CSS, it's important to understand how to identify the HTML elements you'll be styling.

### 🔹 **Container Element**

**What to Learn:**
A container is typically a `<div>` or `<section>` used to group other HTML elements. It doesn't have any visual style on its own but serves as a structural wrapper.

**Example:**

```html
<div class="container">
  <h1>Welcome</h1>
  <p>This content is inside a container.</p>
</div>
```

**Why It Matters:**
You often apply CSS to containers to style groups of content — setting widths, margins, padding, backgrounds, etc.

---

## ✅ **CSS Properties**

CSS is made of **rules** that target HTML elements using **selectors** and define **properties and values**.

### 🔹 **Syntax**

**Structure:**

```css
selector {
  property: value;
}
```

**Example:**

```css
p {
  color: blue;
  font-size: 16px;
}
```

**Explanation:**

* `p` is the selector (targets all `<p>` tags).
* `color` and `font-size` are properties.
* `blue` and `16px` are values.

You can write CSS:

* **Inline** (inside an HTML tag),
* **Internal** (in a `<style>` tag in `<head>`), or
* **External** (in a `.css` file).

---

### 🔹 **Text-Align**

**What to Learn:**
The `text-align` property controls horizontal alignment of text within an element.

**Values:**

* `left` (default)
* `right`
* `center`
* `justify`

**Example:**

```css
h1 {
  text-align: center;
}
```

**Effect:**

```html
<h1 style="text-align: center;">This Heading is Centered</h1>
```

**Pro Tip:**
Apply `text-align` to block-level elements (like `<div>`, `<p>`, `<h1>`) to affect child inline content.


---

# 🎨 **CSS Text Properties**

Text properties control how text appears on a webpage — including its color, size, spacing, and alignment.

---

### 🔹 **Color**

**What to Learn:**
The `color` property sets the **text color** of an element.

**Syntax:**

```css
selector {
  color: value;
}
```

**Common Values:**

* Color names: `red`, `blue`, `black`, etc.
* Hex codes: `#ff0000` (red), `#333333`
* RGB: `rgb(255, 0, 0)`
* HSL: `hsl(0, 100%, 50%)`

**Example:**

```css
h1 {
  color: darkblue;
}
```

**Result:**

```html
<h1 style="color: darkblue;">This heading is dark blue.</h1>
```

**Best Practice:**
Use hex or HSL for design precision; use named colors for simplicity.

---

# 🌈 **CSS Background Properties**

These properties let you set background colors, images, gradients, and more.

---

### 🔹 **Background Color**

**What to Learn:**
`background-color` sets the **background color** of an element.

**Syntax:**

```css
selector {
  background-color: value;
}
```

**Example:**

```css
div {
  background-color: #f0f0f0;
}
```

**HTML Preview:**

```html
<div style="background-color: #f0f0f0;">
  <p>This div has a light gray background.</p>
</div>
```

**Useful Tip:**
Combine with padding or margins to make background colors look cleaner:

```css
.container {
  background-color: lightblue;
  padding: 20px;
}
```

---

# ✍️ **CSS Font and Text Styling Properties**

---

## ✅ **Font Family**

**What to Learn:**
Sets the typeface of text.

**Syntax:**

```css
selector {
  font-family: "Font Name", fallback;
}
```

**Example:**

```css
body {
  font-family: "Arial", sans-serif;
}
```

**Tips:**

* Always include a **generic fallback**: `sans-serif`, `serif`, `monospace`.
* Use Google Fonts for web-safe and beautiful fonts.

**Example using Google Fonts:**

```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">

<style>
  body {
    font-family: 'Roboto', sans-serif;
  }
</style>
```

---

## ✅ **Font Size**

**What to Learn:**
Controls how big or small the text appears.

**Syntax:**

```css
selector {
  font-size: value;
}
```

**Units:**

* `px` (pixels): fixed size
* `em`, `rem`: scalable units
* `%`: relative to parent

**Example:**

```css
h1 {
  font-size: 32px;
}
p {
  font-size: 1rem;
}
```

---

## ✅ **Font Style**

**What to Learn:**
Defines **italicization** or **normal style**.

**Values:**

* `normal`
* `italic`
* `oblique`

**Example:**

```css
blockquote {
  font-style: italic;
}
```

---

## ✅ **Font Weight**

**What to Learn:**
Sets how **bold** the text is.

**Values:**

* `normal` (400)
* `bold` (700)
* `lighter`, `bolder`
* Numeric: `100` to `900`

**Example:**

```css
strong {
  font-weight: bold;
}
h1 {
  font-weight: 700;
}
```

---

## ✅ **Text Decoration**

**What to Learn:**
Adds or removes **lines** on text (underline, overline, etc.).

**Values:**

* `none`
* `underline`
* `overline`
* `line-through`

**Example:**

```css
a {
  text-decoration: none;
}
p.strike {
  text-decoration: line-through;
}
```

---
