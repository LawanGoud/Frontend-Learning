# Specificity Practice - 3

---

## 🎯 1. Goal

To build a webpage using only the **provided CSS styles**, showcasing the use of **type selectors** and **ID selectors**, and their specificity in CSS.

The webpage should display three `<p>` elements:

1. Two paragraphs using **type selector styles**.
2. One paragraph in the middle using an **ID selector** to override type styles.

---

## 📚 2. Content Used

| CSS Feature      | Description                                                                 |
| ---------------- | --------------------------------------------------------------------------- |
| `p` selector     | Targets all `<p>` tags with general styles (background, font, padding)      |
| `#dark` selector | Targets a specific paragraph by ID, overrides the background and text color |
| Specificity Rule | ID selectors override type selectors (higher specificity)                   |

### 🧠 CSS Specificity Rule Recap

- Type Selector (`p`) → Specificity: `0,0,0,1`
- ID Selector (`#dark`) → Specificity: `0,1,0,0`
- So, `#dark` wins over the `p` selector if both apply.

---

## 🛠 3. Solving

### ✅ Step-by-Step Plan

1. Use `<p>` elements to display the required texts.
2. Apply **type selector** styles by default.
3. Apply `id="dark"` to the **middle paragraph** to override the default.
4. Keep the structure clean and semantic.

---

## 💡 Final HTML Code

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>A paragraph with the type selector</p>
    <p id="dark">A paragraph with the ID selector</p>
    <p>A paragraph with the type selector</p>
  </body>
</html>
```

---

## 🎨 CSS Code (already provided, do not change)

```css
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");

p {
  background-color: #f3e1cd;
  font-family: "Open Sans";
  font-size: 22px;
  padding: 25px;
  margin: 0px;
}

#dark {
  background-color: black;
  color: white;
}
```

---

## 📌 4. What I Learned

- **CSS specificity** decides which rule applies when multiple rules target the same element.
- **ID selectors override type selectors** due to higher specificity.
- Even if multiple rules apply, styles from more specific selectors will **override less specific ones**.
- It's better to **re-use common styles** and override only where necessary using selectors like `#id`.

---
