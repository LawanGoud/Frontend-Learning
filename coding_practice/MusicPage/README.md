Here's a clean and organized **Markdown (`.md`) note** for your **Music Page Assignment**, including key concepts, code highlights, and usage instructions.

---

# 🎵 Music Page Assignment Notes

## 📘 Overview

In this assignment, we build a **Music Page** using:

* HTML
* CSS
* Bootstrap
* [CCBP UI Kit](https://learning.ccbp.in/)
  It consists of **two screens**:

1. **Music Home Page**
2. **Music Details Page**

---

## 🧠 Key Concepts Used

### ✅ CCBP UI Kit Requirements

* Section IDs must **start with `section`**
  ❗ `id="sectionMusicHome"` ✅
  ⛔ `id="musicHome"` ❌

* **Do not apply flex directly** to section containers.

```html
<!-- ❌ Wrong -->
<div id="sectionHomepage" class="d-flex">

<!-- ✅ Correct -->
<div id="sectionHomepage">
```

* Sections must be **parallel** (not nested).

---

## 📄 Page Structure

### 🎧 Music Home Page (`#sectionMusicHome`)

* Background: `#03174c`
* Top Section: Background image of **stars and moon**
* Heading: `"Sleep Music"`
* Description: `"Soothing bedtime music..."`
* Card with `"Night Island"` and a button: **"Get Started"**

```html
<button class="button" onclick="display('sectionMusicDetails')">Get Started</button>
```

---

### 🌌 Music Details Page (`#sectionMusicDetails`)

* Shows up when "Get Started" is clicked
* Background: Clouds image
* Description and related sleep music
* Two music cards:

  * **Moon Clouds** – 55 MIN
  * **Sweet Sleep** – 60 MIN

```html
<button class="button" onclick="display('sectionMusicHome')">Back</button>
```

---

## 🎨 Design Details

### 🖼️ Image Assets Used

| Image Type        | URL                                                                             |
| ----------------- | ------------------------------------------------------------------------------- |
| Moon Background   | `https://d2clawv67efefq.cloudfront.net/ccbp-static-website/moon-bg.png`         |
| Moon & Stars      | `https://new-assets.ccbp.in/frontend/static-website/moon-stars-bg.png`          |
| Clouds Header     | `https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/clouds-img.png`      |
| Moon Clouds Music | `https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/moon-clouds-img.png` |
| Sweet Sleep Music | `https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/sweet-sleep-img.png` |

---

## 🖌️ CSS Styling Notes

### 🎨 Colors

| Usage            | Hex Code  |
| ---------------- | --------- |
| Background       | `#03174c` |
| Button BG        | `#8e97fd` |
| Description Text | `#98a1bd` |
| Highlight Text   | `#ffe7bf` |

### 🔤 Font Family

```css
font-family: "Bree Serif";
```

Imported from Google Fonts:

```css
@import url('https://fonts.googleapis.com/css2?family=Bree+Serif&display=swap');
```

### 🎛️ Button

```css
.button {
    background-color: #8e97fd;
    border-radius: 38px;
    width: 100px;
    height: 30px;
}
```

---

## 📜 JavaScript

To switch between pages:

```html
<script src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/js/ccbp-ui-kit.js"></script>
```

Use `display('sectionId')` function to show/hide sections.

---

## ✅ What You Learned

* HTML layout using Bootstrap and semantic tags.
* Switching screens using the `display()` function (from CCBP UI Kit).
* Responsive design using images, background colors, and typography.
* Good use of **UI Kit conventions**, especially section ID rules.

---

