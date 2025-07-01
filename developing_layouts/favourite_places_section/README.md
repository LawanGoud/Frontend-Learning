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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tourism Website</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
 
</head>
<body>
    <div class="bg-container">
        <div class="card-container">
            <h1>Creating Workforce for 4.0</h1>
            <p>
                In this rapidly evolving technology and industry landscape, it is
                inevitable to constantly learn, unlearn, and relearn emerging
                technologies and 21st century skills to leverage this technology
                disruption. iB Hubs commits to create a powerful workforce with all
                the necessary tools and techniques to thrive in this new wave of                    transformation.
            </p>
        </div>
        <div class="card-container">
            <h1>Application Research and Development in 4.0 Technologies</h1>
            <p>
            iB Hubs Tech Parks carry out application Research and Development in
            these new-age technologies. This will lead to the building of
            innovative solutions for the world’s current challenges, enabling
            human advancement.
            </p>
      </div>
    </div>
</body>
</html>
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

