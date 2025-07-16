## 🎯 Specificity Practice-5

**Solved**
**Difficulty:** Easy

---

### 📝 Assignment Objective

Apply **CSS Specificity** concepts to style paragraphs using type, class selectors, and `!important`.

---

### 📌 Instructions

1. **Add CSS class** `blue-bg` to the **last two paragraphs** to change their background to `dodgerblue`.
2. **Also add CSS class** `orange-bg` to the **last paragraph** to override the previous color with `orange` using `!important`.

---

### ✅ Provided CSS (Do NOT modify it)

```css
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");

p {
  color: white;
  background-color: grey;
  font-family: "Roboto";
  padding: 10px;
}

.blue-bg {
  background-color: dodgerblue;
}

.orange-bg {
  background-color: orange !important;
}
```

---

### ✅ Final HTML Code

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>This is the first paragraph.</p>
    <p class="blue-bg">This is the second paragraph.</p>
    <p class="blue-bg orange-bg">This is the third paragraph.</p>
  </body>
</html>
```

---

### 💡 Explanation

- All paragraphs start with a default grey background from the `p` selector.
- The last two are given `blue-bg`, which changes them to **dodgerblue**.
- The very last paragraph also gets `orange-bg`, which overrides the `blue-bg` due to `!important`.
