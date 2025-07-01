Here's a well-organized **README.md** notes section based on the full content you provided. It's formatted and structured for clarity and professional documentation:

---

# 🎆 Diwali Celebration Web Page – Developer Notes

This project is a responsive **Diwali Celebration Page** designed using **HTML**, **CSS**, **Bootstrap**, and **Google Fonts**. The webpage is divided into two primary sections: a **Top Section** with a background image and heading, and a **Bottom Section** showcasing Diwali product cards with a call-to-action button.

---

## 1. 🖼️ HTML Image vs CSS Background Image

### Ways to Add Images in a Website:

* **HTML Image**
* **CSS Background Image**

### When to Use:

#### ✅ HTML Image:

* When the image is **part of the content**.
* When **no content** or HTML elements are placed **over** the image.

#### ✅ CSS Background Image:

* When the image is **not part of the content**.
* When **HTML elements** or **text** are overlaid on top of the image.

---

## 2. 📦 CSS Margin vs CSS Padding

### When to Use:

#### ✅ CSS Padding:

* Adds **space between content and the border** of an HTML element.
* Defines **internal spacing**.

#### ✅ CSS Margin:

* Adds **space around elements** (external).
* Used to manage spacing **between different elements**.

### Example:

```html
<button class="button">View More</button>
```

```css
.button {
  padding: 20px;
  margin: 15px;
}
```

---

## 3. 🧱 Step-by-Step Process to Develop the Diwali Page

The webpage is divided into:

* **Top Section**
* **Bottom Section**

Use suitable **CSS properties and values** from the previous cheat sheets for layout and styling.

---

### 3.1 🌟 Top Section

#### 🔹 Step 1: Add Background Image

* Set `background-image`, `height`, and `background-size`.

#### 🔹 Step 2: Add Heading

* Use `color`, `font-family`, `font-size`, `width`, and `padding`.

```css
.diwali-top-section {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/diwali-bg.png");
  height: 30vh;
  background-size: cover;
}

.diwali-top-section-heading {
  color: white;
  font-family: "Caveat";
  font-size: 36px;
  width: 200px;
  padding: 20px;
}
```

---

### 3.2 🎁 Bottom Section

#### 🔹 Step 1: Add Bottom Section Container

* Use `background-color` and `padding`.

#### 🔹 Step 2: Add Card Items

Each card contains:

* **Image** (`width`, `height`)
* **Name** (`color`, `font-size`)
* **Price** (`color`, `font-weight`)
* Add `padding`, `text-align`, and `margin`.

```css
.diwali-bottom-section {
  text-align: center;
  background-color: #e6f6ff;
  padding: 15px;
}

.diwali-card-item {
  text-align: center;
  background-color: white;
  width: 140px;
  border-radius: 9px;
  padding: 16px;
  margin: 15px;
}
```

#### 🔹 Step 3: Align Cards Using Flexbox

* Wrap every two cards in a `d-flex flex-row justify-content-center` container.

#### 🔹 Step 4: Add Button

* Use Bootstrap `btn` and `btn-primary` classes.

```html
<button class="btn btn-primary">View More</button>
```

---

## 4. 🖼️ Resources Used

### ✅ Background Image URL:

```
https://d2clawv67efefq.cloudfront.net/ccbp-static-website/diwali-bg.png
```

### ✅ Card Item Image URLs:

* Lamp:

  ```
  https://d2clawv67efefq.cloudfront.net/ccbp-static-website/lamp-img.png
  ```
* Diya:

  ```
  https://d2clawv67efefq.cloudfront.net/ccbp-static-website/diya-img.png
  ```
* Firework:

  ```
  https://d2clawv67efefq.cloudfront.net/ccbp-static-website/firework-img.png
  ```
* Firecracker:

  ```
  https://d2clawv67efefq.cloudfront.net/ccbp-static-website/firecracker-img.png
  ```

---

## 5. 🎨 Colors Used

### Named Colors:

* `white`

### Hex Codes:

* Background: `#e6f6ff`
* Card Title: `#616e7c`
* Card Price: `#323f4b`

---

## 6. 🔠 Fonts Used

Google Fonts Imported:

* Caveat
* Roboto
* Bree Serif
* Open Sans
* Work Sans
* Playfair Display
* Playfair Display SC
* Monoton
* Lobster
* Source Sans Pro

```css
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");
```

---

✅ **This README provides a clear roadmap to recreate or modify the Diwali webpage project effectively.**
