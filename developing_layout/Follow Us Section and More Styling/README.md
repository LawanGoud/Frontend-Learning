# Learning Notes

---

## 1. Adding Icons

Bootstrap Icons have a limited set. For more options, we use **Font Awesome Icons**.

### 1.1 Font Awesome Kit Setup

Add the following script tag in the `<head>` of your HTML:

```html
<script
  src="https://kit.fontawesome.com/fac54f0bd8.js"
  crossorigin="anonymous"
></script>
```

---

## 2. Follow Us Section with Font Awesome Icons

A custom section displaying social media icons (Twitter, Instagram, Facebook) using Font Awesome, styled with circular containers.

### 2.1 HTML Structure

```html
<div class="follow-us-section pt-5 pb-5" id="followUsSection">
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h1 class="follow-us-section-heading">Follow Us</h1>
      </div>
      <div class="col-12">
        <div class="d-flex flex-row justify-content-center">
          <div class="follow-us-icon-container">
            <i class="fab fa-twitter icon"></i>
          </div>
          <div class="follow-us-icon-container">
            <i class="fab fa-instagram icon"></i>
          </div>
          <div class="follow-us-icon-container">
            <i class="fab fa-facebook icon"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
```

### 2.2 CSS Styling

```css
.follow-us-section {
  background-color: white;
}

.follow-us-section-heading {
  text-align: center;
  color: #183b56;
  font-family: "Roboto";
  font-size: 28px;
  font-weight: 700;
}

.follow-us-icon-container {
  background-color: #faf7e8;
  width: 80px;
  height: 80px;
  border-radius: 40px;
  margin: 15px;
  padding: 22px 16px 14px 22px;
}

.icon {
  color: #d0b200;
  font-size: 35px;
}
```

---

## 3. Notes on `border-radius`

- The CSS `border-radius` property gives elements rounded corners.
- To get **circular corners**, height and width **must be equal**.
- If dimensions differ, you'll get **elliptical** shapes instead.

---

## 4. Adding Links to Page Sections

Use in-page navigation with `id` attributes and anchor `href`s.

### 4.1 Add `id` to Target Section

```html
<div class="wcu-section pt-5 pb-5" id="wcuSection">...</div>
```

### 4.2 Anchor Link Navigation

```html
<a class="nav-link active" id="navItem1" href="#wcuSection">
  Why Choose Us?
  <span class="sr-only">(current)</span>
</a>
```

- `href="#wcuSection"` links to the section with matching `id`.
- Bootstrap classes like `.nav-link` style navigation items.

---

## 5. Bootstrap Position Utilities

Bootstrap offers utilities to **fix** elements to the top or bottom of the viewport.

### 5.1 Fixed Top

- `fixed-top` keeps the element pinned to the **top** of the viewport even when scrolling.

```html
<nav class="navbar navbar-expand-lg navbar-light bg-white fixed-top">...</nav>
```

### 5.2 Fixed Bottom

- `fixed-bottom` keeps the element pinned to the **bottom** of the viewport.

```html
<nav class="navbar navbar-expand-lg navbar-light bg-white fixed-bottom">
  ...
</nav>
```

---
