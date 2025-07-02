Thanks for sharing the Mobile Specifications Page design!

Here’s a complete breakdown and README-style documentation for your **Mobile Specifications Page** project, based on the design and instructions you provided.

---

## 📄 **README.md – Mobile Specifications Page**

### 📌 Overview

This project showcases the **Mobile Specifications Page** built using HTML, CSS, and Bootstrap. It displays an image of a mobile phone followed by its key specifications and a "Buy Now" button. The layout and styling closely follow the given reference design.

---

### 🧱 Project Structure

```
mobile-specs-page/
│
├── index.html        # Main HTML file
├── styles.css        # Custom CSS styles
└── assets/           # (Optional) For storing local images
```

---

### 🎯 Features

* Responsive design using Bootstrap
* Clean specifications section with bullet list
* Styled “Buy Now” button
* Font and color scheme consistent with the design

---

### 🖼️ Image Used

* Mobile Image:
  [iPhone X](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/iphoneX-bg.png)

---

### 🛠️ HTML Structure Breakdown

```html
<div class="card">
  <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/iphoneX-bg.png" class="card-img-top" alt="iPhone X" />

  <div class="card-body">
    <h5 class="card-title text-primary fw-bold">Specifications:</h5>
    <ul class="spec-list">
      <li>3 GB RAM</li>
      <li>5.80 Super Retina HD OLED Display</li>
      <li>Front Camera 7MP</li>
      <li>Rear Camera 12MP + 12MP</li>
      <li>Apple A11 Bionic Processor</li>
      <li>Battery Capacity 2716mAH</li>
    </ul>
    <a href="#" class="btn btn-primary">Buy Now</a>
  </div>
</div>
```

---

### 🎨 CSS Styling Notes

```css
body {
  font-family: 'Roboto', sans-serif;
  background-color: #ffffff;
}

.card {
  max-width: 350px;
  margin: 20px auto;
  border: 1px solid #e0e0e0;
}

.card-title {
  color: #1e293b;
}

.spec-list {
  padding-left: 1.2rem;
  color: #1e293b;
}

.btn-primary {
  background-color: #2563eb;
  border: none;
}
```

---

### 🎨 CSS Colors Used

| Element              | Hex Code  | Description         |
| -------------------- | --------- | ------------------- |
| Text color           | `#1e293b` | Navy dark gray-blue |
| Button color         | `#2563eb` | Bright blue         |
| Background (default) | `#ffffff` | White               |
| Border color         | `#e0e0e0` | Light gray          |

---

### 🧩 Bootstrap Classes Used

| Purpose         | Class Used                |
| --------------- | ------------------------- |
| Card layout     | `card`, `card-body`       |
| Image styling   | `card-img-top`            |
| Text formatting | `text-primary`, `fw-bold` |
| Button          | `btn`, `btn-primary`      |

---

### 📚 Font Used

* **Roboto**

To include Roboto, add this in `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet" />
```

---

