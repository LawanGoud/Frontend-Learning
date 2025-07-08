# 📐 Bootstrap Grid System

Bootstrap Grid System is a collection of reusable code snippets to create **responsive layouts**. It is made up of:

- **Containers**
- **Rows**
- **Columns**

Bootstrap uses a **12-column system** for layout. You can create up to 12 columns across the page.

---

## 🔳 1. Container

The purpose of a **container** is to hold **rows and columns**.

```html
<div class="container"></div>
````

Here, the container is a `div` element with the Bootstrap class `container`.

---

## 📏 1.1 Row

The purpose of a **row** is to wrap all the **columns**.

```html
<div class="container">
  <div class="row"></div>
</div>
```

Here, the row is a `div` element with the Bootstrap class `row`.

---

## 📦 1.2 Column

Columns must be placed **inside a row**, and the **content goes inside the column**.

You can specify how many columns your content should span (from **1 to 12**):

```html
<div class="container">
  <div class="row">
    <div class="col-12">
      I'm your content inside the grid!
    </div>
  </div>
</div>
```

* `col-12` occupies the **entire width** of the row.
* `col-*` indicates how many columns to span out of 12.

🔹 **Example:**

```html
<div class="container">
  <div class="row">
    <div class="col-12">
      <h1 class="heading">Taj Mahal</h1>
      <p>
        The Taj Mahal is an ivory-white marble mausoleum on the southern
        bank of the river Yamuna in the Indian city of Agra.
      </p>
    </div>
  </div>
</div>
```

---

## 🧱 2. Creating Multiple Column Layouts

Below is a **two-column layout** example using `col-8` and `col-4`. You can also try:

* One column layout (`col-12`)
* Three column layout (`col-4`, `col-4`, `col-4`)
* And more combinations that add up to 12

🔹 **Example:**

```html
<div class="container">
  <div class="row">
    <div class="col-8">
      <h1 class="heading">Taj Mahal</h1>
      <p>
        The Taj Mahal is an ivory-white marble mausoleum on the southern
        bank of the river Yamuna in the Indian city of Agra.
      </p>
    </div>
    <div class="col-4">
      <h1 class="heading">Mysore Palace</h1>
      <p>
        The Mysore Palace is a historical palace and the royal residence at
        Mysore in the Indian State of Karnataka.
      </p>
    </div>
  </div>
</div>
```

---

> ✅ Remember: The total of column widths in a row should not exceed 12.


---

# 🧱 Bootstrap Grid System Guide

Bootstrap Grid System helps in creating **responsive layouts** with reusable code. It is based on a **12-column system** using containers, rows, and columns.

---

## 🔳 1. Container, Row & Column

### ✅ 1.1 Container

```html
<div class="container"></div>
````

The `.container` class is used to wrap the grid layout.

---

### ✅ 1.2 Row

```html
<div class="container">
  <div class="row"></div>
</div>
```

`.row` is used to wrap all columns.

---

### ✅ 1.3 Column

```html
<div class="container">
  <div class="row">
    <div class="col-12">
      I'm your content inside the grid!
    </div>
  </div>
</div>
```

* `col-12` means the column takes the full 12-column width.
* You can use any `col-*` (e.g., `col-6`, `col-4`, etc.) to specify width out of 12.

---

## 🧩 2. Creating Multiple Column Layouts

### ➕ Two Column Layout

```html
<div class="container">
  <div class="row">
    <div class="col-8">
      <h1 class="heading">Taj Mahal</h1>
      <p>The Taj Mahal is an ivory-white marble mausoleum...</p>
    </div>
    <div class="col-4">
      <h1 class="heading">Mysore Palace</h1>
      <p>The Mysore Palace is a historical palace...</p>
    </div>
  </div>
</div>
```

---

## 🔁 3. Column Wrapping

When more than 12 columns are added in one row, the extra columns **wrap to the next line**.

```html
<div class="container">
  <div class="row">
    <div class="col-6">
      <h1 class="heading">Taj Mahal</h1>
      <p>The Taj Mahal is on the southern bank of the river Yamuna.</p>
    </div>
    <div class="col-6">
      <h1 class="heading">Mysore Palace</h1>
      <p>The Mysore Palace is a historical palace and royal residence.</p>
    </div>
    <div class="col-6">
      <h1 class="heading">Golden Temple</h1>
      <p>The Golden Temple is located in the city of Amritsar.</p>
    </div>
    <div class="col-6">
      <h1 class="heading">Varanasi</h1>
      <p>Varanasi is a city located on the bank of the Ganges in UP.</p>
    </div>
  </div>
</div>
```

You can try combinations like:

* `col-4`, `col-4`, `col-6`
* `col-6`, `col-4`, `col-6`, `col-4`

---

## 📱 4. Responsive Breakpoints

Bootstrap has **five responsive breakpoints** with class name prefixes:

| Device           | Width     | Class Prefix |
| ---------------- | --------- | ------------ |
| Extra small (XS) | `<576px`  | `col-`       |
| Small (SM)       | `≥576px`  | `col-sm-`    |
| Medium (MD)      | `≥768px`  | `col-md-`    |
| Large (LG)       | `≥992px`  | `col-lg-`    |
| Extra large (XL) | `≥1200px` | `col-xl-`    |

🟡 **Note**: Behavior defined for a smaller device carries over to larger ones.

---

### 🔀 4.1 Combination of Class Names

You can combine different class names for different screen sizes.

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-lg-6">
      <h1 class="heading">Taj Mahal</h1>
      <p>The Taj Mahal is on the southern bank of the Yamuna.</p>
    </div>
    <div class="col-12 col-lg-6">
      <h1 class="heading">Mysore Palace</h1>
      <p>The Mysore Palace is a royal residence in Karnataka.</p>
    </div>
    <div class="col-12 col-lg-6">
      <h1 class="heading">Golden Temple</h1>
      <p>The Golden Temple is a gurdwara in Amritsar.</p>
    </div>
    <div class="col-12 col-lg-6">
      <h1 class="heading">Varanasi</h1>
      <p>Varanasi is a city on the Ganges in Uttar Pradesh.</p>
    </div>
  </div>
</div>
```

---

## 📌 Final Notes

* ✅ Bootstrap follows a **Mobile First Approach**.
* Start designing for small screens first, and scale up for larger ones.
* The grid automatically adapts to different device sizes.

---



# 🎨 Bootstrap Layout, Spacing, and Color Utilities

This guide covers **CSS box properties**, **Bootstrap spacing utilities**, **background colors**, and **responsive layout design** using Bootstrap 5.

---

## 📦 1. CSS Box Properties

### 🔸 1.1 Margin

The `margin` property adds space **outside** an element.

```css
.box {
  padding: 30px;
  margin-bottom: 10px;
}
.orange-box {
  background-color: orange;
}
.green-box {
  background-color: green;
}
````

### ➕ Margin Variants

* `margin-top`
* `margin-right`
* `margin-bottom`
* `margin-left`

**HTML Example:**

```html
<body>
  <div class="box orange-box"></div>
  <div class="box green-box"></div>
</body>
```

---

## 🔧 2. Bootstrap Spacing Utilities

### 📏 2.1 Margin Utilities

| CSS Property    | Bootstrap Class |
| --------------- | --------------- |
| `margin`        | `m-*`           |
| `margin-top`    | `mt-*`          |
| `margin-right`  | `mr-*`          |
| `margin-bottom` | `mb-*`          |
| `margin-left`   | `ml-*`          |

### 🔢 2.1.1 Margin Values

| Size | Value (in px)          |
| ---- | ---------------------- |
| 0    | 0                      |
| 1    | 0.25 \* 16px = **4px** |
| 2    | 0.5 \* 16px = **8px**  |
| 3    | 1 \* 16px = **16px**   |
| 4    | 1.5 \* 16px = **24px** |
| 5    | 3 \* 16px = **48px**   |

🚫 **Avoid** using `margin-left` and `margin-right` CSS on grid columns—it may break layout structure.

---

### 📐 2.2 Padding Utilities

| CSS Property     | Bootstrap Class |
| ---------------- | --------------- |
| `padding`        | `p-*`           |
| `padding-top`    | `pt-*`          |
| `padding-right`  | `pr-*`          |
| `padding-bottom` | `pb-*`          |
| `padding-left`   | `pl-*`          |

### 🔢 2.2.1 Padding Values

| Size | Value (in px)          |
| ---- | ---------------------- |
| 0    | 0                      |
| 1    | 0.25 \* 16px = **4px** |
| 2    | 0.5 \* 16px = **8px**  |
| 3    | 1 \* 16px = **16px**   |
| 4    | 1.5 \* 16px = **24px** |
| 5    | 3 \* 16px = **48px**   |

---

## 🎨 3. Bootstrap Background Color Utilities

**HTML Example:**

```html
<body>
  <div class="bg-primary p-2"><p>Primary</p></div>
  <div class="bg-secondary p-2"><p>Secondary</p></div>
  <div class="bg-success p-2"><p>Success</p></div>
  <div class="bg-info p-2"><p>Info</p></div>
  <div class="bg-warning p-2"><p>Warning</p></div>
  <div class="bg-light p-2"><p>Light</p></div>
  <div class="bg-dark p-2"><p>Dark</p></div>
  <div class="bg-white p-2"><p>White</p></div>
  <div class="bg-danger p-2"><p>Danger</p></div>
</body>
```

---

## 🧱 4. Developing Layouts for Five Responsive Breakpoints

Bootstrap uses **responsive breakpoints** to create layouts for various devices.

### 📊 4.1 Color Palette Grid Layout

```html
<body>
  <h1 class="color-palette-heading">Color Palette</h1>
  <div class="container">
    <div class="row">
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-primary"><p class="color-name">Primary</p></div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-secondary"><p class="color-name">Secondary</p></div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-success"><p class="color-name">Success</p></div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-info"><p class="color-name">Info</p></div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-warning"><p class="color-name">Warning</p></div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
        <div class="color-box bg-danger"><p class="color-name">Danger</p></div>
      </div>
    </div>
  </div>
</body>
```

### 🖌️ CSS Styles:

```css
.color-palette-heading {
  font-size: 24px;
  text-align: center;
}
.color-box {
  padding: 10px;
}
.color-name {
  color: white;
  font-size: 20px;
}
```

---

## 🔚 Summary

* Use **Bootstrap utilities** like `m-*`, `p-*`, `bg-*` for layout, spacing, and color.
* Rely on **responsive breakpoints** (`col-md-*`, `col-lg-*`, etc.) to create mobile-first layouts.
* Stick to Bootstrap classes over manual CSS for cleaner, more reliable design systems.

---



## ✅ 1. **Bootstrap Navbar**

### 1.1 Basic Structure

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light"></nav>
```

* `navbar-expand-lg`: Navbar expands on large screens.
* `navbar-light bg-light`: Light theme with light background.

### 1.2 Nav Items

```html
<a class="nav-link active" href="#">Home</a>
<a class="nav-link" href="#">Features</a>
<a class="nav-link" href="#">Pricing</a>
<a class="nav-link disabled" href="#" aria-disabled="true">Disabled</a>
```

### 1.3 Complete Example (Non-list based)

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" ...>
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav">
      <a class="nav-link active" href="#">Home</a>
      <a class="nav-link" href="#">Features</a>
      <a class="nav-link" href="#">Pricing</a>
      <a class="nav-link disabled" href="#">Disabled</a>
    </div>
  </div>
</nav>
```

---

## ✅ 2. **HTML Elements**

### 2.1 Block-level

* Start on new line.
* Fill the entire width.
* Examples: `h1`, `p`, `div`.

```html
<h1 class="heading">Title</h1>
<p class="paragraph">Text here.</p>
```

### 2.2 Inline Elements

* Only take up the space they need.
* Examples: `a`, `img`, `button`.

```html
<p class="paragraph">
  Visit the <a class="link-text" href="#">Taj Mahal</a>.
</p>
```

---

## ✅ 3. **CSS Box Properties**

### 3.1 `margin: auto`

* Centers a block-level element horizontally.

```css
.nav-items-center {
  margin: auto;
}
```

### 3.2 Margin Variants

```css
.nav-items-right {
  margin-left: auto;  /* Aligns items to the right */
}
```

---

## ✅ 4. **Bootstrap Utilities**

### 4.1 Margin Classes

| CSS Property        | Bootstrap Class   |
| ------------------- | ----------------- |
| `margin`            | `m-*`             |
| `margin-top`        | `mt-*`            |
| `margin-left`       | `ml-*`            |
| `margin-right`      | `mr-*`            |
| `m-auto`, `ml-auto` | Auto margin utils |

### Example:

```html
<div class="navbar-nav ml-auto">
  <a class="nav-link" href="#">Home</a>
</div>
```

---

## ✅ 5. **Final Navbar with Logo and Responsive Collapse**

```html
<nav class="navbar navbar-expand-lg navbar-light bg-white">
  <a class="navbar-brand" href="#">
    <img src="logo.png" class="navbar-image" alt="Logo" />
  </a>
  <button class="navbar-toggler" type="button" data-toggle="collapse"
    data-target="#navbarNavAltMarkup">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav ml-auto">
      <a class="nav-link active" href="#">Home</a>
      <a class="nav-link" href="#">About Me</a>
      <a class="nav-link" href="#">Projects</a>
      <a class="nav-link" href="#">Testimonials</a>
    </div>
  </div>
</nav>
```

---

