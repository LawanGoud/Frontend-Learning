# Specificity Practice - 1

## 🎯 1. Goal

To build a personal profile section using **CSS specificity concepts**:

- Apply correct styles without editing the CSS.
- Match the design shown in the provided image.
- Understand and use tag, class selectors, and the cascade properly.

---

## 📚 2. Content Used

### ✅ CSS Concepts Covered:

| Concept                    | What I Applied                                                                   |
| -------------------------- | -------------------------------------------------------------------------------- |
| **Specificity**            | Class selectors override tag selectors                                           |
| **Tag Selectors**          | Global `h1`, `p` styles used when no class is present                            |
| **Class Selectors**        | Used `.designation-details`, `.contact-info` etc., to apply more specific styles |
| **Cascade (Order)**        | Later styles in CSS are applied if specificity is the same                       |
| **Separation of Concerns** | HTML for content, CSS for styling                                                |

### ✅ CSS Classes Provided:

- `.profile-container` – outer wrapper
- `h1` – global heading style
- `.designation-details-container` – wraps title + description
- `.designation-details` – title only
- `p` – default paragraph
- `.contact-info-container` – wraps contact info
- `.contact-info` – italic contact text

---

## 🛠 3. Solving

### ✅ Step 1: HTML Structure

Create the main container with class:

```html
<div class="profile-container">
  <!-- Inside content goes here -->
</div>
```

---

### ✅ Step 2: Heading (Name)

Use a simple `<h1>` — styled by tag selector in CSS.

```html
<h1>Rahul</h1>
```

---

### ✅ Step 3: Job Role & Description

Wrap the next two lines inside `.designation-details-container`.

- For "FRONT END DEVELOPER", use `.designation-details` for stronger specificity.
- The second paragraph will use the default `p` tag style, which is different.

```html
<div class="designation-details-container">
  <p class="designation-details">FRONT END DEVELOPER</p>
  <p>
    I am a Front-End Developer with an year of work experience across the
    product development life cycle.
  </p>
</div>
```

---

### ✅ Step 4: Contact Information

Use `.contact-info-container` with a paragraph inside having `.contact-info` for font-style (italic) and color.

```html
<div class="contact-info-container">
  <p class="contact-info">Send me an Email to get access to my work.</p>
</div>
```

---

## 💡 4. Final Code

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="profile-container">
      <h1>Rahul</h1>

      <div class="designation-details-container">
        <p class="designation-details">FRONT END DEVELOPER</p>
        <p>
          I am a Front-End Developer with an year of work experience across the
          product development life cycle.
        </p>
      </div>

      <div class="contact-info-container">
        <p class="contact-info">Send me an Email to get access to my work.</p>
      </div>
    </div>
  </body>
</html>
```

---

## 📘 5. What I Learned

- How **specificity** helps browsers decide which styles to apply.
- **Class selectors override tag selectors** without needing `!important`.
- **Cascade** plays a role when specificity is equal.
- Importance of writing **clean, reusable HTML and CSS** by separating responsibilities.
- Applied styles accurately **without modifying any CSS** – only using structure and class names.

---
