## 🟩 **Assignment: Food Munch Navbar**

**Difficulty:** Easy
**Status:** ✅ Solved

---

### ✅ **Objective:**

Create a **responsive dark-themed navbar** for the **Food Munch** website using **Bootstrap** classes and concepts such as:

* Responsive Navbar
* Collapsible Hamburger Menu
* Bootstrap color utilities
* Navbar alignment using `ml-auto`

---

### 📱 **Responsive Behavior Requirements:**

Ensure your Navbar looks correct across all breakpoints:

* **Extra Small (< 576px)**
* **Small (≥ 576px)**
* **Medium (≥ 768px)**

> Use a collapsible menu (hamburger style)

* **Large (≥ 992px)**
* **Extra Large (≥ 1200px)**

> Show all navigation items horizontally

---

### 🎨 **Design Requirements:**

* Replace `navbar-light` with `navbar-dark` to ensure the toggler icon is visible on a dark background.
* Use Bootstrap’s background utility classes like `bg-dark` for the navbar background.
* Add the provided **Food Munch Logo**.
* Align nav links to the right using `ml-auto`.

---

### 📦 **Resources:**

* **Food Munch Logo URL:**
  `https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/food-munch-logo-img.png`

---

### ✅ **HTML Starter Template:**

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="#">
    <img
      src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/food-munch-logo-img.png"
      class="d-inline-block align-top"
      alt="Food Munch Logo"
      height="30"
    />
  </a>
  <button
    class="navbar-toggler"
    type="button"
    data-toggle="collapse"
    data-target="#navbarNav"
    aria-controls="navbarNav"
    aria-expanded="false"
    aria-label="Toggle navigation"
  >
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarNav">
    <div class="navbar-nav ml-auto">
      <a class="nav-link active" href="#">Home</a>
      <a class="nav-link" href="#">Menu</a>
      <a class="nav-link" href="#">Delivery</a>
      <a class="nav-link" href="#">Contact</a>
    </div>
  </div>
</nav>
```

---

### 📘 **Instructions:**

1. Add this within a complete HTML boilerplate with Bootstrap CSS/JS linked.
2. Use Bootstrap 4 or 5.
3. Make sure the navbar collapses properly on smaller screens.
4. Test the layout across screen sizes using browser DevTools.

---

### ✅ **Tips:**

* Add padding or margin using Bootstrap utilities (e.g., `p-2`, `mb-3`) if needed.
* Always check responsiveness using the device toolbar in your browser.
* If you're using Bootstrap 5, replace `data-toggle`/`data-target` with `data-bs-toggle`/`data-bs-target`.

---

