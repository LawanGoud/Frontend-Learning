# 📘 Web Development Notes – HTML & CSS

These notes include basic concepts of HTML elements and CSS styling, ideal for beginners who are learning to build and style webpages.

---

## 1. HTML Elements

### 1.1 Image Element

The `<img>` tag is used to embed an image in an HTML page.

**Syntax:**
```html
<img src="IMAGE_URL" />
````

### 1.2 `src` Attribute

The `src` attribute specifies the path (URL) of the image.

**Example:**

```html
<img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/tajmahal-img.png" />
```

---

### 1.3 How to Get an Image URL from the Internet

Steps:

1. Go to [Google Images](https://images.google.com/)
2. Search for your image
3. Click to open the image
4. Right-click → "Open image in new tab"
5. Copy the URL from the address bar
6. Paste it in the `src` attribute of the `<img>` tag

---

### 1.4 Applying Height and Width to an Image

You can add multiple attributes like `class` for styling. Here’s an example:

**HTML:**

```html
<img
  src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/tajmahal-img.png"
  class="image"
/>
```

**CSS:**

```css
.image {
  width: 80px;
  height: 100px;
  border-radius: 8px;
}
```

---

## 2. Void Elements

Void elements are self-closing HTML elements without an end tag.

**Example:**

```html
<img src="..." />
```

Other void elements include: `<br>`, `<hr>`, `<input>`, etc.

---

## 3. CSS Box Model Properties

### 3.1 Margin

Margins define the space around elements.

**Example:**

```css
.card-container {
  margin: 10px;
}
```

You can apply margins to specific sides:

```css
margin-top: 10px;
margin-right: 10px;
margin-bottom: 10px;
margin-left: 10px;
```

---

## 4. Example Projects

### Project: Workforce Card

**HTML:**

```html
<div class="bg-container">
  <div class="card-container">
    <h1>Creating Workforce for 4.0</h1>
    <p>...</p>
  </div>
</div>
```

**CSS:**

```css
.bg-container {
  background-color: #214875;
  padding: 3px;
}

.card-container {
  background-color: #f7fbff;
  padding: 10px;
  margin: 10px;
}
```

---

### Project: Favourite Places

**HTML:**

```html
<div class="favourite-places-bg-container">
  <h1 class="favourite-places-heading">Favourite Places</h1>
  <div class="favourite-place-card-container d-flex flex-row">
    <div>
      <h1 class="favourite-place-card-heading">Taj Mahal</h1>
      <p class="favourite-place-card-description">...</p>
    </div>
    <img
      src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/tajmahal-img.png"
      class="favourite-place-card-image"
    />
  </div>
</div>
```

**CSS:**

```css
.favourite-places-bg-container {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/towerbg.png");
  height: 100vh;
  background-size: cover;
}

.favourite-places-heading {
  color: white;
  font-family: "Roboto";
  font-size: 28px;
  font-weight: bold;
  padding: 24px;
}

.favourite-place-card-container {
  background-color: white;
  border-radius: 8px;
  padding: 16px;
}

.favourite-place-card-heading {
  color: #0f0e46;
  font-size: 23px;
  font-weight: bold;
}

.favourite-place-card-description {
  color: #6c6b70;
  font-size: 13px;
}

.favourite-place-card-image {
  width: 80px;
  height: 100px;
}
```

---

## ✅ Summary

| Concept       | Description                    |
| ------------- | ------------------------------ |
| `<img>`       | Embeds an image in HTML        |
| `src`         | Attribute to specify image URL |
| Void Elements | Elements without closing tags  |
| CSS Margin    | Space around elements          |
| Project       | Built using Bootstrap and CSS  |

---

**📌 Next Steps:**

* Learn about padding and borders in CSS
* Try positioning elements using Flexbox or Grid
* Explore using media queries for responsiveness

---

**📁 Resources:**

* [HTML Reference - MDN](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS Reference - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)

