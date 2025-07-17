Let's build the **VR Website Optics and Controllers Section** step by step using the provided instructions and reference images.

---

## ✅ Objective

Create a responsive **VR Optics and Controllers Section** with two major parts:

1. **Optics** (Image on left, text on right)
2. **Controllers** (Image on right, text on left)

---

## 🧱 Step-by-Step Implementation

---

### 🖼️ **Step 1: HTML Structure**

```html
<div class="vr-features-section">
  <!-- Optics Section -->
  <div class="feature-item">
    <img
      src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-optics-img.png"
      alt="VR Optics"
      class="feature-img"
    />
    <div class="feature-text">
      <h1 class="feature-heading">Improved Optics</h1>
      <p class="feature-description">
        A virtual reality headset is a head-mounted device that provides virtual
        reality for the wearer.
      </p>
      <button class="feature-button">Read More</button>
    </div>
  </div>

  <!-- Controllers Section -->
  <div class="feature-item reverse">
    <img
      src="https://d2clawv67efefq.cloudfront.net/ccbp-responsive-website/vr-controllers-img.png"
      alt="VR Controllers"
      class="feature-img"
    />
    <div class="feature-text">
      <h1 class="feature-heading">Two Touch Controllers</h1>
      <p class="feature-description">
        Your Oculus Touch controllers are a pair of tracked controllers that
        give you hand presence—the feeling that your virtual hands are actually
        your own.
      </p>
      <button class="feature-button">Read More</button>
    </div>
  </div>
</div>
```

---

### 🎨 **Step 2: CSS Styling**

```css
.vr-features-section {
  background-color: #1a2137;
  padding: 40px 20px;
}

.feature-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 40px;
}

.feature-img {
  width: 100%;
  max-width: 400px;
}

.feature-text {
  text-align: center;
  padding-top: 20px;
}

.feature-heading {
  color: #ffffff;
  font-size: 24px;
  margin-bottom: 10px;
}

.feature-description {
  color: #7b8794;
  font-size: 16px;
  margin-bottom: 20px;
  max-width: 500px;
}

.feature-button {
  background-color: #ffffff;
  color: #1f2933;
  border: none;
  padding: 10px 20px;
  font-weight: bold;
  border-radius: 5px;
  cursor: pointer;
}

.reverse {
  flex-direction: column-reverse;
}

/* Responsive styling */
@media screen and (min-width: 768px) {
  .feature-item {
    flex-direction: row;
    justify-content: space-between;
    text-align: left;
  }

  .feature-text {
    flex: 1;
    padding: 0 20px;
  }

  .feature-img {
    flex: 1;
    max-width: 50%;
  }

  .reverse {
    flex-direction: row-reverse;
  }
}
```

---

## 🧪 What You'll See

- On **mobile**, images stack above/below text.
- On **tablet and desktop**, layout becomes side-by-side:

  - **First section:** image left, text right.
  - **Second section:** text left, image right.

- Fully **responsive**, aligned with the visual reference.
- Buttons styled clearly and legibly.

---

Would you like this code exported into a `.zip` or hosted in a sandbox for live testing?
