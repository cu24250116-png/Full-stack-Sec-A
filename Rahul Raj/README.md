# Full Stack Web Development Lab Submissions

**Student Name:** Rahul Raj  
**Curriculum:** Full Stack Lab  
**Lab Sheets Covered:** Lab Sheet 01 & Lab Sheet 02  

---

## 📁 Repository Directory Structure

```text
Rahul Raj/
├── index.html                                 # Central Showcase & Evaluation Portal
├── README.md                                  # Complete Documentation & Verification Guide
│
├── Lab Sheet 1/                               # LAB SHEET 01: Core Web Structures Using Semantic HTML
│   ├── task1_resume/
│   │   ├── index.html                         # Task 1.1: Semantic HTML5 Resume Page
│   │   └── style.css                          # Accessible Typographic & Print Styles
│   ├── task2_nested_nav/
│   │   ├── index.html                         # Task 1.2: Nested Navigation Menu Bar
│   │   └── style.css                          # Multi-Tier Flyout Dropdown & Focus Styles
│   └── task3_catalog/
│       ├── index.html                         # Task 1.3: Itemized Web Catalog (<dl>, <dt>, <dd>)
│       └── style.css                          # Metadata Definition List Card Styles
│
└── Lab Sheet 2/                               # LAB SHEET 02: Dynamic Interface Styling & Interactivity
    ├── task1_dark_mode/
    │   ├── index.html                         # Task 2.1: Clean Dark-Mode Landing Layout
    │   ├── style.css                          # CSS Variables (:root & [data-theme="dark"])
    │   └── script.js                          # Vanilla JS Theme Toggler with LocalStorage
    ├── task2_photo_grid/
    │   ├── index.html                         # Task 2.2: Responsive Flexbox Photo Grid
    │   └── style.css                          # Pure CSS Flexbox Rules & Hover Transforms
    └── task3_todo_app/
        ├── index.html                         # Task 2.3: Interactive Client-Side Todo Application
        ├── style.css                          # Modern Card Layout & Error Flag Badges
        └── script.js                          # Runtime Append Engine & Operational Error Flags
```

---

## 📋 Syllabus Tasks & Implementations

### Lab Sheet 01: Core Web Structures Using Semantic HTML
*Primary Syllabus Exercise Reference: Write a program to create a simple webpage using HTML5. Incorporate standard header elements, dynamic text formatting anchors, and a main container block.*

- **Task 1.1: Semantic HTML Resume Page**
  - Incorporates semantic layout blocks: `<header>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<address>`, `<time>`.
  - Full conformance with modern accessibility parameters: WCAG 2.1 Level AA, skip-to-content links, ARIA landmark roles, accessible typography, and `@media print` layout.
- **Task 1.2: Nested Navigation Menu Bar**
  - Hierarchical menu constructed with list item anchors (`<ul>`, `<li>`, `<a>`).
  - Strict implementation of absolute path linking patterns to external resource addresses (W3C, WHATWG, MDN, TC39, Node.js, Python, GitHub).
  - Accessible multi-level dropdowns with `:focus-within` and live absolute URL verification table.
- **Task 1.3: Itemized Web Catalog Interface**
  - Formulates descriptive technical metadata terms via structured definition lists (`<dl>`, `<dt>`, `<dd>`).
  - Catalog features runtime systems, databases, web servers, and in-memory caches with live client-side category and keyword search filtering.

---

### Lab Sheet 02: Dynamic Interface Styling & Scripting Interactivity
*Primary Syllabus Exercise Reference: Write a program to create an interactive website using a combination of HTML layout nodes, external CSS stylesheets, and core JavaScript operational elements.*

- **Task 2.1: Clean Dark-Mode Landing Layout**
  - Implements custom styling overrides via CSS custom properties (`:root` light tokens vs `[data-theme="dark"]` overrides).
  - Interactive toggler method in vanilla JavaScript with `localStorage` state persistence and OS `prefers-color-scheme` synchronization.
  - Interactive live CSS variable token inspector.
- **Task 2.2: Responsive Flexbox Photo Grid**
  - Built strictly with CSS Flexbox rules (`display: flex; flex-wrap: wrap; justify-content: center; gap: ...`).
  - Wraps fluidly across mobile viewports without horizontal clipping.
  - Rich hovering transform animations (`translateY`, scale, zoom, overlay transition).
- **Task 2.3: Client-Side Interactive Todo Application**
  - **Runtime Element Append Mechanisms**: Uses `document.createElement()`, binds attributes/listeners in memory, and dynamically injects nodes via `prepend()` and `appendChild()`.
  - **Operational Validation Error Flags**: Detects empty or whitespace inputs, minimum character constraints (< 3 characters), and active duplicate tasks, rendering dynamic animated warning flags.
  - Task status toggling, deletion with fade-out animations, filtering (All / Active / Completed), and persistent storage.

---

## 🚀 How to Run & Verify

1. Open `Rahul Raj/index.html` in any web browser to access the central evaluation portal.
2. From the portal, click **Launch Task** on any card to test the individual task.
3. Every individual task page includes a **Back to Lab Portal** button for seamless navigation.

---

## 🔄 Git Push Instructions

To push this codebase to your mentor's repository or your personal repository:

```bash
# Navigate into the project folder
cd "Rahul Raj"

# Initialize Git repository (if not already done)
git init

# Add all lab sheets and files
git add .

# Commit with a descriptive message
git commit -m "feat: complete Full Stack Lab Sheet 01 and Lab Sheet 02 for Rahul Raj"

# Add your remote repository URL
git remote add origin <YOUR_GITHUB_REPO_URL>

# Push to your branch
git branch -M main
git push -u origin main
```

If submitting a Pull Request to your mentor's repository:
```bash
git remote add mentor <MENTOR_GITHUB_REPO_URL>
git fetch mentor
```
