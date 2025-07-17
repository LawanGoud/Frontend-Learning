### ✅ **Goal**

Create a responsive "Included VR Kit" section with:

- A heading: **"Included VR Kit"**
- Three items:

  1. Two Touch Controllers
  2. VR Headset
  3. Charging Cable

---

## 🔧 Step-by-Step Implementation

---

### 🧱 **Step 1: HTML Structure**

```html
<div class="vr-kit-section">
  <h1 class="section-heading">Included VR Kit</h1>
  <div class="vr-kit-container">
    <div class="vr-kit-item">
      <img
        src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-kit-1-img.png"
        alt="Two Touch Controllers"
        class="vr-kit-img"
      />
      <p class="kit-description">Two Touch Controllers</p>
    </div>
    <div class="vr-kit-item">
      <img
        src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-kit-2-img.png"
        alt="VR Headset"
        class="vr-kit-img"
      />
      <p class="kit-description">VR Headset</p>
    </div>
    <div class="vr-kit-item">
      <img
        src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-kit-3-img.png"
        alt="Charging Cable"
        class="vr-kit-img"
      />
      <p class="kit-description">Charging Cable</p>
    </div>
  </div>
</div>
```

---

### 🎨 **Step 2: CSS Styling**

```css
/* Base styles */
.vr-kit-section {
  background-color: #f9fbfe;
  padding: 30px 20px;
  text-align: center;
}

.section-heading {
  color: #1f2933;
  font-size: 24px;
  font-weight: 600;
  margin-bottom: 30px;
}

/* Kit container layout */
.vr-kit-container {
  display: flex;
  flex-direction: column;
  gap: 30px;
}

/* Each kit item */
.vr-kit-item {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.vr-kit-img {
  width: 100%;
  max-width: 200px;
  height: auto;
}

.kit-description {
  font-size: 18px;
  color: #323f4b;
  margin-top: 15px;
}

/* Responsive layout */
@media screen and (min-width: 768px) {
  .vr-kit-container {
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
  }

  .vr-kit-item {
    flex: 1;
    padding: 0 10px;
  }
}
```

---

### 🧪 Result

**On Small Devices (Mobile/Tablets):**

- Stack items vertically.

**On Medium and Larger Devices:**

- Display items horizontally in a single row.

---

### 📌 Notes

- Fonts/colors match the image references (`#1f2933`, `#323f4b`, `#f9fbfe`)
- Fully responsive using **Flexbox**
- Simple structure: easy to expand or integrate

---
