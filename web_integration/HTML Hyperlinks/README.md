# HTML Anchor Element Notes

## 1. HTML `<a>` Anchor Element

The HTML `<a>` element defines a **Hyperlink**.  
We use **Hyperlinks** to navigate to other web resources or to a specific element within the HTML document.  
They are also called _links_.

### Syntax:
```html
<a href="URL">Content</a>
````

---

### 1.1 `href` Attribute

The `href` attribute specifies the URL/path of the page where the link goes to.

Example:

```html
<a href="https://www.ccbp.in/">Explore CCBP 4.0 Certification Programs</a>
```

---

### 1.2 `target` Attribute

The `target` attribute specifies where to open the linked web resource.

* `_blank`: Opens the link in a new tab.

Example:

```html
<a href="https://www.ccbp.in/" target="_blank">Explore CCBP 4.0 Certification Programs</a>
```

---

## 2. Navigate Within the Same HTML Document

The HTML `<a>` element can also be used to navigate to different sections within the same HTML document.

### Steps:

1. Add an `id` attribute to the section you want to navigate to.
2. Use `#id` in the anchor tag’s `href`.

Example:

```html
<a href="#bioSection">Bio</a>

<!-- Somewhere in the document -->
<div id="bioSection">
  <h1>Bio</h1>
  <p>Vinod is an Indian-American business executive...</p>
</div>
```

---

## 3. Hyperlinked Image

Images can also be used as hyperlinks:

```html
<a href="https://www.ccbp.in/">
  <img src="https://d2clawv67efefq.cloudfront.net/ccbp-static-website/learn-technologies-img.png" />
</a>
```

---

## 4. Sample HTML Page

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Twinkle Poem</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1 class="heading">Twinkle Twinkle Little Star</h1>
    <hr />
    <p>
      Twinkle, twinkle, little star, <br />
      How I wonder what you are! <br />
      Up above the world so high, <br />
      Like a diamond in the sky.
    </p>
    <hr />
  </body>
</html>
```

---

## 5. Basic CSS Styles

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,700&display=swap");

.profile {
  text-align: center;
  background-color: #ffffff;
  padding: 30px;
}

.image {
  width: 200px;
  margin: 30px;
}

.heading {
  font-size: 24px;
  font-weight: bold;
}
```


## 6. Most Commonly Used HTML Void Elements

Void elements are HTML elements that **do not have a closing tag**. They are self-contained and typically affect the document structure or layout.

---

### 6.1 HTML `<br>` – Line Break Element

The `<br>` element is used to insert a **line break** in text.  
It forces the text to continue on the **next line**.

#### Example:
```html
<p>
  Twinkle, twinkle, little star, <br />
  How I wonder what you are!
</p>
````

---

### 6.2 HTML `<hr>` – Horizontal Rule Element

The `<hr>` element inserts a **horizontal line**, often used to separate content or sections visually.

#### Example:

```html
<p>Section One</p>
<hr />
<p>Section Two</p>
```

---

These void elements are especially useful for formatting and structuring content in HTML pages.



---

## Summary

* Use `<a href="URL">Text</a>` for links.
* Use `target="_blank"` to open in a new tab.
* Use `href="#id"` to navigate within the same page.
* You can hyperlink images using `<a>` tag.
* Combine HTML with CSS for styling.


