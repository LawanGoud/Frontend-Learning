# 📘 CSS Selectors & Core Concepts

This guide provides an overview of fundamental **CSS selectors** and **core styling concepts** such as **inheritance**, **specificity**, and **the cascade**. Examples are included to support each explanation.

---

## 🔹 1. CSS Selectors

CSS selectors are used to "select" the HTML elements you want to style.

### 📌 1.1 Simple Selectors

---

#### ✅ Class Selector

- **Syntax**: `.class-name`
- Selects all elements with the specified class.

```html
<p class="paragraph">The population of India is around 138 crores.</p>
```

```css
.paragraph {
  color: blue;
}
```

> Multiple elements can share the same class:

```html
<h1 class="heading">About India</h1>
<p class="paragraph">The population of India is around 138 crores.</p>
<p class="paragraph">There are 28 states in India.</p>
```

```css
.heading {
  color: orange;
  font-size: 28px;
  font-weight: 600;
}
```

---

#### ✅ ID Selector

- **Syntax**: `#id-name`
- Selects a **single** element with a specific ID (should be unique in the document).

```html
<p id="populationParagraph">The population of India is around 138 crores.</p>
```

```css
#populationParagraph {
  color: blue;
}
```

> Example with multiple IDs:

```html
<h1 id="countryHeading">About India</h1>
<p id="populationParagraph">The population of India is around 138 crores.</p>
<p id="statesParagraph">There are 28 states in India.</p>
```

```css
#countryHeading {
  color: orange;
  font-size: 28px;
  font-weight: 600;
}
#populationParagraph {
  color: blue;
}
#statesParagraph {
  color: green;
}
```

---

#### ✅ Type (Tag Name) Selector

- **Syntax**: Uses an HTML tag name (e.g., `p`, `h1`, `div`)
- Selects **all** elements of that tag.

```html
<h1>About India</h1>
<p>The population of India is around 138 crores.</p>
<p>There are 28 states in India.</p>
```

```css
h1 {
  color: orange;
  font-size: 28px;
  font-weight: 600;
}
p {
  color: blue;
}
```

---

## 🔹 2. Core CSS Concepts

CSS styling is governed by three fundamental principles:

- **Inheritance**
- **Specificity**
- **Cascade**

---

### 📘 2.1 Inheritance

Inheritance allows child elements to take on styles from their parent elements — but only for **inheritable** properties.

#### 🧩 Parent & Child Elements

```html
<div>
  <h1>The seven wonders of the world</h1>
  <p>
    The <a href="https://en.wikipedia.org/wiki/Taj_Mahal">Taj Mahal</a> is one
    of the seven wonders of the world.
  </p>
</div>
```

- `div` is the parent of `h1` and `p`
- `p` is the parent of `a`

---

### ✅ 2.1.3 Inherited Properties

These properties **do** get inherited from parent to child:

#### 🔤 Text-related Properties:

- `font-family`
- `font-style`
- `font-weight`
- `text-align`
- `color`

#### 📋 List-related Properties:

- `list-style-type`

---

### ❌ 2.1.4 Non-inherited Properties

These properties **do not** get inherited automatically:

#### 📦 Box-related Properties:

- `width`
- `height`
- `margin`
- `padding`
- `border-style`
- `border-width`
- `border-color`
- `border-radius`

#### 🎨 Background-related Properties:

- `background-color`
- `background-image`
- `background-size`

#### ✂️ Other:

- `text-decoration`

---

### ✅ Example: Inheritance in Action

```html
<div class="country-container">
  <h1>About India</h1>
  <p>The population of India is around 138 crores.</p>
  <p>There are 28 states in India.</p>
</div>
```

```css
.country-container {
  text-align: center;
  color: blue;
  border-style: solid;
  border-width: 3px;
  border-color: orange;
}
```

> `text-align` and `color` will be inherited by the `h1` and `p` tags.
> But `border-style` and other box-related properties will only apply to `.country-container`.

---

## ✅ Summary Tables

### 📌 Selector Types

| Selector   | Syntax       | Description                            |
| ---------- | ------------ | -------------------------------------- |
| Class      | `.classname` | Targets all elements with that class   |
| ID         | `#idname`    | Targets one unique element by ID       |
| Type (Tag) | `p`, `h1`    | Targets all elements of a specific tag |

---

### 📌 Core CSS Concepts

| Concept     | Description                                                 |
| ----------- | ----------------------------------------------------------- |
| Inheritance | Child elements inherit certain properties from parents      |
| Specificity | Determines which style wins when multiple rules apply       |
| Cascade     | Rules are applied in order based on importance and location |

---

## 🧠 Tips for Writing Clean CSS

- Use **class selectors** for shared/reusable styles.
- Use **ID selectors** only for unique components (e.g., `#navbar`, `#footer`).
- Rely on **inheritance** for managing consistent styles (e.g., text alignment, color).
- Always structure selectors based on how HTML is nested.

> 💡 **Practice Tip**: Try combining selectors like `.container p` to apply styles only to paragraphs inside a container.

---

# 🎯 CSS Specificity, Inline Styles & Cascade

This section explains how CSS decides **which styles to apply** when multiple rules target the same element. Key concepts include **specificity**, **inline styles**, **the cascade**, and `!important`.

---

## 🔹 1. Specificity

**Specificity** determines which CSS rules are applied when multiple rules target the same element.

> The higher the specificity, the more “weight” the rule carries.

### 🔢 Specificity Order (Low ➡ High):

1. **Type (Tag Name) Selector**
2. **Class Selector**
3. **ID Selector**

---

### 📌 1.1 Type Selector vs. Class Selector

A **class selector** is more specific than a **type selector**.

#### ✅ Example:

```html
<body>
  <h1>Heading 1</h1>
  <h1>Heading 2</h1>
  <h1 class="heading">Heading 3</h1>
  <h1 class="heading">Heading 4</h1>
  <h1 class="heading">Heading 5</h1>
</body>
```

```css
h1 {
  color: grey;
  font-family: "Roboto";
  font-size: 22px;
}

.heading {
  color: blue;
  font-weight: bold;
}
```

> Only shared properties (like `color`) get overridden by the more specific selector.

---

### 📌 1.2 Class Selector vs. ID Selector

An **ID selector** is more specific than a **class selector**, and should be used only for unique elements.

#### ✅ Example:

```html
<body>
  <h1>Heading 1</h1>
  <h1>Heading 2</h1>
  <h1 class="heading">Heading 3</h1>
  <h1 class="heading">Heading 4</h1>
  <h1 class="heading">Heading 5</h1>
  <h1 class="heading" id="heading5">Heading 5</h1>
</body>
```

```css
h1 {
  color: grey;
  font-family: "Roboto";
  font-size: 22px;
}

.heading {
  color: blue;
  font-weight: bold;
}

#heading5 {
  color: green;
  font-size: 28px;
  font-style: italic;
}
```

---

## 🔹 2. Inline Styles

**Inline styles** are written directly inside an HTML tag using the `style` attribute.

### 🧾 Syntax:

```html
<tag style="property1: value1; property2: value2;">Content</tag>
```

#### ✅ Example:

```html
<body>
  <h1
    class="heading"
    id="heading5"
    style="color: white; background-color: orange;"
  >
    Heading 5
  </h1>
</body>
```

```css
h1 {
  color: grey;
  font-family: "Roboto";
  font-size: 22px;
}

.heading {
  color: blue;
  font-weight: bold;
}

#heading5 {
  color: green;
  font-size: 28px;
  font-style: italic;
}
```

> ✅ **Note**: Inline styles have the **highest specificity** and override all other selectors, unless a `!important` rule is applied.

---

### ⚠️ Avoid Inline Styles

- ❌ Not reusable
- ❌ Reduces readability
- ✅ Keep CSS separate from HTML for maintainable code

---

## 🔹 3. CSS Cascade

When two rules have the **same specificity**, the **one that appears last** wins.

#### ✅ Example:

```html
<h1 class="style-2 style-1">About India</h1>
```

```css
.style-1 {
  color: green;
}

.style-2 {
  color: blue;
}
```

> ✅ Even though `.style-1` is listed **first** in the HTML, `.style-2` wins because it appears **later** in the CSS.

---

### ⚠️ Class Order in HTML Doesn’t Matter

Only the **order in the CSS file** matters — **not** the order of class names in the `class` attribute.

---

## 🔹 3.1 The `!important` Rule

The `!important` flag forces a style to take precedence **regardless** of specificity or order.

#### ✅ Example:

```html
<h1 class="style-1">About India</h1>
```

```css
.style-1 {
  color: green;
}

h1 {
  color: orange !important;
}
```

> ✅ The `h1` rule wins due to `!important`.

---

### 🔁 Overriding `!important`

To override a style marked `!important`, the new rule must:

- Also use `!important`, and
- Either appear **after** it, or have **higher specificity**

#### ✅ Example:

```html
<h1 class="style-2 style-1">About India</h1>
```

```css
.style-1 {
  color: green !important;
}

h1 {
  color: orange !important;
}

.style-2 {
  color: blue !important;
}
```

> 🔄 Final applied color: **blue**, from `.style-2` (last and `!important`)

---

### ⚠️ Use `!important` Sparingly

Only use `!important` when necessary:

- ✅ To override styles from external libraries (e.g., Bootstrap)
- ❌ Avoid for your own CSS — use proper specificity instead

---
