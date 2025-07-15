# Specificity Practice - 4

---

## 🎯 1. Goal

To practice CSS specificity by styling different elements using:

- Type selector
- Class selector
- ID selector
- Inline styles

While doing this:

- Use a **type selector** to style the container.
- Use a **class selector** to color the heading text.
- Use an **ID selector** to resize paragraph text.
- Use **inline style** to set button background.

---

## 📚 2. Content Used

| Selector Type  | Usage                                             | Specificity |
| -------------- | ------------------------------------------------- | ----------- |
| Type Selector  | `.language-container` via `div` tag               | `0,0,0,1`   |
| Class Selector | `.blue-text` on `<h1>`                            | `0,0,1,0`   |
| ID Selector    | `#description` on `<p>`                           | `0,1,0,0`   |
| Inline Style   | `style="background-color: orange;"` on `<button>` | `1,0,0,0`   |

**Specificity hierarchy (↑ higher priority):**
Inline Style > ID > Class > Type

---

## 🛠 3. Solving

### ✅ Step-by-Step Plan

1. Wrap all content inside a `div` with the class `language-container` (type selector for container styles).
2. Use an `<h1>` tag with the class `blue-text` for the main heading.
3. Use a `<p>` tag with the `id="description"` to apply ID-based font size.
4. Add a `<button>` element with an **inline style** to override its background color.

---

## 💡 Final HTML Code

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="language-container">
      <h1 class="blue-text">HTML</h1>
      <p id="description" class="language-description">
        HTML is a Standard Markup Language for creating Web pages.
      </p>
      <button style="background-color: orange;">Learn</button>
    </div>
  </body>
</html>
```

---

## 🎨 CSS Code (already provided)

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");

.language-container {
  background-color: lightgray;
  text-align: center;
  font-family: "Roboto";
  padding: 40px;
}

.blue-text {
  color: blue;
}

h1 {
  color: orange;
  font-size: 30px;
  font-weight: bold;
}

.language-description {
  font-size: 16px;
}

#description {
  font-size: 20px;
}

button {
  width: 100px;
  height: 30px;
  border-width: 0px;
  border-radius: 5px;
}
```

---

## 🧠 4. What I Learned

- **Type selectors** are the most basic, with the least specificity.
- **Class selectors** override type styles.
- **ID selectors** override class and type selectors.
- **Inline styles** override everything in the CSS file.
- Best practice is to avoid inline styles unless necessary; this task was purely for understanding specificity.

---

```

```
