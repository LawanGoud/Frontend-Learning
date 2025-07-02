Here’s a **concise and organized set of notes** based on the provided content about the **CCBP UI Kit** and **Tourism Website Sections**:

---

## 🌐 1. CCBP UI Kit

### 1.1 What is it?

* A collection of **reusable UI components**, similar to Bootstrap.
* Built specifically for **CCBP training**.

### 1.2 How to Add CCBP UI Kit to a Web Page

* Add the script **before the closing `</body>` tag**:

```html
<script type="text/javascript" src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/js/ccbp-ui-kit.js"></script>
```

* Bootstrap (optional but often used alongside):

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" />
```

### 1.3 Display Utility

* Used to **switch between different sections** on a single page.
* Example usage:

```html
<button onclick="display('section2')">Go to Section 2</button>
```

---

## 🏝️ 2. Tourism Website Sections

### 2.1 Home Section

#### HTML Structure

```html
<div class="bg-container d-flex flex-column justify-content-end">
  <div class="tourism-card">
    <h1 class="main-heading">Tourism</h1>
    <p class="paragraph">Plan your trip.</p>
    <button class="button">Get Started</button>
  </div>
</div>
```

#### CSS Styling

```css
.bg-container {
  background-image: url(".../ocean.jpg");
  height: 100vh;
  background-size: cover;
}
.tourism-card {
  background-color: white;
  border-top-left-radius: 25px;
  border-top-right-radius: 25px;
  text-align: center;
  padding: 5px;
}
.button {
  background-color: #25b1cc;
  border-radius: 20px;
  color: white;
}
```

---

### 2.2 Favourite Places Section

#### Content Example

* **Places**: Taj Mahal, Golden Temple, Mysore Palace, Varanasi Temple

#### HTML Structure (Each Card)

```html
<div class="favourite-place-card-container d-flex flex-row">
  <div>
    <h1 class="favourite-place-card-heading">Taj Mahal</h1>
    <p class="favourite-place-card-description">Description...</p>
  </div>
  <img src="..." class="favourite-place-card-image" />
</div>
```

#### CSS Tips

```css
.favourite-places-bg-container {
  background-image: url(".../towerbg.png");
  background-size: cover;
  padding: 24px;
  /* Note: remove 'height' to make image stretch based on content */
}
```

---

### 2.3 Detailed View Section

#### Features

* **Bootstrap Carousel** for sliding images
* Title and paragraph for detailed information

#### Carousel Snippet

```html
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="..." class="d-block w-100" />
    </div>
    <!-- More items -->
  </div>
</div>
```

---

## 📌 Notes

* **Don't set fixed height** on containers with background images if you want them to expand based on content.
* Use **Bootstrap classes** (`d-flex`, `justify-content-end`, etc.) for responsive design.
* Always include **CCBP UI Kit script** for utilities like `display()`.

---

Sure! Here's a **clean, structured set of notes** based on the HTML project and integration process you shared. These notes are designed to be **easy to understand**, help you revise, and preserve your current setup and instructions.

---

# 📝 HTML & Website Integration Notes for Tourism Project

---

## 3. HTML Attributes

### 3.1 The `id` Attribute

* **Used to uniquely identify** an HTML element.
* Each `id` **must be unique** in the document.
* **Important for CCBP UI Kit**:
  Every `id` for a section must start with `section` (e.g., `sectionHome`, `sectionFavouritePlaces`).
  ❗ Without this prefix, the **display function won't work**.

```html
<div id="sectionHome">...</div>
```

---

### 3.2 The `onclick` Attribute

* Executes a JavaScript function when an element is clicked.
* Syntax:

```html
<button onclick="display('sectionFavouritePlaces')">Click</button>
```

* **Use double quotes** around `onclick`, and **single quotes** inside `display()`.

---

## 4. Website Integration

---

### 4.1 Switching Between Home and Favourite Places

✅ **Steps to Navigate from Home to Favourite Places:**

1. ✅ Ensure section `id`s start with `section`.
2. ✅ Add HTML and CSS for **Home Section**.
3. ✅ Add HTML and CSS for **Favourite Places Section**.
4. ✅ Add `onclick="display('sectionFavouritePlaces')"` to the Home section button.

```html
<button onclick="display('sectionFavouritePlaces')">Get Started</button>
```

✅ **Steps to Navigate Back to Home Section:**

5. ✅ Add a **Back button** in Favourite Places.
6. ✅ Use `onclick="display('sectionHome')"` on the button.

```html
<button onclick="display('sectionHome')">Back</button>
```

---

### 4.2 Navigating to Taj Mahal Detailed View

✅ **Steps to Navigate from Favourite Places to Taj Mahal Detail View:**

1. ✅ Add HTML for `sectionTajMahalDetailedView`.
2. ✅ Add CSS for the detailed view.
3. ✅ Add `onclick="display('sectionTajMahalDetailedView')"` to the **Taj Mahal card container**.

```html
<div onclick="display('sectionTajMahalDetailedView')">...</div>
```

✅ **Steps to Go Back to Favourite Places:**

4. ✅ Add a Back button in `sectionTajMahalDetailedView`.
5. ✅ Use `onclick="display('sectionFavouritePlaces')"`.

```html
<button onclick="display('sectionFavouritePlaces')">Back</button>
```

---

## 💡 Quick Reminders

* ✅ Always use section `id`s with **prefix `section`**.
* ✅ `onclick` must follow proper syntax: `onclick="display('sectionName')"`
* ✅ Each section should be wrapped in a `div` with a unique `id`.

---

## 🔗 External Resources Used

* ✅ **Bootstrap 4** for styling
* ✅ **CCBP UI Kit** (`ccbp-ui-kit.js`) for switching sections
* ✅ **Google Fonts** for typography
* ✅ **CloudFront Images** for visual content

---

## ✅ File Structure Summary

```html
<sectionHome>               <!-- Main Tourism Page -->
<sectionFavouritePlaces>    <!-- List of Places -->
<sectionTajMahalDetailedView> <!-- Taj Mahal Detailed View -->
```

---

## ✅ Working Flow Diagram (Simple)

```
Home Page
  |
  v
[Favourite Places]
  |
  |-- Click "Taj Mahal" -->
  v
[Taj Mahal Detailed View]
  |
  <-- Back button --
  v
[Favourite Places]
  |
  <-- Back button --
  v
[Home Page]
```

---

Your HTML and CSS code together make up a **complete tourism website** with:

### ✅ Total Functional Components:

1. **Homepage ("Tourism")**

   * Fullscreen background
   * CTA button ("Get Started")

2. **Favourite Places Section**

   * Lists 4 tourist places:

     * Taj Mahal
     * Golden Temple
     * Mysore Palace
     * Varanasi Temple

3. **Detailed View Pages for Each Place**

   * Each has a Bootstrap carousel with 3 images
   * Text description
   * "Go Back" button to return to Favourite Places

4. **Navigation with JS**

   * Handled using the `display()` function from the `ccbp-ui-kit.js` script
   * This toggles visibility of sections

---

### 📦 Summary of Total Files and Features:

| Item                    | Count/Status            |
| ----------------------- | ----------------------- |
| HTML Sections           | 6 total                 |
| Places in List          | 4                       |
| Carousel in Each Place  | Yes (3 images each)     |
| External Libraries Used | Bootstrap, jQuery       |
| CSS File                | 1 (plus Bootstrap)      |
| JS Navigation Logic     | From CCBP UI Kit        |
| Fonts Used              | Google Fonts (multiple) |
| Responsiveness          | Via Bootstrap classes   |

---

### 💡 Suggestions for Completion (Optional Enhancements):

* Add a **navigation bar** to jump to sections.
* Make the `display()` function defined in your own JS file if you're not using ccbp-ui-kit.
* Add **footer** with contact info/social links.
* Add **Google Maps embed** for each place.
* Improve **accessibility** with proper `alt` tags and semantic HTML.


---

# 📋 HTML Lists

HTML Lists are a way to **group related pieces of information** so that they are **easy to read and understand**.

✅ **Examples:**

* Shopping List
* To-do List

There are mainly **two types of Lists** in HTML:

* Unordered List
* Ordered List

---

## 🔹 3.1 Unordered List

An **Unordered List** is a collection of related items that **have no special order or sequence**.

### ✅ Example: List of Hobbies

* Painting
* Reading Books
* Playing the Guitar

### 🧾 HTML Syntax

```html
<ul>
  <li>Painting</li>
  <li>Reading Books</li>
  <li>Playing the Guitar</li>
</ul>
```

> 🟢 **Note:** By default, list items in the Unordered List are marked with **bullets**.

---

### 🎨 3.1.1 Styling Unordered List

The CSS `list-style-type` property is used to **style the unordered list**.

### 🧾 CSS Example:

```css
.unordered-square-list {
  list-style-type: square;
}
```

### ✅ Possible Values for `list-style-type`:

| Value    | Description                        |
| -------- | ---------------------------------- |
| `square` | Solid square bullets               |
| `circle` | Hollow circle bullets              |
| `disc`   | Solid circle bullets (**default**) |
| `none`   | No bullets                         |

---

## 🔸 3.2 Ordered List

An **Ordered List** is a collection of related items that **follow some order or sequence**.

### ✅ Example: Web Technologies Learning Steps

1. Go through the HTML elements and CSS properties
2. Complete the Todolist Coding Practice
3. Go through the Bootstrap Concepts
4. Read the Bootstrap cheat sheet
5. Build a Tourism Website

### 🧾 HTML Syntax

```html
<ol>
  <li>Go through the HTML elements and CSS properties</li>
  <li>Complete the Todolist Coding Practice</li>
  <li>Go through the Bootstrap Concepts</li>
  <li>Read the Bootstrap cheat sheet</li>
  <li>Build a Tourism Website</li>
</ol>
```

> 🟢 **Note:** By default, list items in the Ordered List are marked with **numbers**.

---

### 🎨 3.2.1 Styling Ordered List

The CSS `list-style-type` property is used to **style the ordered list**.

### 🧾 CSS Example:

```css
.ordered-lower-roman-list {
  list-style-type: lower-roman;
}
```

### ✅ Possible Values for `list-style-type`:

| Value         | Description                              |
| ------------- | ---------------------------------------- |
| `upper-alpha` | Uppercase letters (A, B, C, …)           |
| `lower-alpha` | Lowercase letters (a, b, c, …)           |
| `upper-roman` | Uppercase Roman numerals (I, II, III, …) |
| `lower-roman` | Lowercase Roman numerals (i, ii, iii, …) |
| `decimal`     | Numbers (1, 2, 3, …)                     |
| `none`        | No numbering                             |

---

