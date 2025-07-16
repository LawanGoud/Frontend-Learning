## 1. ✅ **Bootstrap Spacing Utilities**

Bootstrap provides utility classes to quickly set padding and margin using a consistent spacing scale.

### 1.1 🔹 **Padding Classes**

| CSS Property     | Bootstrap Class |
| ---------------- | --------------- |
| `padding`        | `p-*`           |
| `padding-top`    | `pt-*`          |
| `padding-right`  | `pr-*`          |
| `padding-bottom` | `pb-*`          |
| `padding-left`   | `pl-*`          |

---

### 1.1.1 📏 **Padding Size Values**

| Size Class | Multiplier | Calculation (with spacer = 16px) | Value in px |
| ---------- | ---------- | -------------------------------- | ----------- |
| 0          | 0          | 0 × 16px                         | `0px`       |
| 1          | 0.25       | 0.25 × 16px                      | `4px`       |
| 2          | 0.5        | 0.5 × 16px                       | `8px`       |
| 3          | 1          | 1 × 16px                         | `16px`      |
| 4          | 1.5        | 1.5 × 16px                       | `24px`      |
| 5          | 3          | 3 × 16px                         | `48px`      |

📝 Example usage:

```html
<div class="pt-4 pb-2 pl-3 pr-5">...</div>
```

---

## 2. ✅ **HTML `<span>` Element**

- The `<span>` tag is an **inline container** for text.
- Used **only for styling or marking a part** of the text.
- Does **not add line breaks**.

### 📌 Use Case:

```html
<p>Get discount up to <span class="offers">50% OFF</span> on all products!</p>
```

### ✨ CSS Styling:

```css
.offers {
  color: #323f4b;
  font-style: italic;
  font-weight: 600;
}
```

---

## 3. ✅ **Real-World Component Example: Why Choose Us Section**

### 🧩 HTML Structure:

- Uses Bootstrap `container`, `row`, and `col` for layout
- `p-*` classes for spacing
- Three feature cards using `.col-md-4`

### 📦 Key Bootstrap Classes Used:

| Element           | Class Used        | Purpose                  |
| ----------------- | ----------------- | ------------------------ |
| Section container | `pt-5 pb-5`       | Adds vertical spacing    |
| Column layout     | `col-12 col-md-4` | Responsive grid system   |
| Card padding      | `p-3 mb-3`        | Inner spacing and margin |
| Title spacing     | `mt-3`            | Margin above title       |

---

## 🎨 Custom CSS Summary

| Class                      | Purpose                                        |
| -------------------------- | ---------------------------------------------- |
| `.wcu-section`             | Background color for the section               |
| `.wcu-section-heading`     | Section title style (color, size, weight)      |
| `.wcu-section-description` | Subtitle styling                               |
| `.wcu-card`                | Card appearance with borders and border-radius |
| `.wcu-card-title`          | Card title color and font settings             |
| `.wcu-card-description`    | Card paragraph text style                      |
| `.wcu-card-image`          | Image size control                             |
| `.offers`                  | Inline span style (color, italic, bold)        |

---

## 🧪 Practical Example of Spacing

```html
<div class="wcu-section pt-5 pb-5">
  <div class="container">
    <div class="row">
      <div class="col-12 col-md-4">
        <div class="wcu-card p-3 mb-3">
          <!-- Content Here -->
        </div>
      </div>
    </div>
  </div>
</div>
```

🔍 Analysis:

- `pt-5 pb-5` adds 48px top and bottom padding
- `p-3` adds 16px padding inside the card
- `mb-3` adds 16px margin-bottom for spacing between rows

---

## 📚 Summary

| Topic                     | Key Takeaways                                   |
| ------------------------- | ----------------------------------------------- |
| Bootstrap Padding Classes | Use `p-`, `pt-`, `pl-`, etc., with values 0–5   |
| Padding Calculation       | Multiplier × 16px (default spacer)              |
| HTML `<span>` Element     | Used for inline styling without breaking layout |
| Real-world Example        | Bootstrap grid + spacing + custom CSS           |

---
