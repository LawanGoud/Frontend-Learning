# 📓 Favourite Place Detailed View Page using Bootstrap

---

## 🔧 1. Bootstrap Components

### 1.1 Carousel

* Used to create a slideshow of images.
* Bootstrap Carousel supports indicators, controls, and multiple items.
* Code snippet for each image:

  ```html
  <img
    class="d-block w-100"
    src="IMAGE_URL_HERE"
    alt="..."
  />
  ```
* Example setup:

  ```html
  <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
      <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="tajmahal-c1-img.png" class="d-block w-100" alt="..." />
      </div>
      ...
    </div>
    <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">...</a>
    <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">...</a>
  </div>
  ```

---

## 🧩 2. Bootstrap Utilities

### 2.1 Embed Responsive YouTube Video

* Used Bootstrap’s `embed-responsive` class.
* Change the **video ID** inside the `src` attribute:

  ```html
  <div class="embed-responsive embed-responsive-16by9">
    <iframe
      class="embed-responsive-item"
      src="https://www.youtube.com/embed/VIDEO_ID_HERE?rel=0"
      allowfullscreen
    ></iframe>
  </div>
  ```

### 2.1.1 🔎 How to Get a YouTube Video ID

1. Visit [youtube.com](https://youtube.com)
2. Search and select the video
3. Copy the video ID:

   * From URL: `https://www.youtube.com/watch?v=49HTIoCccDY`
   * Video ID = `49HTIoCccDY`
4. Embed it like this:

   ```html
   src="https://www.youtube.com/embed/49HTIoCccDY?rel=0"
   ```

---

## 🧱 3. Step-by-Step Project Development

### ✅ Step 1: Background Image and Heading

* Add full-screen background:

  ```css
  .detailed-view-bg-container {
    background-image: url("seabg.png");
    height: 100vh;
    background-size: cover;
  }
  ```
* Heading:

  ```html
  <h1 class="detailed-view-heading">Detailed View</h1>
  ```

---

### ✅ Step 2: Create the Detailed View Card

#### 🟦 2.1 Add Card Container

```html
<div class="detailed-view-card-container"> ... </div>
```

#### 🖼️ 2.2 Add Carousel or YouTube Embed

* **Option 1: Bootstrap Carousel**
* **Option 2: YouTube Video using Embed**

#### 📝 2.3 Add Text Content

```html
<h1 class="detailed-view-card-heading">Taj Mahal</h1>
<p class="detailed-view-card-description">
  The Taj Mahal is considered to be the greatest architectural achievement...
</p>
```

---

### 🎨 Step 3: Add Styling

```css
.detailed-view-card-container {
  background-color: white;
  border-radius: 8px;
  margin: 24px;
}

.detailed-view-card-text-container {
  padding: 16px;
}

.detailed-view-card-heading {
  font-size: 23px;
  color: #0f0e46;
}

.detailed-view-card-description {
  font-size: 13px;
  color: #6c6b70;
}
```

---

## 📁 Project Folder Structure

```
Favourite-Place-Project/
│
├── index.html
├── styles.css
└── README.md (includes setup guide and development steps)
```

---

## ✅ Summary

| Feature             | Implemented  |
| ------------------- | ------------ |
| Bootstrap Carousel  | ✅            |
| Embed YouTube Video | ✅ (optional) |
| Custom Styling      | ✅            |
| Responsive Layout   | ✅            |

---

