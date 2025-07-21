# CSS Gradients & More Bootstrap Components

## 1. Bootstrap Components

### 1.1 Modal

A **Bootstrap Modal** is a dialog box or popup window that is displayed on top of the current page.

- Can be triggered via a button with `data-toggle="modal"` and `data-target="#modalId"`.
- Customizable content areas:

  - **Modal Header**
  - **Modal Body**
  - **Modal Footer**

#### Example Usage:

```html
<!-- Trigger Button -->
<button
  type="button"
  class="btn btn-primary"
  data-toggle="modal"
  data-target="#exampleModal"
>
  Launch Modal
</button>

<!-- Modal Structure -->
<div
  class="modal fade"
  id="exampleModal"
  tabindex="-1"
  aria-labelledby="exampleModalLabel"
  aria-hidden="true"
>
  <div class="modal-dialog mt-5">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Gift Voucher</h5>
        <button
          type="button"
          class="close"
          data-dismiss="modal"
          aria-label="Close"
        >
          <span aria-hidden="true">×</span>
        </button>
      </div>
      <div class="modal-body">
        <!-- Modal content like image or text -->
        <img src="gift-image-url.png" class="w-100" />
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">
          Close
        </button>
      </div>
    </div>
  </div>
</div>
```

---

## 2. Thanking Customers Section with Bootstrap Modal

- Section displays a thank-you message with a **Redeem Gift** button.
- Clicking the button opens a **Bootstrap modal** showing a **gift voucher image**.

### Key Styles:

```css
.thanking-customers-section {
  background-color: #d0b2001a;
}

.thanking-customers-section-heading {
  color: #183b56;
  font-family: "Roboto";
  font-size: 28px;
  font-weight: 700;
}

.custom-button {
  background-color: #d0b200;
  color: white;
  border-radius: 8px;
  width: 130px;
  height: 45px;
  border: none;
}
```

---

## 3. CSS Gradients

Gradients are smooth transitions between two or more specified colors.

### Types of Gradients

#### 3.1 Linear Gradient

A linear transition between colors along a straight line.

```css
.linear-gradient-background {
  height: 100vh;
  background-image: linear-gradient(#2196f3, #f44336);
}
```

##### 3.1.1 Changing Direction

Use `to left`, `to right`, `to top`, `to bottom`:

```css
background-image: linear-gradient(to right, #2196f3, #f44336);
```

##### 3.1.2 More Than Two Colors

```css
.linear-gradient-background-with-more-colors {
  background-image: linear-gradient(red, blue, yellow, orange);
}
```

---

#### 3.2 Radial Gradient

Colors radiate out from a center point.

```css
.radial-gradient-background {
  background-image: radial-gradient(#2196f3, #f44336);
}
```

##### 3.2.1 More Than Two Colors

```css
.radial-gradient-background-with-more-colors {
  background-image: radial-gradient(red, blue, yellow, orange);
}
```

---

## 4. Food Munch Website Code

A full-feature responsive food ordering website with the following key sections:

### Navigation Bar

- Sticky navigation with logo and scroll links.
- Utilizes `navbar`, `navbar-expand-lg`, `navbar-light`.

### Banner Section

- Full screen background image.
- CTA buttons: `View Menu`, `Order Now`.

```css
.banner-section-bg-container {
  background-image: url("banner-image-url");
  height: 100vh;
  background-size: cover;
}
```

### Why Choose Us (WCU) Section

Three-card layout showing:

- Food Service
- Fresh Food
- Best Offers

### Explore Menu Section

Grid layout with different menu items like:

- Non-Veg Starters
- Veg Starters
- Soups, Seafood, Main Course, Noodles, Salads, Desserts

### Healthy Food Section

Highlighting healthy organic food with image and description.

### Delivery and Payment Section

Emphasizes:

- Live tracking
- Multiple payment options (Visa, MasterCard, PayPal, Amex)

### Thanking Customers Section

Same modal logic for showing gift voucher reused here.

### Follow Us Section

Social media icons inside circular containers.

```css
.follow-us-icon-container {
  background-color: #faf7e8;
  width: 80px;
  height: 80px;
  border-radius: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### Footer Section

- Contact Email
- Physical Address
- Footer logo

---

## Design Elements Summary

### Fonts Used:

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
```

### Key Custom Classes:

| Class Name                       | Description                              |
| -------------------------------- | ---------------------------------------- |
| `.custom-button`                 | Gradient background CTA button           |
| `.custom-outline-button`         | Transparent button with border           |
| `.thanking-customers-section`    | Background with radial gradient          |
| `.modal-header`, `.modal-footer` | Custom modal styling                     |
| `.wcu-card`, `.menu-item-card`   | Box layout with border-radius & shadows  |
| `.follow-us-icon-container`      | Circular icon wrapper with centered icon |

---

## Conclusion

This project showcases:

- Responsive Bootstrap components.
- Custom-styled modal interactions.
- CSS gradient backgrounds (linear and radial).
- Structured layout using Bootstrap grid system.
- Reusability of design components (e.g., buttons, modals, cards).

Perfect for learning how to combine **Bootstrap UI**, **custom styles**, and **CSS gradients** in real-world web design!

---
