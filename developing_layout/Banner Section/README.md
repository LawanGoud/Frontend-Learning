## 📌 1. Bootstrap Navbar (Without List-Based Approach)

This navbar uses Bootstrap 4.5.2 and avoids a traditional `<ul>` list. It provides a responsive menu with toggling behavior on smaller screens.

### ✅ Features:

- Logo image
- Navigation links
- Mobile toggle with hamburger icon

### ✅ Sample Code:

```html
<nav class="navbar navbar-expand-lg navbar-light bg-white">
  <div class="container">
    <a class="navbar-brand" href="#">
      <img
        src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/food-munch-img.png"
        class="food-munch-logo"
      />
    </a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNavAltMarkup"
      aria-controls="navbarNavAltMarkup"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav ml-auto">
        <a class="nav-link active" id="navItem1" href="#">Why Choose Us?</a>
        <a class="nav-link" id="navItem2" href="#">Explore Menu</a>
        <a class="nav-link" id="navItem3" href="#">Delivery & Payment</a>
        <a class="nav-link" id="navItem4" href="#">Follow Us</a>
      </div>
    </div>
  </div>
</nav>
```

---

## 📌 2. Bootstrap Containers

Bootstrap containers manage **horizontal spacing and layout width**.

### ✅ 2.1 `container`

A fixed-width responsive container with padding.

| Device Size      | Width ≥  | Max Width |
| ---------------- | -------- | --------- |
| Extra small (xs) | < 576px  | 100%      |
| Small (sm)       | ≥ 576px  | 540px     |
| Medium (md)      | ≥ 768px  | 720px     |
| Large (lg)       | ≥ 992px  | 960px     |
| Extra large (xl) | ≥ 1200px | 1140px    |

### ✅ 2.2 `container-fluid`

A full-width container that spans the entire width of the viewport.

### ✅ Sample Code:

```html
<!-- Fixed container -->
<div class="container">
  <div class="row">
    <div class="col-12">
      <h1>Taj Mahal</h1>
      <p>
        The Taj Mahal is an ivory-white marble mausoleum on the southern bank of
        the Yamuna in Agra.
      </p>
    </div>
  </div>
</div>

<!-- Fluid container -->
<div class="container-fluid">
  <div class="row">
    <div class="col-12">
      <h1>Taj Mahal</h1>
      <p>
        The Taj Mahal is an ivory-white marble mausoleum on the southern bank of
        the Yamuna in Agra.
      </p>
    </div>
  </div>
</div>
```

---

## 📌 3. CSS Colors

### ✅ 3.1 Transparent Background

To make a background fully transparent:

#### ✅ Custom CSS:

```css
.custom-outline-button {
  background-color: transparent;
}
```

#### ✅ Bootstrap Utility Class:

```html
<div class="bg-transparent">...</div>
```

---

## 📌 4. Banner Section Layout

This section uses Bootstrap classes and custom styles to create a visually appealing full-screen banner with centered text and buttons.

### ✅ HTML Structure:

```html
<div
  class="banner-section-bg-container d-flex justify-content-center flex-column"
>
  <div class="text-center">
    <h1 class="banner-heading mb-3">Get Delicious Food Anytime</h1>
    <p class="banner-caption mb-4">Eat Smart & Healthy</p>
    <button class="custom-button">View Menu</button>
    <button class="custom-outline-button">Order Now</button>
  </div>
</div>
```

---

## 📌 5. Custom CSS

```css
.food-munch-logo {
  width: 80px;
  height: 70px;
}

#navItem1,
#navItem2,
#navItem3,
#navItem4 {
  color: #323f4b;
  font-family: "Roboto";
}

.banner-section-bg-container {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/foodmunch-banner-bg.png");
  height: 100vh;
  background-size: cover;
}

.banner-heading {
  color: white;
  font-family: "Roboto";
  font-size: 45px;
  font-weight: 300;
}

.banner-caption {
  color: #f5f7fa;
  font-family: "Roboto";
  font-size: 24px;
  font-weight: 300;
}

.custom-button {
  color: white;
  background-color: #d0b200;
  width: 130px;
  height: 45px;
  border: none;
  border-radius: 8px;
  margin-right: 10px;
}

.custom-outline-button {
  color: #d0b200;
  background-color: transparent;
  width: 130px;
  height: 45px;
  border: 1px solid #d0b200;
  border-radius: 8px;
}
```

---

## ✅ Corrections Made:

- Fixed inline style consistency.
- Ensured all `nav-link` elements have unique IDs.
- Used `ml-auto` on `.navbar-nav` for proper right alignment.
- Ensured CSS uses consistent formatting and correct font names.

---

## 📚 Additional Tips

- Use **Bootstrap spacing utilities** (`mb-3`, `ml-auto`) for margin and layout control.
- Keep button styles reusable by using custom classes (`.custom-button`, `.custom-outline-button`).
- Prefer `container` for centered content, `container-fluid` for full-width layout.
- Avoid using inline styles unless necessary; use classes instead.

---
