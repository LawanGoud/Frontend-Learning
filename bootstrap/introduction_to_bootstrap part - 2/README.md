
# 📘 **Bootstrap Flexbox Utilities**

## ✅ **1. Flexbox Container**

**What to Learn:**
Bootstrap’s `d-flex` class turns an HTML element into a Flexbox Container.
The **direct children** of that container become **flex items**.

**Example:**

```html
<div class="d-flex">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

**Notes:**

* Only direct children of `.d-flex` are considered flex items.
* Nested elements like `<h1>`, `<p>`, and `<button>` are **not** flex items unless they are direct children.

---

## ✅ **2. Flex Direction**

**What to Learn:**
`flex-direction` defines the direction in which flex items are placed in the container.

| Class         | Direction            |
| ------------- | -------------------- |
| `flex-row`    | Horizontal (default) |
| `flex-column` | Vertical             |

---

### 🔹 **2.1 flex-row**

**Use:** Arrange items horizontally (left to right).

```html
<div class="d-flex flex-row">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

### 🔹 **2.2 flex-column**

**Use:** Arrange items vertically (top to bottom).

```html
<div class="d-flex flex-column">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

## ✅ **3. Justify Content**

**What to Learn:**
Controls the alignment of flex items **along the main axis** (which depends on the flex direction).

| Class                     | Alignment             |
| ------------------------- | --------------------- |
| `justify-content-start`   | Start (left or top)   |
| `justify-content-center`  | Center                |
| `justify-content-end`     | End (right or bottom) |
| `justify-content-between` | Space between items   |

---

### 🔹 **3.1 justify-content-start**

```html
<div class="d-flex flex-column justify-content-start">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

* With `flex-row`: items align to **left**
* With `flex-column`: items align to **top**

---

### 🔹 **3.2 justify-content-center**

```html
<div class="d-flex flex-column justify-content-center">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

* With `flex-row`: items align **horizontally center**
* With `flex-column`: items align **vertically center**

---

### 🔹 **3.3 justify-content-end**

```html
<div class="d-flex flex-column justify-content-end">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

* With `flex-row`: items align to **right**
* With `flex-column`: items align to **bottom**

---

### 🔹 **3.4 justify-content-between**

```html
<div class="d-flex flex-column justify-content-between box-container">
  <div class="box box-orange"><p>Box 1</p></div>
  <div class="box box-green"><p>Box 2</p></div>
</div>
```

**Result:** Equal space **between** flex items.

---

## ✅ **💡 Full Example: Flex Layout with Background**

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" />
  </head>
  <body>
    <div class="bg-container d-flex flex-column justify-content-end">
      <div class="tourism-card">
        <h1 class="main-heading">Tourism</h1>
        <p class="paragraph">Plan your trip.</p>
        <button class="button">Get Started</button>
      </div>
    </div>
  </body>
</html>
```

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

.bg-container {
  background-image: url("https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/ocean.jpg");
  height: 100vh;
  background-size: cover;
}

.tourism-card {
  text-align: center;
  background-color: white;
  padding: 5px;
  border-top-left-radius: 25px;
  border-top-right-radius: 25px;
}

.main-heading, .paragraph {
  font-family: "Roboto";
}

.button {
  color: white;
  background-color: #25b1cc;
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 20px;
}
```

---

## ✅ **Bonus Example: justify-content-between**

```html
<div class="d-flex flex-column justify-content-between box-container">
  <div class="box box-orange"><p>Box 1</p></div>
  <div class="box box-green"><p>Box 2</p></div>
</div>
```

```css
.box-container {
  width: 100vw;
  height: 100vh;
}

.box {
  width: 100px;
  height: 100px;
  color: white;
}

.box-orange {
  background-color: orange;
}

.box-green {
  background-color: green;
}
```

---
