# Specificity Practice - 2

---

## 🎯 1. Goal

Build a To-Do list using **CSS specificity**:

- Apply styles using **IDs**, **classes**, and **tag selectors**.
- Match the visual output exactly as shown in the reference image.
- Do **not edit** the provided CSS — only use appropriate HTML structure and attributes.

---

## 📚 2. Content Used

### ✅ CSS Concepts Practiced

| Concept                    | What I Applied                                              |
| -------------------------- | ----------------------------------------------------------- |
| **ID Selectors**           | `#todayHeading` — more specific than class or tag           |
| **Class Selectors**        | `.completed` used for crossed-out and italic list items     |
| **Tag Selectors**          | `li`, `h1` for global list/item styling                     |
| **Font Styling**           | `font-style: italic`, `text-decoration: line-through`, etc. |
| **Separation of Concerns** | Structure in HTML, styles in CSS                            |

---

## 🛠 3. Solving

### ✅ Step 1: Create Container

Wrap everything inside `.todo-list-container`:

```html
<div class="todo-list-container">
  <!-- Inner content here -->
</div>
```

---

### ✅ Step 2: Main Heading

Add a top-level `<h1>` for "TodoList":

```html
<h1>TodoList</h1>
```

---

### ✅ Step 3: Today Section

Use a `<h1>` with an `id="todayHeading"` to get **blue color**.

Then list items in `<ul>` with `li`, and apply `.completed` to done tasks:

```html
<h1 id="todayHeading">Today</h1>
<ul>
  <li>Have a Drink</li>
  <li class="completed">Go for a Walk</li>
  <li>Read a book</li>
  <li class="completed">Schedule Meeting with Alex</li>
</ul>
```

---

### ✅ Step 4: Tomorrow Section

Use normal `<h1>` (black by default via tag selector), then a list with no `.completed` classes:

```html
<h1>Tomorrow</h1>
<ul>
  <li>Listen to the Video Session</li>
  <li>Attempt Practice questions</li>
  <li>Go for Shopping</li>
  <li>Read Monthly Magazine</li>
</ul>
```

---

## 💡 Final Code

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="todo-list-container">
      <h1>TodoList</h1>

      <h1 id="todayHeading">Today</h1>
      <ul>
        <li>Have a Drink</li>
        <li class="completed">Go for a Walk</li>
        <li>Read a book</li>
        <li class="completed">Schedule Meeting with Alex</li>
      </ul>

      <h1>Tomorrow</h1>
      <ul>
        <li>Listen to the Video Session</li>
        <li>Attempt Practice questions</li>
        <li>Go for Shopping</li>
        <li>Read Monthly Magazine</li>
      </ul>
    </div>
  </body>
</html>
```

---

## 🔍 5. What I Learned

- **ID selectors** override class and tag styles.
- Applying `.completed` class changes multiple CSS properties.
- How **HTML structure** interacts with predefined styles.
- Used only existing CSS styles to achieve the output, reinforcing the power of **CSS specificity**.

---

```

```
