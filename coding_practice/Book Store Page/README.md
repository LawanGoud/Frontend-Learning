# 📚 Book Store Page – Notes

## ✅ Goal

Build an interactive **Book Store** webpage using:

* HTML
* CSS
* Bootstrap (for layout and responsiveness)
* CCBP UI Kit for transitions and styling

---

## 📌 Functional Requirements

1. **Home Page** with:

   * One **Popular Book**
   * Two **Recommended Books**
   * `Read Now` button for each book leading to respective details page

2. **Book Details Pages**:

   * `Wings of Fire`
   * `The 3 Mistakes of My Life`
   * `Harry Potter`
   * Each has:

     * Book image
     * Title, Author
     * Description
     * `Back` and `Buy Now` buttons

3. **Navigation** via `onclick="display(...)"` function (from CCBP UI Kit).

---

## 🚨 Guidelines

* ✅ All section IDs must **start with `section`**, e.g., `sectionBookStoreHome`.
* ⚠️ Avoid assigning **Bootstrap flex properties to sections directly**.

  * ✅ Good: `<div id="sectionBookStoreHome">`
  * ❌ Bad: `<div id="sectionBookStoreHome" class="d-flex">`

---

## 🖼️ Image Assets

| Book                      | Image URL                                                                              |
| ------------------------- | -------------------------------------------------------------------------------------- |
| Wings of Fire             | `https://d2clawv67efefq.cloudfront.net/ccbp-static-website/book-apj-img.png`           |
| The 3 Mistakes of My Life | `https://d2clawv67efefq.cloudfront.net/ccbp-static-website/book-chetan-bhagat-img.png` |
| Harry Potter              | `https://d2clawv67efefq.cloudfront.net/ccbp-static-website/harrypotter-img.png`        |

---

## 🎨 Styling & Design

### 🎨 Colors

* Background: `#1b1b1b` (Dark gray/black)
* Text:

  * White: `#ffffff`
  * Subhead: `#183b56`, `#9aa5b1`, `#e4e7eb`
  * Popular Book BG: `#e6f6ff`

### 🖋️ Fonts

* `Bree Serif` – For headings and book titles
* `Roboto` – For button text

### 📐 Layouts

#### Home Page

* Header: `Popular Book`
* Card layout for:

  * Popular Book
  * Recommended Books (two stacked rows)

#### Book Details Page

* Center-aligned image and text
* Description aligned left
* Two buttons at bottom:

  * `Back` (returns to homepage)
  * `Buy Now`

---

## 🧩 Components

### HTML Sections

```html
<div id="sectionBookStoreHome">...</div>
<div id="sectionWingsOfFireBookDetails">...</div>
<div id="sectionTheThreeMistakesOfMyLifeBookDetails">...</div>
<div id="sectionHarryPotterBookDetails">...</div>
```

### Buttons

```html
<button class="button btn btn-primary" onclick="display('sectionXYZ')">Read Now</button>
<button class="button btn btn-warning" onclick="display('sectionBookStoreHome')">Back</button>
```

---

## 💡 Tips

* Use **Bootstrap Grid** and `d-flex flex-row` for horizontal layouts.
* Use **margins and padding** to space content properly.
* Ensure images are appropriately sized (`width`, `height` fixed).
* Use `display()` function from CCBP UI Kit for page transitions.

---

