Great! You're working on the **Goa Tourism Page** assignment, and based on the screenshot and resources, here's a detailed guide to help you build the page using **HTML**, **CSS**, and optionally **Bootstrap**.

---

## ✅ Goa Page – Assignment Overview

### 📸 Page Sections

1. **Header Image Carousel**
2. **About Section**
3. **More Pictures**
4. **Videos (YouTube embedded)**

---

## 🧩 Structure & Features

### 1. 🔁 Image Carousel (Top)

Use Bootstrap's Carousel or a full-width image with scrolling support.

**Carousel Images:**

```text
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c1-img.png
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c2-img.png
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c3-img.png
```

### 2. 📄 About Section

**Text:**

> Goa is known for its striking landscape, famous beaches in India, astounding monuments and churches and bustling Goa nightlife. Goa is one of the most visited tourist places in India, especially on weekends, as it is not very far from Mumbai and having Panaji as its capital and Vasco da Gama as the largest city. It attracts a large number of tourists from all over the world, round the year.

* Font: **Roboto**
* Text color: A soft grey like `#7b8794`
* Header font color: `#323f4b`

### 3. 🖼️ More Pictures

Display 3 images in a row (can be done with Bootstrap grid or flexbox).

**Images:**

```text
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more1-img.png
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more2-img.png
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more3-img.png
```

### 4. ▶️ Videos Section

Embed 3 YouTube videos in square (1:1) aspect ratio.

**Video URLs:**

```text
https://www.youtube.com/embed/NFalCkZAClY
https://www.youtube.com/embed/4irzfMfTmM8
https://www.youtube.com/embed/OJu0gjzsvQE
```

Use Bootstrap’s embed class like:

```html
<div class="embed-responsive embed-responsive-1by1">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/NFalCkZAClY" allowfullscreen></iframe>
</div>
```

---

## 🧱 Suggested HTML Skeleton

```html
<!DOCTYPE html>
<html>
<head>
  <title>Goa Tourism</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <style>
    body {
      font-family: 'Roboto', sans-serif;
    }
    .section-title {
      color: #323f4b;
      font-weight: bold;
      margin-top: 20px;
    }
    .about-text {
      color: #7b8794;
    }
  </style>
</head>
<body>

<!-- Carousel Section -->
<div id="goaCarousel" class="carousel slide" data-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c1-img.png" class="d-block w-100">
    </div>
    <div class="carousel-item">
      <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c2-img.png" class="d-block w-100">
    </div>
    <div class="carousel-item">
      <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-c3-img.png" class="d-block w-100">
    </div>
  </div>
</div>

<!-- About Section -->
<div class="container mt-4">
  <h5 class="section-title">About</h5>
  <p class="about-text">
    Goa is known for its striking landscape, famous beaches in India, astounding monuments and churches and bustling Goa nightlife. Goa is one of the most visited tourist places in India...
  </p>

  <!-- More Pictures -->
  <h5 class="section-title">More Pictures</h5>
  <div class="d-flex justify-content-between">
    <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more1-img.png" class="img-thumbnail" width="100">
    <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more2-img.png" class="img-thumbnail" width="100">
    <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/goa-more3-img.png" class="img-thumbnail" width="100">
  </div>

  <!-- Videos Section -->
  <h5 class="section-title">Videos</h5>
  <div class="d-flex justify-content-between">
    <div class="embed-responsive embed-responsive-1by1 mr-2">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/NFalCkZAClY" allowfullscreen></iframe>
    </div>
    <div class="embed-responsive embed-responsive-1by1 mr-2">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/4irzfMfTmM8" allowfullscreen></iframe>
    </div>
    <div class="embed-responsive embed-responsive-1by1">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/OJu0gjzsvQE" allowfullscreen></iframe>
    </div>
  </div>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

---

