# Full Stack Web Development Lab Submissions (Labs 1 &ndash; 4)

**Student Name:** Rahul Raj  
**Course:** Full Stack Web Development Laboratory  
**Submissions Included:** Lab Sheet 01, Lab Sheet 02, Lab Sheet 03, Lab Sheet 04  

---

## 📁 Repository Directory Structure

```text
Rahul Raj/
├── index.html                                 # Central Evaluation & Showcase Hub (Labs 1-4)
├── README.md                                  # Complete Technical Guide & Documentation
│
├── Lab Sheet 1/                               # LAB SHEET 01: Core Web Structures Using Semantic HTML
│   ├── task1_resume/ (index.html, style.css)  # Task 1.1: Semantic HTML5 Resume Page (A11y, WCAG 2.1)
│   ├── task2_nested_nav/ (index.html, style.css) # Task 1.2: Nested Navigation Menu with Absolute URLs
│   └── task3_catalog/ (index.html, style.css) # Task 1.3: Itemized Web Catalog (<dl>, <dt>, <dd>)
│
├── Lab Sheet 2/                               # LAB SHEET 02: Dynamic Interface Styling & Interactivity
│   ├── task1_dark_mode/ (index.html, style.css, script.js) # Task 2.1: CSS Variables Dark Mode
│   ├── task2_photo_grid/ (index.html, style.css)           # Task 2.2: Flexbox Photo Grid (Fluid Wrapping)
│   └── task3_todo_app/ (index.html, style.css, script.js)  # Task 2.3: Validation Flags Todo App
│
├── Lab Sheet 3/                               # LAB SHEET 03: Introduction to React.js
│   ├── package.json, vite.config.js           # Vite + React 18 configuration
│   ├── dist/                                  # Production built preview bundle
│   └── src/
│       ├── App.jsx                            # State & Effect persistence engine
│       ├── components/
│       │   ├── AddTaskForm.jsx                # Input form with operational validation flags
│       │   ├── TaskList.jsx                   # Container mapping to child items
│       │   ├── TaskItem.jsx                   # Single task element with status & actions
│       │   ├── FilterTabs.jsx                 # Filter tab controls & count indicators
│       │   ├── TaskMetrics.jsx                # Analytics & completion rate calculator
│       │   └── ComponentTree.jsx              # Deliverable: Component Tree Diagram UI
│       └── README.md                          # Architecture specs & Component Tree Diagram
│
└── Lab Sheet 4/                               # LAB SHEET 04: React Routing & State Management
    ├── package.json, vite.config.js           # Vite + React + react-router-dom
    ├── dist/                                  # Production built preview bundle
    └── src/
        ├── App.jsx                            # react-router-dom route declarations
        ├── context/
        │   └── StoreContext.jsx               # Context API Global State (Cart & Favorites)
        ├── data/
        │   └── products.js                    # Comprehensive developer hardware catalog
        ├── pages/
        │   ├── Home.jsx                       # 1. Landing Page
        │   ├── Products.jsx                   # 2. Products Catalog with filters & search
        │   ├── ProductDetails.jsx             # 3. Dynamic Route (:id params)
        │   └── NotFound.jsx                   # 4. Custom 404 Not Found Page
        └── components/
            ├── Navbar.jsx                     # Reactive badges for Cart & Favorites
            ├── ProductCard.jsx                # Reusable catalog card
            ├── CartDrawer.jsx                 # Global Cart Drawer modal
            └── LoadingSkeleton.jsx            # Deliverable: Loading state simulator
```

---

## 🌳 Lab 3: Component Tree Diagram

```mermaid
graph TD
    App["&lt;App /&gt; (useState, useEffect, localStorage)"]
    App --> AddTaskForm["&lt;AddTaskForm /&gt; (Input &amp; Validation Flags)"]
    App --> FilterTabs["&lt;FilterTabs /&gt; (Filter State Callbacks)"]
    App --> TaskList["&lt;TaskList /&gt; (Props Delegation)"]
    App --> TaskMetrics["&lt;TaskMetrics /&gt; (Computed Stats)"]
    TaskList --> TaskItem["&lt;TaskItem /&gt; (Dynamic Item Row xN)"]

    AddTaskForm -.->|onAddTask(newTodo)| App
    FilterTabs -.->|onFilterChange(filter)| App
    TaskItem -.->|onToggle(id) / onDelete(id)| TaskList
    TaskList -.->|onToggleTask / onDeleteTask| App
```

---

## 🗺️ Lab 4: SPA Routing & State Flow Architecture

```mermaid
graph TD
    User([User Browser]) --> App["&lt;App /&gt; (StoreProvider)"]
    App --> Navbar["&lt;Navbar /&gt; (Live Cart &amp; Favorite Badges)"]
    App --> Routes["&lt;Routes&gt;"]

    Routes -->|Path: '/'| Home["&lt;Home /&gt;"]
    Routes -->|Path: '/products'| Products["&lt;Products /&gt;"]
    Routes -->|Path: '/products/:id'| ProductDetails["&lt;ProductDetails /&gt; (useParams)"]
    Routes -->|Path: '*'| NotFound["&lt;NotFound /&gt; (404 Fallback)"]

    StoreContext[("StoreContext (Global Cart &amp; Favorites)")] -.-> Navbar
    StoreContext -.-> Home
    StoreContext -.-> Products
    StoreContext -.-> ProductDetails
    StoreContext -.-> CartDrawer["&lt;CartDrawer /&gt;"]
```

---

## 🚀 How to Run & Verify

### Viewing the Central Portal:
Open `Rahul Raj/index.html` in your browser to test and launch all 4 lab sheets!

### Running Lab 3 (React.js):
```bash
cd "Rahul Raj/Lab Sheet 3"
npm run dev     # or preview dist/ with: npm run preview
```

### Running Lab 4 (React Router SPA):
```bash
cd "Rahul Raj/Lab Sheet 4"
npm run dev     # or preview dist/ with: npm run preview
```
