## ✅ **1. Bootstrap Flex Utilities**

### 1.1 `order-*`

- Changes the **visual display order** of flex items.
- `order-0` to `order-12`
- Can be used responsively:
  e.g., `order-1 order-md-2 order-lg-3`

#### ✅ Example:

```html
<div class="d-flex">
  <div class="order-3">First in DOM, last visually</div>
  <div class="order-2">Second visually</div>
  <div class="order-1">First visually</div>
</div>
```

---

## ✅ **2. Bootstrap Display Utilities**

### `d-*` classes control visibility and display type.

- **Hide/show elements** responsively:

  - `d-none`, `d-sm-none`, `d-md-none`, etc.

- **Force display type**:

  - `d-block`, `d-md-inline`, `d-lg-inline-block`, etc.

#### ✅ Example:

```html
<p class="d-none d-md-block">Visible only on md and above</p>
<a class="d-md-none d-lg-inline">Visible below md & inline above lg</a>
```

---

## ✅ **3. Food Munch Sections**

These sections use **responsive Bootstrap grids + utility classes**:

---

### 🍎 **Healthy Food Section**

- **Image left on md+**, **above text on mobile**
- Uses:

  - `col-12 col-md-5` for responsive image
  - Utility classes for spacing (`pt-5`, `pb-5`)

---

### 🚚 **Delivery & Payment Section**

- Image is **after** text on desktop (`order-md-2`), **above** text on mobile (`order-1`)
- `order-*` lets you **reorder columns** without changing HTML order

---

### 🎁 **Thanking Customers Section**

- Shows **image above** text on mobile, **to the right** on desktop
- Uses:

  - `d-md-none` and `d-none d-md-block` to toggle image placement
  - `flex-column justify-content-center` to center content vertically

---

## 💡 Key Takeaways

- `order-*` is for reordering **flex items**
- `d-*` is for controlling **visibility and display types**
- Combine with **Bootstrap Grid (col-\*)** to make fully responsive layouts
- Very useful in **mobile-first** designs like Food Munch

---
