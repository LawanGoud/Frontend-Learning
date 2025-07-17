### ✅ **1. Goal**

Build a **responsive "Features" section** for a VR website using **Bootstrap grid system**, responsive breakpoints, and HTML/CSS concepts.

---

### ✅ **2. Content Used / Concepts Applied**

- ✅ Bootstrap Grid System (`container`, `row`, `col-*`)
- ✅ Responsive column sizes (`col-12`, `col-md-6`, `col-lg-4`)
- ✅ Images with `img-fluid` for responsiveness
- ✅ Font and color styling using custom CSS
- ✅ Mobile-first design
- ✅ Spacing utilities: `pt-5`, `mb-3`, etc.

---

### ✅ **3. Solving Steps (Implementation)**

#### ✅ Step 1: HTML Skeleton

```html
<div class="features-section pt-5 pb-5">
  <div class="container">
    <div class="row">
      <div class="col-12 text-center">
        <h1 class="features-heading">Features</h1>
      </div>
    </div>
    <div class="row">
      <!-- Feature Cards Go Here -->
    </div>
  </div>
</div>
```

#### ✅ Step 2: Create Each Feature Card

```html
<div class="col-12 col-md-6 col-lg-4 text-center mb-4">
  <img src="FEATURE_IMAGE_URL" class="feature-img img-fluid mb-3" />
  <h5 class="feature-title">Feature Title</h5>
  <p class="feature-description">Description about the feature.</p>
</div>
```

➡️ Repeat this for all **6 features**, using appropriate images and text.

---

### ✅ **4. Replace with Actual Content**

| Feature Title      | Image URL               | Description                                                                                            |
| ------------------ | ----------------------- | ------------------------------------------------------------------------------------------------------ |
| Easy to connect    | `easy-connect-img.png`  | Instead of viewing a screen in front of them, users are immersed and able to interact with 3D worlds.  |
| VR Capability      | `vr-capability-img.png` | Virtual reality (VR) can create an environment similar to or completely different from the real world. |
| Video games        | `video-games-img.png`   | Ability to recognize hand motion, evolving interactions and gameplay in VR.                            |
| Interaction        | `interaction-img.png`   | Interaction refers to the <b>natural interaction</b> between the user and the virtual scene.           |
| Easy to play       | `easy-play-img.png`     | In 360-degree video, the locations of viewers are fixed, viewers are limited to the angles captured.   |
| Awesome Experience | `experience-img.png`    | VR is a simulated experience that can be similar to or completely different from the real world.       |

---

### ✅ **5. CSS Styling**

```css
.features-heading {
  color: #1f2933;
  font-size: 28px;
  font-family: "Roboto";
  font-weight: 700;
}

.feature-img {
  width: 90px;
  height: 90px;
}

.feature-title {
  font-size: 20px;
  color: #1f2933;
  font-family: "Roboto";
  font-weight: 500;
}

.feature-description {
  font-size: 16px;
  color: #7b8794;
  font-family: "Roboto";
}
```

---

### ✅ **6. Final Touch**

- Use responsive classes `col-12 col-md-6 col-lg-4` for **3 cards per row** on large screens.
- Use `img-fluid` for images to make them responsive.
- Ensure vertical stacking on small screens.

---
