Here’s a complete `README.md` specifically for your **Conference Page** project:

---

# 🎤 Conference Page

This project is a simple and responsive **Conference Page** built using **HTML**, **CSS**, and **Bootstrap**, along with **CCBP UI Kit** standards.

It consists of two main sections:
- **Home Page**
- **Conference Details Page**

Clicking the **"Know more"** button navigates from the home page to the details section.

---

## 📄 Features

### ✅ Conference Home Page
- Displays a hero section with a featured image.
- Shows the conference title and a short description.
- Contains a “Know more” button that triggers the view of the detailed conference section.

### ✅ Conference Details Page
- Embeds a YouTube video from the event.
- Displays key stats:
  - 1400+ Attendees
  - 100+ Workshops
  - 120+ Speakers
  - 10+ Countries
- Includes a **Back** button to return to the home section.

---

## 💻 Tech Stack

- HTML5
- CSS3
- Bootstrap 4+
- CCBP UI Kit

---

## 🖼️ Resources Used

### 📷 Images
- **Conference Banner:**  
  `https://d2clawv67efefq.cloudfront.net/ccbp-static-website/conference-img.png`

### 🎥 YouTube Video
- `https://www.youtube.com/embed/W_2hCKnzWj0`

---

## ⚙️ Implementation Notes

- Used `Roboto` font throughout.
- All section containers follow the **CCBP naming rule**:
  ```html
  <div id="sectionHomePage">...</div>
  <div id="sectionConferencePage">...</div>
  ```

* Sections are **not nested**; they are placed **parallelly** in the HTML document.
* **Avoided** applying Bootstrap flex classes (`d-flex`, etc.) directly to section containers.

---

## 🧪 How It Works

1. User lands on the **Home Page** with a summary of the conference.
2. On clicking the **"Know more"** button:

   * The app shows the **Conference Details Page** with a video and stats.
3. Clicking **"Back"** returns the user to the **Home Page**.

---

## 📌 Screenshot Previews

### Home Page

![Home Page](./home-preview.png)

### Conference Details Page

![Details Page](./details-preview.png)

---

## 📁 Folder Structure (Suggested)

```
project-folder/
│
├── index.html
├── styles.css
├── README.md
├── home-preview.png
└── details-preview.png
```

---

## 📚 Learnings

* Working with multi-section navigation in HTML.
* Applying Bootstrap spacing and alignment effectively.
* Embedding YouTube videos responsively.
* Using `id`-based section management as per CCBP UI Kit standards.

---

## 🚀 Author

**Your Name**
[GitHub Profile](https://github.com/yourusername)

