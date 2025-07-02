## ✅ **Movie Page Structure and Notes for README.md**

### 🎯 Goal:

Recreate a movie details page for **Finding Nemo** with:

* Carousel of images
* Movie description
* "Watch Now" button
* List of similar movies
* Responsive design with Bootstrap

---

## 📁 **Project Structure**

```
movie-page/
│
├── index.html         # Main HTML file
├── styles.css         # Custom styles
└── images/            # (Optional) Local backup of images
```

---

## 🧱 **Key HTML Elements Used**

### 1. **Background**

```css
body {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/orange-color-bg.png");
  background-size: cover;
  font-family: "Roboto", sans-serif;
}
```

### 2. **Image Carousel**

Use Bootstrap’s Carousel component with the 3 Nemo images.

```html
<div id="nemoCarousel" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner rounded">
    <div class="carousel-item active">
      <img src="nemo-c1-img.png" class="d-block w-100" />
    </div>
    <!-- Repeat for other images -->
  </div>
</div>
```

### 3. **Movie Details Section**

```html
<h2 class="text-white mt-3">Finding Nemo</h2>
<button class="btn btn-light mb-3">Watch Now</button>
<p class="text-white">
  A clown fish is overly cautious with his son, Nemo...
</p>
```

### 4. **Similar Movies Section**

```html
<h5 class="text-white">Similar Movies</h5>
<div class="d-flex justify-content-between">
  <img src="finding-dory-img.png" class="img-thumbnail rounded" />
  <img src="bugslife-img.png" class="img-thumbnail rounded" />
  <img src="ratatouille-movie-img.png" class="img-thumbnail rounded" />
</div>
```

---

## 🎨 **CSS Styling Tips**

```css
.movie-container {
  max-width: 300px;
  margin: auto;
  padding: 16px;
}

img {
  width: 100%;
  border-radius: 12px;
}

.carousel-inner img {
  border-radius: 12px;
}
```

---

## 🔧 **Resources Used**

### 🔗 **Image Links**

* Background: [orange-color-bg](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/orange-color-bg.png)
* Carousel:

  * [nemo-c1](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/nemo-c1-img.png)
  * [nemo-c2](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/nemo-c2-img.png)
  * [nemo-c3](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/nemo-c3-img.png)
* Similar Movies:

  * [Finding Dory](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/finding-dory-img.png)
  * [Bug's Life](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/bugslife-img.png)
  * [Ratatouille](https://d2clawv67efefq.cloudfront.net/ccbp-static-website/ratatouille-movie-img.png)

---

## ✅ **Bootstrap Classes Used**

| Purpose              | Class Used                   |
| -------------------- | ---------------------------- |
| Horizontal spacing   | `justify-content-between`    |
| Image responsiveness | `img-thumbnail`, `w-100`     |
| Buttons              | `btn`, `btn-light`           |
| Layout               | `d-flex`, `mt-3`, `mb-3`     |
| Typography           | `text-white`, `h5`, `h2`     |
| Carousel             | `carousel`, `carousel-inner` |

---

