## 🌐 **HTML + CSS Learning Path**

---

### 🧱 **HTML Basics**

* **Tags**

  * `h1` – Heading
  * `p` – Paragraph
  * `button` – Button
  * `div` – Container
  * `img` – Image

    * `src` – Source Attribute
* **Lists**

  * `ul` – Unordered List
  * `ol` – Ordered List
  * `li` – List Item

---

### 🔗 **HTML Anchor (`<a>`)**

* Used to create hyperlinks:

  * External links (e.g., to a website)
  * Internal navigation (within the same page)
* **Attributes**

  * `href` – Destination URL or `#id` for internal
  * `target="_blank"` – Open in new tab

---

### 🧭 **Internal Navigation**

* Use `id` on destination section
* Link using `href="#sectionId"`

```html
<a href="#about">Go to About</a>
<div id="about">...</div>
```

---

### 🚫 **Void (Self-Closing) Elements**

* `<br>` – Line break
* `<hr>` – Horizontal line

---

### 🏷️ **Common HTML Attributes**

* `class`
* `id`
* `onclick`

---

### 🎨 **CSS Text & Font Styling**

* `color`
* `font-size`
* `font-family`
* `font-weight`
* `font-style`
* `text-decoration`
* `text-align`

---

### 🖼️ **CSS Background Styling**

* `background-color`
* `background-image`
* `background-size`

---

### 📦 **Box Model**

* `height`
* `width`
* `margin`
* `padding`
* `border`

  * `border-radius`

    * `border-top-left-radius`
    * `border-top-right-radius`
    * `border-bottom-left-radius`
    * `border-bottom-right-radius`
  * `border-width`

---

### 🧰 **Flexbox Layout**

* `d-flex`
* `flex-row`
* `flex-column`
* `justify-content-start`
* `justify-content-center`
* `justify-content-end`

---

### 🖌️ **Structure & Styling Practices**

* Use `div`s for layout structure
* Apply styles with:

  * CSS
  * Bootstrap
  * Google Fonts (via import)

---

### 📷 **Embedding Media**

* Wrap images in links:

```html
<a href="https://example.com">
  <img src="image.png" />
</a>
```

---

### ⚙️ **Bootstrap Components**

* Buttons
* Carousel
* Video Embed

  * YouTube Video

---

### 🧩 **CCBP UI Kit**

* Display Utility

---

### ☁️ **Web Fundamentals**

* **Internet**

  * IP Address
  * DNS Server
* **AWS (Amazon Web Services)**

  * Route 53
  * S3

---


---

---

### 📝 Notes: HTML Basic Structure – Step-by-Step Breakdown

---

#### 🔹 What is HTML?

* **HTML** stands for **HyperText Markup Language**.
* It is the **standard language** used to create and structure web pages.
* HTML describes the **content and layout** of a webpage using **elements and tags**.

---

#### 🔹 Basic HTML Document Structure

Here’s the **default template** of any HTML file:

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    Your code goes here
  </body>
</html>
```

Let’s break down each part in detail:

---

#### 1. `<!DOCTYPE html>` – Document Type Declaration

* This **declaration** tells the browser:

  > “This is an HTML5 document.”
* Always appears **at the top** of the HTML file.
* Helps browsers **render the page correctly**.

---

#### 2. `<html> ... </html>` – Root Element

* This is the **root** of the HTML document.
* All other elements go **inside** this tag.
* Attributes (like `lang="en"`) can be added:

  ```html
  <html lang="en">
  ```

---

#### 3. `<head> ... </head>` – Head Section

* The **metadata** of the page goes here.
* Doesn’t contain visible content.
* Typical content inside `<head>` includes:

  * `<title>` – Sets the page title in the browser tab
  * `<meta>` – Info like character encoding and viewport settings
  * `<link>` – Links to external resources like CSS
  * `<style>` – Internal CSS styles
  * `<script>` – JavaScript for client-side behavior

Example:

```html
<head>
  <title>My Webpage</title>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="style.css">
</head>
```

---

#### 4. `<body> ... </body>` – Body Section

* Everything inside `<body>` is **visible** on the webpage.
* This is where your **actual webpage content** goes.
* Can include:

  * Text (`<p>`, `<h1>` to `<h6>`)
  * Media (`<img>`, `<video>`)
  * Links (`<a>`)
  * Lists (`<ul>`, `<ol>`)
  * Layout containers (`<div>`, `<section>`)
  * Forms (`<form>`, `<input>`, `<button>`), etc.

Example:

```html
<body>
  <h1>Welcome to My Site</h1>
  <p>This is a paragraph of text.</p>
</body>
```

---

### ✅ Summary: Step-by-Step Template Use

1. **Start** with `<!DOCTYPE html>`
2. **Wrap everything** inside `<html>`
3. **Put page settings** in `<head>`
4. **Write visible content** in `<body>`

---

### 🧠 Pro Tip:

* Use proper indentation (2 spaces or a tab) to keep code readable.
* Always **close tags** properly.
* Use a **code editor** like VS Code for syntax highlighting and auto-completion.

---
---

# 📝 HTML Elements – Complete Step-by-Step Notes

---

## 🔸 1. Heading Element

* The `<h1>` tag defines the **main heading** of a web page.
* There are 6 heading levels: `<h1>` to `<h6>`, where `<h1>` is the most important.

**Example:**

```html
<h1>Tourism</h1>
```

---

## 🔸 2. Paragraph Element

* The `<p>` tag is used to define a **paragraph** of text.

**Example:**

```html
<p>Plan your trip wherever you want to go</p>
```

---

## 🔸 3. Button Element

* The `<button>` element creates a **clickable button**.

**Example:**

```html
<button>Get Started</button>
```

---

## 🔸 4. Container Element

* The `<div>` tag is a **block-level container** used to group elements together.
* It helps in organizing content and applying styles.

**Example:**

```html
<div>
  <h1>Tourism</h1>
  <p>Plan your trip wherever you want to go</p>
  <button>Get Started</button>
</div>
```

---

## 🔸 5. Image Element

* The `<img>` tag is used to **display an image**.
* It’s a **void element** (self-closing).

### 5.1 `src` Attribute

* The `src` attribute holds the **URL/path** of the image.

**Syntax:**

```html
<img src="IMAGE_URL" />
```

**Example:**

```html
<img src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/tajmahal-img.png" />
```

---

## 🔸 6. Anchor Element

* The `<a>` tag defines a **hyperlink**.
* Used to navigate to other web pages or sections.

### Syntax:

```html
<a href="URL">Content</a>
```

### 6.1 `href` Attribute

* The `href` attribute sets the **destination URL**.

**Example:**

```html
<a href="https://www.ccbp.in/">Explore CCBP 4.0 Certification Programs</a>
```

---

### 6.2 Ways to Use Anchor Elements

#### 6.2.1 Navigate Within the Same HTML Document

* Use the `id` attribute on a target element.
* Use `#idValue` in the `href` attribute to link to that section.

```html
<a href="#section1">Go to Section 1</a>

...

<h2 id="section1">Section 1</h2>
```

> ⚠️ Note: If the target section has very little content, it may not scroll visibly.

#### 6.2.2 Image as a Link

* Wrap the `<img>` tag inside an `<a>` tag.

**Example:**

```html
<a href="https://www.ccbp.in/">
  <img src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/learn-technologies-img.png" />
</a>
```

---

## 🔸 7. Void Elements

* Elements with **no closing tag** and **no content** inside.
* Self-closing with `/`.

**Example:**

```html
<img src="image.png" />
```

---

## 🔸 8. Line Break Element

* The `<br />` tag **inserts a line break** in text.

**Example:**

```html
<p>
  Twinkle, twinkle, little star, <br />
  How I wonder what you are!
</p>
```

---

## 🔸 9. Horizontal Rule Element

* The `<hr />` tag adds a **horizontal line** to separate content.

**Example:**

```html
<h1>Title</h1>
<hr />
<p>Content below the line</p>
```

---

## 🔸 10. HTML Lists

* Lists group related content.
* Two main types:

  * **Unordered List (`<ul>`)** – No specific order
  * **Ordered List (`<ol>`)** – Items have a sequence

---

## 🔸 11. Unordered List

* Starts with `<ul>`, each item inside `<li>`.
* Default style: **bullet points**.

**Example:**

```html
<ul>
  <li>Painting</li>
  <li>Reading Books</li>
</ul>
```

### 11.1 Styling Unordered Lists

* Use `list-style-type` in CSS.

```css
.unordered-square-list {
  list-style-type: square;
}
```

**Style Options:**

* `disc` (default)
* `circle`
* `square`
* `none`

---

## 🔸 12. Ordered List

* Starts with `<ol>`, each item inside `<li>`.
* Default style: **numbers**.

**Example:**

```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

### 12.1 Styling Ordered Lists

* Use `list-style-type` in CSS.

```css
.ordered-lower-roman-list {
  list-style-type: lower-roman;
}
```

**Style Options:**

* `decimal` (default)
* `upper-alpha`, `lower-alpha`
* `upper-roman`, `lower-roman`
* `none`

---

## ✅ Quick Recap:

| Tag             | Purpose         | Example                  |
| --------------- | --------------- | ------------------------ |
| `<h1>` – `<h6>` | Headings        | `<h1>Title</h1>`         |
| `<p>`           | Paragraph       | `<p>Text</p>`            |
| `<button>`      | Button          | `<button>Click</button>` |
| `<div>`         | Container       | `<div>...</div>`         |
| `<img>`         | Image           | `<img src="url" />`      |
| `<a>`           | Link            | `<a href="url">Text</a>` |
| `<br />`        | Line Break      | Used inside `<p>`        |
| `<hr />`        | Horizontal Line | Separates sections       |
| `<ul>`, `<ol>`  | Lists           | `<li>Item</li>`          |

---



# 📝 HTML Attributes – Detailed Notes

---

## 🔹 What are HTML Attributes?

* HTML attributes provide **additional information** about elements.
* They are always written **in the opening tag**.
* Syntax: `attribute="value"`

---

## 🔸 1. `id` Attribute

* The `id` attribute is used to assign a **unique identifier** to an HTML element.
* The value **must be unique** across the entire document.

**Syntax:**

```html
<tag id="uniqueId">Content</tag>
```

**Example:**

```html
<div id="section1">Section 1</div>
```

### ✅ Usage:

* Used to target elements with **CSS** or **JavaScript**.
* Used for internal page navigation (`<a href="#section1">`).

### ⚠️ Special Note (For CCBP UI Kit Users):

* IDs for sections **must start with `section`**, e.g., `section1`, `sectionHome`.
* This is a **requirement for CCBP UI Kit** to work properly.

---

## 🔸 2. `onclick` Attribute

* Triggers a **JavaScript function** when the element is **clicked**.
* Commonly used with buttons or clickable elements.

**Syntax:**

```html
<tag onclick="functionName('value')">Content</tag>
```

**Example:**

```html
<button class="btn btn-primary" onclick="display('section3')">
  Go to Section 3
</button>
```

### ⚠️ Syntax Tip:

* Double quotes for the `onclick` value.
* **Single quotes** inside the function call.

---

## 🔸 3. `src` Attribute

* Used with the `<img>` tag to define the **image URL/path**.
* Tells the browser **where to fetch the image** from.

**Syntax:**

```html
<img src="IMAGE_URL" />
```

**Example:**

```html
<img src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/tajmahal-img.png" />
```

---

## 🔸 4. `href` Attribute

* Used with the `<a>` tag to define the **destination URL**.
* Clicking the link sends the user to this path.

**Syntax:**

```html
<a href="URL">Link Text</a>
```

**Example:**

```html
<a href="https://www.ccbp.in/">Explore CCBP 4.0 Certification Programs</a>
```

---

## 🔸 5. `target` Attribute

* Defines **where** to open the linked document.
* Common values:

  * `_self`: Default. Opens in **same tab**.
  * `_blank`: Opens in a **new tab**.
  * `_parent`, `_top`: Less commonly used, for frames.

**Syntax:**

```html
<a href="URL" target="value">Link Text</a>
```

**Example:**

```html
<a href="https://www.ccbp.in/" target="_blank">Explore CCBP 4.0 Certification Programs</a>
```

---

## ✅ Summary Table

| Attribute | Description                      | Example                         |
| --------- | -------------------------------- | ------------------------------- |
| `id`      | Unique identifier for an element | `<div id="section1">`           |
| `onclick` | Triggers JS on click             | `<button onclick="func('id')">` |
| `src`     | Image source path                | `<img src="image.png" />`       |
| `href`    | URL to navigate to               | `<a href="url">`                |
| `target`  | Where to open the link           | `target="_blank"`               |

---

# 📝 CSS Syntax & Text Properties – Step-by-Step Notes

---

## 🎯 What is CSS?

* **CSS (Cascading Style Sheets)** is used to style HTML elements.
* It defines **how** elements should look on a webpage (colors, fonts, spacing, etc.)

---

## 🔸 CSS Syntax

```css
selector {
  property1: value1;
  property2: value2;
}
```

* **Selector**: Targets the HTML element.
* **Property**: The style to apply (e.g., color, font-size).
* **Value**: Defines the setting for the property.

---

## 🔹 Text Properties in CSS

---

### ✅ 1. `text-align`

* Aligns text **horizontally** inside an element.

```css
.h-center {
  text-align: center;
}
```

**Values:**

| Value  | Description               |
| ------ | ------------------------- |
| center | Aligns text to the center |
| left   | Aligns text to the left   |
| right  | Aligns text to the right  |

---

### ✅ 2. `color`

* Sets the **text color**.

```css
.main-heading {
  color: blue;
}
.paragraph {
  color: grey;
}
```

#### 2.1. Common Named Colors

* blue, grey, lightblue, orange, red, green

#### 2.2. Hex Code Colors

* Used when a named color isn't specific enough.

| Color Name | Hex Code  |
| ---------- | --------- |
| orange     | `#ffa500` |
| red        | `#ff0000` |
| blue       | `#0000ff` |
| green      | `#008000` |
| teal-dark  | `#012d36` |
| brown-dark | `#432711` |
| cyan       | `#25b1cc` |

```css
.button {
  background-color: #25b1cc;
}
```

#### 2.2.1. Picking Colors

* Use **Google's color picker** by typing "color picker" in the search bar.

---

### ✅ 3. `font-family`

* Sets the **font** used for text.

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");

.main-heading {
  font-family: "Roboto";
}
```

> ⚠️ **Notes:**
>
> * Always enclose font names in **quotes**.
> * Make sure to **import Google Fonts** correctly.
> * No spelling errors in font names.

---

### ✅ 4. `font-size`

* Sets the **size of the font**.

```css
.main-heading {
  font-size: 36px;
}
.paragraph {
  font-size: 28px;
}
```

> ⚠️ **Rules:**
>
> * Use `px` for pixel values.
> * No space between number and `px`.
> * Do **not** use quotes.

---

### ✅ 5. `font-style`

* Defines the **style of the font**.

```css
.main-heading {
  font-style: italic;
}
.paragraph {
  font-style: normal;
}
```

**Values:**

* `normal`
* `italic`
* `oblique`

> ⚠️ No quotes or spelling mistakes.

---

### ✅ 6. `font-weight`

* Sets the **thickness** of the text.

```css
.main-heading {
  font-weight: bold;
}
.paragraph {
  font-weight: 200;
}
```

**Values:**

* Keywords: `normal`, `bold`, `bolder`, `lighter`
* Numeric: 100–900 (multiples of 100)

> ⚠️ Avoid typos; use only allowed values.

---

### ✅ 7. `text-decoration`

* Adds **visual decoration** to text.

```css
.main-heading {
  text-decoration: underline;
}
.paragraph {
  text-decoration: overline;
}
```

**Values:**

| Value        | Description          |
| ------------ | -------------------- |
| underline    | Underlines the text  |
| line-through | Strikes through text |
| overline     | Line above the text  |

> ⚠️ Use hyphens correctly (`line-through`), and no quotes.

---

## 🔚 Summary Table

| Property          | Purpose                   | Common Values                     |
| ----------------- | ------------------------- | --------------------------------- |
| `text-align`      | Align text                | center, left, right               |
| `color`           | Text color                | red, blue, #ff0000                |
| `font-family`     | Font style                | "Roboto", "Lobster"               |
| `font-size`       | Text size                 | 28px, 36px                        |
| `font-style`      | Italic or normal text     | normal, italic, oblique           |
| `font-weight`     | Thickness of text         | bold, 400, 700                    |
| `text-decoration` | Underline, overline, etc. | underline, line-through, overline |


---

# 🧱 CSS Background & Box Properties – Notes

---

## 🎨 Background Properties

---

### ✅ 1. `background-color`

* Sets the **background color** of an element.

```css
.card {
  background-color: lightblue;
}
```

---

### ✅ 2. `background-image`

* Sets a **background image**.

```css
.card {
  background-image: url("https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/ocean.jpg");
}
```

> ⚠️ **Warnings:**
>
> * Background image takes the **height of the content** if no `height` is set.
> * Make sure the `url()` is **valid and correct**.

---

### ✅ 3. `background-size`

* Defines how the background image should scale.

```css
.card {
  background-size: cover;
}
```

**Value:**

* `cover`: Scales the image to cover the entire element while **maintaining aspect ratio** (width/height), even if it gets cropped.

---

## 📦 Box Properties

---

### ✅ 1. `height`

* Sets the **height** of an element.

```css
.card {
  height: 200px;
}
```

---

### ✅ 2. `width`

* Sets the **width** of an element.

```css
.card {
  width: 250px;
}
```

---

### ✅ 3. `border-width`

* Sets the **thickness** of the border.

```css
.button {
  border-width: 2px;
}
```

To **remove the border**:

```css
.button {
  border-width: 0px;
}
```

> ⚠️ **Important**:
>
> * You must also specify `border-style`, otherwise border won’t be visible (except on `<button>`).

---

### ✅ 4. `border-radius`

* Rounds the **corners** of an element.

```css
.button {
  border-radius: 20px;
}
```

To round **specific corners**:

```css
border-top-left-radius
border-top-right-radius
border-bottom-left-radius
border-bottom-right-radius
```

> 💡 Tip: Add `background-color` to better see the rounded corners.

---

### ✅ 5. `border-color`

* Sets the **color of the border**.

```css
.button {
  border-color: orange;
}
```

> ⚠️ Must be used **with** `border-style` to be visible.

---

### ✅ 6. `border-style`

* Defines the **style/appearance** of the border.

```css
.button {
  border-style: dashed;
}
```

**Common Values:**

| Value  | Description         |
| ------ | ------------------- |
| dotted | Dotted border       |
| dashed | Dashed border       |
| solid  | Solid line          |
| none   | No border (default) |

---

### ✅ 7. `padding`

* Space **inside the border**, around content.

```css
.card {
  padding: 10px;
}
```

---

### ✅ 8. `margin`

* Space **outside the border**, around the element.

```css
.card-container {
  margin: 10px;
}
```

To apply margin on specific sides:

```css
margin-top
margin-right
margin-bottom
margin-left
```

---

## 📌 Quick Summary Table

| Property           | Purpose                  | Sample Value        |
| ------------------ | ------------------------ | ------------------- |
| `background-color` | Background color         | lightblue           |
| `background-image` | Background image         | url("...")          |
| `background-size`  | Scaling background image | cover               |
| `height`           | Height of element        | 200px               |
| `width`            | Width of element         | 250px               |
| `border-width`     | Thickness of border      | 2px                 |
| `border-color`     | Border color             | orange              |
| `border-style`     | Style of border          | solid, dashed, etc. |
| `border-radius`    | Rounded corners          | 20px                |
| `padding`          | Space inside element     | 10px                |
| `margin`           | Space outside element    | 10px                |

---

---

# 🌐 CSS Viewport Units – `vh` and `vw`

---

## 📏 What is the Viewport?

> The **viewport** is the **visible area** of a web page in the browser window.

---

## 📐 1. `vh` – Viewport Height

* **`1vh` = 1%** of the **viewport height**.
* Used to make elements scale relative to the height of the browser window.

```css
.card {
  height: 50vh; /* Takes up half the viewport height */
}
```

🔹 **Example:**

```css
.full-screen {
  height: 100vh; /* Fills the entire vertical screen */
}
```

---

## 📐 2. `vw` – Viewport Width

* **`1vw` = 1%** of the **viewport width**.
* Used to make elements scale relative to the width of the browser window.

```css
.card {
  width: 100vw; /* Fills the full width of the screen */
}
```

---

## ✅ Summary Table

| Unit | Description     | 1 Unit Equals               | Common Use                             |
| ---- | --------------- | --------------------------- | -------------------------------------- |
| `vh` | Viewport Height | 1% of browser window height | Fullscreen sections, banners, etc.     |
| `vw` | Viewport Width  | 1% of browser window width  | Full-width layouts, responsive designs |

---

## 📌 Notes

* `100vh` or `100vw` makes an element occupy the **full screen height or width**.
* Viewport units are excellent for **responsive design**.
* Avoid horizontal scroll by handling paddings/margins when using `100vw`.

---

---

# ♻️ CSS Reusability & Multiple Class Names

---

## ✅ 1. Reusability of CSS Rulesets

**Why?**
To avoid writing the same styles multiple times for different HTML elements.

### 🔹 Concept:

Write a **CSS class** once and apply it to **multiple elements** by using the `class` attribute.

### 🔹 Example:

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}
```

```html
<button class="button">Get Started</button>
<button class="button">Visit Now</button>
```

🟢 Both buttons now share the **same consistent styling** from the `.button` class.

---

## ✅ 2. Using Multiple Class Names in HTML

### 🔹 Why?

To **combine multiple styles** for a single element.

### 🔹 Syntax:

```html
<tag class="class1 class2 class3">Content</tag>
```

* Class names must be **separated by a space**.
* CSS rules from **all listed classes** will be applied **in order**.

---

### 🔹 Example:

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}

.button-green {
  background-color: #8cc63f;
}
```

```html
<button class="button button-green">Get Started</button>
```

🟢 This button will:

* Use size and shape from `.button`
* Use background color from `.button-green`

---

## 💡 Pro Tips:

| Best Practice          | Description                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------ |
| 🔁 **Reuse styles**    | Saves time and keeps code clean                                                      |
| 📚 **Modular CSS**     | Break styling into logical, reusable parts                                           |
| ⚠️ **Order matters**   | If two classes have the same property, the one written **later** in CSS takes effect |
| 🎯 **Semantic naming** | Name classes by role/purpose (e.g., `.btn-primary`, `.card-shadow`)                  |

---

# 🚀 Bootstrap (v4.5.2)

## ✅ What is Bootstrap?

**Bootstrap** is a **free and open-source** front-end framework used to build **responsive**, **mobile-first** websites quickly.

It includes a **large collection of reusable code snippets** written in:

* ✅ HTML
* ✅ CSS
* ✅ JavaScript

These snippets help create components like:

* 🔹 Buttons
* 🔹 Cards
* 🔹 Navbars
* 🔹 Carousels
* 🔹 Modals
* ...and many more.

---

## 🛠 How to Use Bootstrap?

To start using Bootstrap, include the **Bootstrap CDN** (Content Delivery Network) in your HTML document — usually inside the `<head>` tag.

### 📌 Bootstrap CDN Code:

```html
<!-- Bootstrap CSS -->
<link
  rel="stylesheet"
  href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
  integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z"
  crossorigin="anonymous"
/>

<!-- Bootstrap JS (with dependencies) -->
<script
  src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
  integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
  crossorigin="anonymous"
></script>
<script
  src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"
  integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN"
  crossorigin="anonymous"
></script>
<script
  src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"
  integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV"
  crossorigin="anonymous"
></script>
```

---

## 🧠 Quick Notes:

| Feature                  | Description                                                                           |
| ------------------------ | ------------------------------------------------------------------------------------- |
| ✅ Easy Setup             | Just include the CDN, no installation needed                                          |
| 💡 Responsive Design     | Built-in mobile-first design                                                          |
| 🧱 Predefined Components | Buttons, Cards, Modals, etc.                                                          |
| 🎨 Utility Classes       | Use class names like `text-center`, `bg-primary`, `p-3`, etc.                         |
| ⚙️ Requires JS           | Some components (like modals, carousels) need JavaScript (jQuery & Popper.js) to work |

---

## 🧪 Example: Bootstrap Button

```html
<button class="btn btn-primary">Click Me</button>
```

🔹 `btn` – Base button style
🔹 `btn-primary` – Blue button style

---

# 📐 Bootstrap Flexbox Utilities

---

## 1. Flex Container

* **`.d-flex`**: Defines a **Flexbox container**.
* **Flex items** are only the **direct children** of this container.

```html
<div class="d-flex">
  <div>…</div>       <!-- flex item -->
  <div>…</div>       <!-- flex item -->
</div>
```

> ❗️Make sure your elements are **wrapped** in `.d-flex` to apply any flex utilities.

---

## 2. Flex Direction

Controls the **main axis** (direction) of flex items.

| Class          | Direction  |
| -------------- | ---------- |
| `.flex-row`    | Horizontal |
| `.flex-column` | Vertical   |

* **Default**: `.flex-row` (items flow left‑to‑right).

```html
<div class="d-flex flex-column">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

## 3. Justify Content

Aligns flex items **along the main axis** (based on flex‑direction).

| Class                      | Effect                                   |
| -------------------------- | ---------------------------------------- |
| `.justify-content-start`   | Items at **start** (left or top)         |
| `.justify-content-center`  | Items at **center**                      |
| `.justify-content-end`     | Items at **end** (right or bottom)       |
| `.justify-content-between` | **Equal space** between items            |
| `.justify-content-around`  | Equal space **around** each item         |
| `.justify-content-evenly`  | Equal **space between and around** items |

```html
<div class="d-flex flex-row justify-content-between">
  <div>Left</div>
  <div>Center</div>
  <div>Right</div>
</div>
```

---

## 4. Align Items (Cross‑Axis)

Aligns flex items **perpendicular** to the main axis.

| Class                   | Effect                                |
| ----------------------- | ------------------------------------- |
| `.align-items-start`    | Align at **cross‑start** (top/left)   |
| `.align-items-center`   | Align at **center**                   |
| `.align-items-end`      | Align at **cross‑end** (bottom/right) |
| `.align-items-stretch`  | Stretch to **fill** container         |
| `.align-items-baseline` | Align on **text baselines**           |

```html
<div class="d-flex align-items-center" style="height:200px;">
  <div>Top</div>
  <div>Middle</div>
  <div>Bottom</div>
</div>
```

---

## 5. Flex Wrap

Controls whether items **wrap** onto multiple lines.

| Class                | Behavior                      |
| -------------------- | ----------------------------- |
| `.flex-wrap`         | Allow items to **wrap**       |
| `.flex-nowrap`       | **No wrap** (all on one line) |
| `.flex-wrap-reverse` | Wrap in **reverse** order     |

```html
<div class="d-flex flex-wrap">
  <div class="p-2">1</div>
  <div class="p-2">2</div>
  … more items …
</div>
```

---

## 6. Flex Grow / Shrink / Basis

| Class            | Effect                                             |
| ---------------- | -------------------------------------------------- |
| `.flex-grow-0`   | **Disable** growth (stay at base size)             |
| `.flex-grow-1`   | **Enable** growth (fill available space)           |
| `.flex-shrink-0` | **Disable** shrinking                              |
| `.flex-shrink-1` | **Enable** shrinking                               |
| `.flex-fill`     | **Flex-grow:1**, **flex-shrink:1**, **basis:100%** |

```html
<div class="d-flex">
  <div class="flex-fill">fills</div>
  <div>fixed</div>
</div>
```

---

## 📝 Quick Reference Table

| Utility                         | Purpose                  | Example                            |
| ------------------------------- | ------------------------ | ---------------------------------- |
| `.d-flex`                       | Define flex container    | `<div class="d-flex">…</div>`      |
| `.flex-row` / `.flex-column`    | Main-axis direction      | `.d-flex flex-column`              |
| `.justify-content-*`            | Main-axis alignment      | `.justify-content-center`          |
| `.align-items-*`                | Cross-axis alignment     | `.align-items-end`                 |
| `.flex-wrap` / `.flex-nowrap`   | Control wrapping         | `.d-flex flex-wrap`                |
| `.flex-grow-1` / `.flex-grow-0` | Enable/disable flex grow | `<div class="flex-grow-1">…</div>` |

---


# 🎨 Bootstrap Predefined Styles

---

## 1. 🔘 Buttons

### Basic Button

```html
<button class="btn">Submit</button>
```

### Colored Buttons

Use these with `.btn`:

| Class           | Appearance      |
| --------------- | --------------- |
| `btn-primary`   | Blue            |
| `btn-secondary` | Grey            |
| `btn-success`   | Green           |
| `btn-danger`    | Red             |
| `btn-warning`   | Yellow/Orange   |
| `btn-info`      | Teal/Light Blue |
| `btn-dark`      | Dark Grey       |
| `btn-light`     | Light Grey      |

### Outline Buttons

Replace `btn-` with `btn-outline-`:

```html
<button class="btn btn-outline-primary">Get Started</button>
```

> 🔔 `btn` alone has **no background color** by default.

---

## 2. 🎨 Text Colors

Apply with classes like:

```html
<h1 class="text-primary">Tourism</h1>
```

| Class            | Effect        |
| ---------------- | ------------- |
| `text-primary`   | Blue          |
| `text-secondary` | Grey          |
| `text-success`   | Green         |
| `text-danger`    | Red           |
| `text-warning`   | Orange/Yellow |
| `text-dark`      | Dark Grey     |
| `text-white`     | White         |

---

## 3. 🔠 Text Transform

| Class             | Effect               |
| ----------------- | -------------------- |
| `text-uppercase`  | UPPERCASE            |
| `text-lowercase`  | lowercase            |
| `text-capitalize` | Capitalize Each Word |

```html
<p class="text-capitalize">plan your trip wherever you want</p>
```

---

## 4. 🧱 Background Colors

Use on any HTML element:

```html
<div class="bg-success">Success Box</div>
```

| Class          | Color         |
| -------------- | ------------- |
| `bg-primary`   | Blue          |
| `bg-secondary` | Grey          |
| `bg-success`   | Green         |
| `bg-danger`    | Red           |
| `bg-warning`   | Yellow/Orange |
| `bg-info`      | Light Blue    |
| `bg-dark`      | Dark Grey     |
| `bg-white`     | White         |

---

## 5. 🧰 Other Common Utility Classes

| Class                    | Purpose                 |
| ------------------------ | ----------------------- |
| `card`, `card-body`      | For cards               |
| `carousel`               | For image sliders       |
| `alert`, `alert-success` | For alert messages      |
| `alert-link`             | Alert-styled hyperlinks |

---

## ⚠️ Warning

> Avoid using **Bootstrap class names as selectors in custom CSS**, e.g.,

```css
.btn { ... } /* ⚠️ May conflict with Bootstrap styles */
```

Instead, create your own class:

```css
.my-button { ... }
```

---


# 🖼️ Bootstrap Carousel Component

## ✅ What is it?

A **carousel** is a slideshow component for cycling through **images or content** — automatically or with user interaction.

---

## 🧩 Basic Structure

```html
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
  <!-- Indicators -->
  <ol class="carousel-indicators">
    <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
  </ol>

  <!-- Slides -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/tajmahal-c1-img.png" alt="Taj Mahal">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="IMAGE_URL_2" alt="...">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="IMAGE_URL_3" alt="...">
    </div>
  </div>

  <!-- Controls -->
  <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
  </a>
  <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
  </a>
</div>
```

---

## 🔁 Change Image

Change `src` attribute to your own image URL:

```html
<img class="d-block w-100" src="YOUR_IMAGE_URL" alt="description">
```

---

## 📌 Important Notes

### 1. Unique Carousel ID

If you're using **more than one carousel**, each must have a **unique ID**:

✅ Correct:

```html
<div id="carouselTajMahal" class="carousel slide" ...>
```

❌ Avoid:

```html
<div id="carouselExampleIndicators" ...> <!-- Used multiple times -->
```

### 2. Required Scripts

Ensure Bootstrap and jQuery are loaded for the carousel to function:

```html
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.2/dist/js/bootstrap.bundle.min.js"></script>
```

---

## 🛠️ Carousel Features Recap

| Feature                      | Description                           |
| ---------------------------- | ------------------------------------- |
| `carousel-inner`             | Holds all the slides                  |
| `carousel-item`              | Represents one slide                  |
| `active`                     | Class for the initially visible slide |
| `data-slide="prev"` / `next` | Navigation controls                   |
| `carousel-indicators`        | Dots for navigation                   |
| `data-ride="carousel"`       | Enables auto-sliding                  |

---


# 🎬 Bootstrap Video Embed Utility

## ✅ Purpose:

Embed responsive YouTube videos that maintain aspect ratio across screen sizes.

---

## 📦 Basic Embed Code:

```html
<div class="embed-responsive embed-responsive-16by9">
  <iframe
    class="embed-responsive-item"
    src="https://www.youtube.com/embed/49HTIoCccDY?rel=0"
    allowfullscreen
  ></iframe>
</div>
```

---

## 🎯 How to Add Your Own Video:

### Step 1: Get your YouTube Video ID

A YouTube video URL looks like:

```
https://www.youtube.com/watch?v=abc123XYZ
```

🔑 **Video ID = `abc123XYZ`**

### Step 2: Replace in `src`

Format it like this:

```
https://www.youtube.com/embed/abc123XYZ?rel=0
```

### ✅ Final Code:

```html
<div class="embed-responsive embed-responsive-16by9">
  <iframe
    class="embed-responsive-item"
    src="https://www.youtube.com/embed/abc123XYZ?rel=0"
    allowfullscreen
  ></iframe>
</div>
```

---

## 🔲 Change Video Size (Aspect Ratio):

| Aspect Ratio   | Class Name               |
| -------------- | ------------------------ |
| 16:9 (default) | `embed-responsive-16by9` |
| 1:1 (square)   | `embed-responsive-1by1`  |

### 📏 Example - Square Embed:

```html
<div class="embed-responsive embed-responsive-1by1">
  <iframe
    class="embed-responsive-item"
    src="https://www.youtube.com/embed/abc123XYZ?rel=0"
    allowfullscreen
  ></iframe>
</div>
```

---

## 📝 Notes & Warnings:

* ✅ **Use `embed-responsive` on the outer `div`**, and `embed-responsive-item` on the `iframe`.
* ⚠️ **Do not remove** the `?rel=0` if you want to **prevent YouTube from showing related videos** at the end.
* ⚠️ **Avoid typos** in the YouTube embed link. One wrong character can break the video.

---

# 💡 CCBP UI Kit Overview

The **CCBP UI Kit** is a collection of **reusable code snippets**—just like Bootstrap—but tailored for **CCBP training projects**. It helps you quickly add functionality and styles without writing much custom code.

---

## 1️⃣ How to Add CCBP UI Kit

To use it, insert the following in your HTML:

### ✅ In `<head>` (jQuery is required):

```html
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
  integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
  crossorigin="anonymous"></script>
```

### ✅ At the **end of `<body>`**:

```html
<script type="text/javascript"
  src="https://d1tgh8fmlzexmh.cloudfront.net/ccbp-static-website/js/ccbp-ui-kit.js">
</script>
```

### 📝 Why at the end?

Putting it before `</body>` ensures:

* Your page loads faster.
* The DOM is fully loaded before the script runs.

---

## 2️⃣ Display Utility

The **Display Utility** in CCBP UI Kit helps:

* Show or hide elements (like sections, modals, menus) based on user actions (clicks, toggles, etc).

### ✅ Typical Usage:

You can use helper methods like:

```javascript
displayElement("sectionId");      // Shows the element with given id
hideElement("sectionId");         // Hides it
toggleDisplay("sectionId");       // Toggles visibility
```

These are usually triggered by event listeners (like button clicks).

### 📌 Example:

```html
<button onclick="displayElement('infoSection')">Show Info</button>
<button onclick="hideElement('infoSection')">Hide Info</button>

<div id="infoSection" style="display: none;">
  <p>This is a hidden section revealed by CCBP UI Kit.</p>
</div>
```

---

## ✅ Summary

| Feature         | Description                                            |
| --------------- | ------------------------------------------------------ |
| UI Kit Source   | Hosted by CCBP CloudFront (JS file)                    |
| jQuery Required | Yes (must load before the UI Kit script)               |
| Display Utility | `displayElement()`, `hideElement()`, `toggleDisplay()` |

---

## 🔗 1. Getting Image URLs with Cloudinary

**Cloudinary** is a free cloud-based image and video hosting service. You can:

* Upload images from your computer.
* Get a **hosted URL** to use in your HTML/CSS.

### ✅ Use Cases:

* For `<img>` tags:

  ```html
  <img src="https://res.cloudinary.com/your-cloud/image/upload/v12345/your-image.jpg" />
  ```

* For CSS background images:

  ```css
  .banner {
    background-image: url("https://res.cloudinary.com/your-cloud/image/upload/v12345/your-image.jpg");
  }
  ```

🔗 [Visit Cloudinary](https://cloudinary.com/) to sign up and upload images.

---

## 💻 2. Install Visual Studio Code

**VS Code** is a lightweight and powerful source code editor. It's free and available on all major OS.

### Video Duration Tips:

* **Windows**: Full walkthrough
* **Ubuntu/Linux**: Watch \~2 mins
* **Mac**: Watch \~2.5 mins

Once installed, open a folder/project, create your `index.html` and `style.css`, and start coding.

---

## 📎 3. Linking HTML and CSS

Always **link your CSS file** inside the `<head>` of your HTML document:

```html
<head>
  <link rel="stylesheet" href="tourism.css">
</head>
```

✅ This ensures your page loads with the correct styles from the start.

---

## 🖼️ 4. HTML `<img>` vs CSS `background-image`

| Use HTML `<img>`                            | Use CSS `background-image`                 |
| ------------------------------------------- | ------------------------------------------ |
| Image is **part of content** (like a photo) | Image is **decorative** or behind elements |
| No content layered on top                   | Has content layered (like text or buttons) |
| Easier for SEO/accessibility                | Better for layout/styling                  |

### Example:

* **HTML image**:

  ```html
  <img src="cloudinary-url.jpg" alt="Taj Mahal">
  ```

* **CSS background image**:

  ```css
  .hero {
    background-image: url("cloudinary-url.jpg");
    background-size: cover;
    height: 300px;
  }
  ```

---

## 📏 5. CSS Margin vs Padding

| Property    | Use Case                                                   |
| ----------- | ---------------------------------------------------------- |
| **Padding** | Space **inside** the element (between content and border)  |
| **Margin**  | Space **outside** the element (between element and others) |

### Example:

```css
.button {
  padding: 20px;  /* space inside the button */
  margin: 15px;   /* space around the button */
}
```

🧠 **Tip**: Think of `padding` as "internal spacing" and `margin` as "external spacing".

---

