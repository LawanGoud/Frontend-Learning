
# 📘 **Introduction to HTML**

## ✅ **Basic Structure of an HTML Document**

**What to Learn:**
Understand how an HTML page is laid out using standard tags.

**Key Tags:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Web Page</title>
  </head>
  <body>
    <!-- All content goes here -->
  </body>
</html>
```

**Explanation:**

* `<!DOCTYPE html>` tells the browser you're using HTML5.
* `<html>` is the root element.
* `<head>` contains metadata like `<title>`, links to CSS, etc.
* `<body>` is where all visible content goes.

---

## ✅ **Heading Element**

**What to Learn:**
Headings define the hierarchy and structure of content on the page.

**Tags:**
`<h1>` to `<h6>`

**Example:**

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Smaller Heading</h3>
```

**Tip:** Use only one `<h1>` per page for accessibility and SEO.

---

## ✅ **Paragraph Element**

**What to Learn:**
Paragraphs are blocks of text used to display readable content.

**Tag:**
`<p>`

**Example:**

```html
<p>This is a simple paragraph explaining a concept.</p>
```

**Note:** HTML ignores multiple spaces and line breaks inside a paragraph by default.

---

## ✅ **Button Element**

**What to Learn:**
Buttons are used for user interaction, like submitting forms or triggering events.

**Tag:**
`<button>`

**Example:**

```html
<button>Click Me</button>
```

**Attributes to Explore:**

* `type="button"` or `type="submit"`
* `disabled`
* Inline event: `onclick="alert('Hello!')"`

