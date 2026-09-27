# Bloomwell — Skincare Brand Website

Bloomwell is a fully interactive skincare brand website designed with a warm, natural, and premium visual identity. The project combines **glassmorphism**, botanical colors, responsive layouts, and interactive JavaScript components to create a modern skincare shopping experience.

## 🌐 Live Demo

[View Bloomwell Live](https://stupendous-frangollo-379059.netlify.app/)

## ✨ Features

* Premium glassmorphism-based UI
* Responsive design for desktop, tablet, and mobile
* Asymmetric hero section with interactive product card
* Trust and credibility information strip
* Brand story section with statistics
* Interactive ingredient explorer
* Interactive skincare routine builder
* Add and remove products from a routine
* Live routine step count and total price
* Flip-card based "How to Use" section
* Testimonial carousel with navigation controls
* Newsletter subscription form with email validation
* Mobile hamburger navigation
* Keyboard-accessible interactive elements
* Reduced-motion support for accessibility

## 🎨 Design & UI

Bloomwell follows a clean-beauty inspired visual language rather than a generic e-commerce layout.

### Color Palette

The design uses a warm botanical palette consisting of:

* Moss green
* Clay / terracotta
* Gold
* Ivory

### Typography

* **Fraunces** — Used for headings and the Bloomwell wordmark
* **Manrope** — Used for body text and interface elements

### Visual Style

The interface uses:

* Frosted glass panels
* Background blur
* Soft shadows
* Layered cards
* Blurred color blobs
* Subtle grain texture
* Rounded UI elements

These elements create a layered visual depth while maintaining a calm skincare-focused aesthetic.

## 🧩 Interactive Components

### Ingredient Explorer

Users can select different ingredient chips to view detailed information about each ingredient without displaying all information at once.

### Routine Builder

The routine builder allows users to:

* Add products to their skincare routine
* Remove products
* View the number of routine steps
* See the running total price

The routine state is managed using JavaScript's `Map` data structure.

### Flip Cards

The "How to Use" section uses CSS 3D flip cards.

Each card contains:

* An icon and step name on the front
* Detailed instructions on the back

The flip effect uses:

```css
transform: rotateY();
transform-style: preserve-3d;
backface-visibility: hidden;
```

The cards can be interacted with through hover and keyboard focus.

### Testimonial Carousel

The testimonial section displays one review at a time and includes:

* Previous button
* Next button
* Dot indicators

JavaScript controls the active testimonial.

### Newsletter Form

The newsletter form includes client-side email validation with inline success and error states.

## 📱 Responsive Design

Bloomwell is designed for different screen sizes using two primary breakpoints:

* **Tablet:** `max-width: 960px`
* **Mobile:** `max-width: 640px`

### Tablet

At the tablet breakpoint:

* Two-column layouts become single-column layouts
* The routine summary changes from a sticky sidebar to a normal block
* Navigation changes to a hamburger menu
* Hero and brand-story sections stack vertically

### Mobile

At the mobile breakpoint:

* Flip cards become a single-column layout
* Product cards stack vertically
* Trust information wraps and centers
* Interactive controls receive larger touch-friendly spacing
* Navigation opens through a mobile menu

Headings also use CSS `clamp()` for fluid typography.

## ♿ Accessibility

The project includes several accessibility considerations:

* Semantic HTML elements
* Alternative text for product images
* `aria-label` attributes for icon-only buttons
* Keyboard focus support
* `tabindex` for interactive flip cards
* `:focus-within` support
* `prefers-reduced-motion` support

## 🛠️ Technologies Used

* **HTML5** — Structure and semantic markup
* **CSS3** — Styling, responsive design, animations, glassmorphism, and 3D transforms
* **JavaScript** — Interactive functionality and DOM manipulation
* **Google Fonts** — Fraunces and Manrope

## 📂 Project Structure

The project is implemented as a self-contained frontend application.

```text
Bloomwell/
│
├── index.html
└── README.md
```

The main HTML file contains the website structure, styling, and JavaScript functionality. Product images are embedded directly into the project so the page can operate as a standalone file.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/bloomwell.git
```

### 2. Open the project

```bash
cd bloomwell
```

### 3. Run the website

Open `index.html` directly in a browser.

No backend server or package installation is required.

## 💡 Design Decisions

### Why an asymmetric hero?

The asymmetric hero layout creates a stronger visual hierarchy by placing the main message and product visual in separate areas instead of using a conventional centered layout.

### Why a flip card for the routine steps?

A flat card can become visually cluttered when it contains both the step title and detailed instructions.

The flip-card approach keeps the front of the card simple while allowing the back to contain the complete instructions.

This makes the section easier to scan while still providing detailed information when needed.

### Why an interactive ingredient explorer?

Showing every ingredient description at once would make the section unnecessarily long. The interactive explorer keeps the interface clean while allowing users to explore individual ingredients.

## 📌 Project Highlights

* Fully responsive skincare brand interface
* Interactive vanilla JavaScript components
* CSS 3D card animations
* Dynamic routine builder
* Client-side form validation
* Accessible interactive elements
* Premium glassmorphism design
* Mobile-friendly navigation
* No frontend framework required

## 🔗 Links

**Live Website:**
https://stupendous-frangollo-379059.netlify.app/


## 📄 License

This project is created for learning, portfolio, and demonstration purposes.
