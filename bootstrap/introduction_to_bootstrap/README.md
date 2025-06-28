# 📘 **CSS & Bootstrap Basics**

## ✅ **1. Reusability of CSS Rulesets**

**What to Learn:**
Reuse CSS classes across multiple elements to keep styles consistent and code DRY (Don't Repeat Yourself).

**CSS Example:**

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}
```

**HTML Example:**

```html
<button class="button">Get Started</button>
<button class="button">Visit Now</button>
```

**Tip:** Apply the same class to multiple elements to maintain uniform styles.

---

## ✅ **2. Multiple Class Names in HTML**

**What to Learn:**
An element can use multiple CSS classes by separating them with spaces.

**Syntax:**

```html
<tag class="name1 name2 name3">Content</tag>
```

**Example:**

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}

.button-green {
  background-color: #8cc63f;
}
```

```html
<button class="button button-green">Get Started</button>
```

**Tip:** Use utility classes to compose flexible styling.

---

## ✅ **3. Introduction to Bootstrap**

**What to Learn:**
Bootstrap is a framework with prewritten HTML, CSS, and JS components for fast web development.

---

### 🔹 **3.1 How to Add Bootstrap (CDN)**

**Include this in `<head>`:**

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" />
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
```

---

### 🔹 **3.2 Bootstrap Buttons**

**What to Learn:**
Use Bootstrap’s `btn` classes to style buttons quickly.

**Example:**

```html
<button class="btn btn-primary">Get Started</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Delete</button>
```

**Outline Buttons:**

```html
<button class="btn btn-outline-primary">Primary</button>
<button class="btn btn-outline-danger">Danger</button>
```

---

### 🔹 **3.3 Bootstrap Text Colors**

**What to Learn:**
Use text utility classes like `text-primary`, `text-success`, etc.

**Example:**

```html
<p class="text-success">Success Message</p>
<p class="text-danger">Error Message</p>
```

---

### 🔹 **3.4 Text Transformation in Bootstrap**

**What to Learn:**
Apply case transformations using utility classes.

**Example:**

```html
<p class="text-uppercase">This will be uppercase</p>
<p class="text-capitalize">this will be Capitalized</p>
<p class="text-lowercase">THIS WILL BE lowercase</p>
```

---

### 🔹 **3.5 Background Color Classes**

**What to Learn:**
Bootstrap provides `bg-*` classes for background colors.

**Example:**

```html
<div class="bg-info text-white">Info Box</div>
<div class="bg-warning text-dark">Warning Box</div>
```

---

### ⚠️ **Important: Don’t Override Bootstrap Class Names Directly**

**❌ Avoid:**

```css
.btn {
  background-color: blue;
}
```

**✅ Instead:**

```css
.button-custom {
  background-color: blue;
  color: white;
}
```

```html
<button class="btn button-custom">Custom Button</button>
```

---

