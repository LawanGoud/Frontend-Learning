# 📦 **CSS Box Properties**

These control the physical size of HTML elements.

---

## ✅ 1. **Height**

Sets the vertical size of an element.

**Syntax:**

```css
selector {
  height: value;
}
```

**Units:** `px`, `%`, `vh`, `em`

**Example:**

```css
div {
  height: 200px;
}
```

---

## ✅ 2. **Width**

Sets the horizontal size of an element.

**Syntax:**

```css
selector {
  width: value;
}
```

**Example:**

```css
div {
  width: 100%;
}
```

**Note:** Using `%` makes the width relative to the parent element.

---

# 🖼️ **CSS Background Properties**

---

## ✅ 1. **Background Image**

Sets an image as the background of an element.

**Syntax:**

```css
selector {
  background-image: url("path/to/image.jpg");
}
```

**Example:**

```css
.hero {
  background-image: url("banner.jpg");
}
```

**Tip:** You can also combine it with `background-color`, `position`, `repeat`, and `size`.

---

## ✅ 2. **Background Size**

Controls the scaling of a background image.

**Values:**

- `auto`
- `cover` – Fills container, maintains aspect ratio
- `contain` – Fits entire image in container
- Exact values (e.g., `100px 200px`)

**Example:**

```css
.hero {
  background-size: cover;
}
```

---

# 📱 **Viewport Units**

Viewport units help create responsive designs based on the browser window size.

---

## ✅ 1. **Viewport Height (`vh`)**

**What It Is:**
1 `vh` = 1% of the viewport height.

**Example:**

```css
.section {
  height: 100vh; /* fills full screen height */
}
```

---

## ✅ 2. **Viewport Width (`vw`)**

**What It Is:**
1 `vw` = 1% of the viewport width.

**Example:**

```css
.container {
  width: 50vw; /* takes half the screen width */
}
```

---

## ✅ Summary Tip:

Use viewport units for fullscreen layouts, hero sections, and responsive scaling. Combine with media queries for best results.

---

# 📦 **CSS Border & Padding Properties**

These properties define the **edge appearance** of an element and the **space between its content and border**.

---

## ✅ **Border Width**

**What It Does:**
Sets how **thick** the border is.

**Syntax:**

```css
selector {
  border-width: value;
}
```

**Units:** `px`, `em`, `rem`

**Example:**

```css
.box {
  border-width: 2px;
}
```

**Note:** Usually used with `border-style` to make the border visible.

---

## ✅ **Border Radius**

**What It Does:**
Rounds the **corners** of an element.

**Syntax:**

```css
selector {
  border-radius: value;
}
```

**Example:**

```css
.card {
  border-radius: 10px;
}
```

**Creative Use:**
To make a circle:

```css
.circle {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
```

---

## ✅ **Border Color**

**What It Does:**
Sets the **color** of the border.

**Syntax:**

```css
selector {
  border-color: color;
}
```

**Example:**

```css
.alert {
  border-color: red;
}
```

**Pro Tip:** You can also use shorthand:

```css
border: 2px solid green;
```

---

## ✅ **Border Style**

**What It Does:**
Defines the **pattern** of the border line.

**Values:**

- `solid`
- `dashed`
- `dotted`
- `double`
- `none`

**Example:**

```css
div {
  border-style: dashed;
}
```

**Complete Border Example:**

```css
.card {
  border: 3px solid #007bff;
}
```

---

## ✅ **Padding**

**What It Does:**
Creates **space between the content and the border** of an element.

**Syntax:**

```css
selector {
  padding: value;
}
```

**Example:**

```css
.container {
  padding: 20px;
}
```

**Multiple Values:**

```css
padding: 10px 20px 30px 40px; /* top right bottom left */
```

**Shorthand Tips:**

- `padding: 10px;` → all sides
- `padding: 10px 20px;` → top/bottom, left/right

---

✅ **Next Suggested Topics:**

- `margin` (space **outside** the border)
- Full **box model visualization**
- `box-sizing: border-box;` behavior
- CSS shorthand: `border`, `padding`, `margin` combinations
