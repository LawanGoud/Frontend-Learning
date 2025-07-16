# ✅ VR Website Navbar & Banner Section

## 🔍 Problem Statement

Create a **responsive Navbar and Banner Section** for a **VR website** using **Bootstrap 4.5.2**, custom CSS, and media responsiveness principles.

---

## 🖼️ Reference Design

The design should work and look good on:

- Extra Small devices (`<576px`)
- Small devices (`≥576px`)
- Medium devices (`≥768px`)
- Large and Extra Large devices (`≥992px`, `≥1200px`)

---

## 🧰 Resources Provided

| Element          | Resource URL                                                                                                                                                     |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| VR Logo          | [https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-logo-img.png](https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-logo-img.png)   |
| Background Image | [https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-banner-bg.png](https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-banner-bg.png) |

### 🎨 Colors Used

- Primary Text Color: `#323f4b`
- Banner Background Overlay: `#1a2137`

---

## 🧱 Step-by-Step Implementation

---

### ✅ Step 1: HTML Boilerplate + Bootstrap CDN

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>VR Website</title>
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
    />
    <link
      href="https://fonts.googleapis.com/css2?family=Roboto&display=swap"
      rel="stylesheet"
    />
    <style>
      /* Add custom CSS here */
    </style>
  </head>
  <body>
    <!-- Code goes here -->
  </body>
</html>
```

---

### ✅ Step 2: Navbar Implementation

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-transparent">
  <div class="container">
    <a class="navbar-brand" href="#">
      <img
        src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-logo-img.png"
        class="vr-logo"
        alt="VR Logo"
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
      <div class="ml-auto d-flex flex-column flex-lg-row">
        <a class="nav-link text-white" href="#">Home</a>
        <a class="nav-link text-white" href="#">Products</a>
        <a class="nav-link text-white" href="#">Recent Blogs</a>
        <a class="nav-link text-white" href="#">Contact Us</a>
      </div>
    </div>
  </div>
</nav>
```

---

### ✅ Step 3: Banner Section Layout

```html
<section
  class="banner-section d-flex justify-content-center align-items-center"
>
  <div class="text-center">
    <h1 class="banner-heading">The Revolution in Virtual Reality</h1>
    <button class="btn custom-button mt-4">View More</button>
  </div>
</section>
```

---

### ✅ Step 4: Custom CSS Styling

```css
body {
  font-family: "Roboto", sans-serif;
}

.vr-logo {
  width: 60px;
}

.banner-section {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-banner-bg.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
  color: white;
  position: relative;
}

.banner-heading {
  font-size: 36px;
  font-weight: bold;
  max-width: 600px;
  margin: 0 auto;
}

.custom-button {
  background-color: white;
  color: #1a2137;
  padding: 10px 20px;
  border-radius: 5px;
  font-weight: bold;
  border: none;
}

.nav-link {
  font-size: 16px;
  padding: 8px 16px;
}
```

---

## ✅ Final Checklist

| Feature                      | Implemented |
| ---------------------------- | ----------- |
| Bootstrap 4.5.2 used         | ✅          |
| Responsive Navbar            | ✅          |
| Logo on the left             | ✅          |
| Links on right for large     | ✅          |
| Hamburger menu for small     | ✅          |
| Banner with background image | ✅          |
| Heading + CTA button         | ✅          |
| Font & colors matched        | ✅          |

---

## 🎯 Output Expectations

✅ Should work across all devices
✅ Consistent alignment and spacing
✅ Typography and button styling should match
✅ Use of `container`, `navbar`, and utility classes from Bootstrap

---
