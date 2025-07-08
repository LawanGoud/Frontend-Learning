
## 🟩 **Assignment: Responsive Color Palette**

**Difficulty:** Easy
**Status:** ✅ Solved

---

### ✅ **Objective:**

Build a **Responsive Color Palette** using **Bootstrap's Grid System**, **Spacing Utilities**, and **Background Color Utilities** to support **five responsive breakpoints**:

* Extra Small (`< 576px`)
* Small (`≥ 576px`)
* Medium (`≥ 768px`)
* Large (`≥ 992px`)
* Extra Large (`≥ 1200px`)

Your layout should adapt correctly across all screen sizes, maintaining consistent spacing and structure.

---

### 🛠️ **Requirements:**

* Use Bootstrap 4 or 5.
* Use Bootstrap classes like `col-`, `col-sm-`, `col-md-`, `col-lg-`, `col-xl-`.
* Each color box must contain:

  * A background color class (e.g. `bg-primary`)
  * Padding using Bootstrap spacing (e.g. `p-2`)
  * A text label with white color
* Use responsive column widths to adjust layout across screen sizes.

---

### 💡 **Design Reference:**

Use the following colors as sample blocks:

```html
bg-primary, bg-secondary, bg-success, bg-info, bg-warning, bg-danger
```

---

### ⚠️ **Warning:**

> ❌ Avoid placing `.col-*` elements directly outside of a `.row`.
> ✅ Always nest columns within a `.row`.

---

### ✅ **Correct HTML Structure Example:**

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4 col-xl-3 mb-3">
      <div class="color-box bg-primary p-2">
        <p class="color-name text-white">Primary</p>
      </div>
    </div>
    <!-- Repeat for other color boxes -->
  </div>
</div>
```

---

### ✅ **CSS:**

```css
.color-box {
  padding: 10px;
}
.color-name {
  font-size: 20px;
  color: white;
}
```

---

### ✅ **Bonus Tips:**

* Use `mb-3` for vertical spacing between rows in smaller screens.
* Use `text-center` if you want to center the color labels.
* Use `container` class to ensure proper alignment and padding.

---

