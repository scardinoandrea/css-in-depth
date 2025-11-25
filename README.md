# CSS in Depth - Course Materials

A comprehensive collection of HTML and CSS examples covering advanced CSS concepts, layouts, and techniques. This repository contains practical implementations and demonstrations of modern CSS features based on the book "CSS in Depth".

## 📋 Table of Contents

- [Overview](#overview)
- [Course Structure](#course-structure)
- [Getting Started](#getting-started)
- [Chapter Breakdown](#chapter-breakdown)
- [Key Concepts](#key-concepts)
- [Resources](#resources)

## 🎯 Overview

This repository contains hands-on examples and exercises for learning advanced CSS concepts. Each chapter focuses on specific CSS topics with practical implementations that demonstrate real-world usage patterns and best practices from the "CSS in Depth" book.

## 🗂️ Course Structure

```
css-in-depth/
├── chapter1.html       # CSS Fundamentals
├── chapter2.html       # Working with Relative Units
├── chapter3.html       # Mastering the Box Model
├── chapter4.html       # Making Sense of Floats
├── chapter5.html       # Flexbox
├── chapter5-grid.html  # CSS Grid Layout
├── chapter6.html       # Responsive Design
├── chapter7.html       # Positioning and Stacking Contexts
├── chapter8.html       # Responsive Images
└── README.md          # This file
```

## 🚀 Getting Started

1. **Clone or download** this repository
2. **Open any HTML file** in your web browser
3. **Inspect the code** using browser developer tools
4. **Modify styles** to experiment with different effects

### Prerequisites

- Basic understanding of HTML and CSS
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Text editor or IDE for code editing

## 📖 Chapter Breakdown

### Chapter 1 - Cascade, specificity and inheritance

Basic CSS concepts, selectors, and styling fundamentals.

### Chapter 2 - Working with Relative Units

Understanding `em`, `rem`, viewport units, and creating scalable designs.

### Chapter 3 - Mastering the Box Model

Deep dive into padding, margin, border, and how elements calculate their size.

### Chapter 4 - Making Sense of Floats

Float-based layouts, clearing floats, and understanding float behaviors.

### Chapter 5 - Flexbox

Modern flexible layouts with practical examples:

- Flex containers and flex items
- Flex direction, wrap, and alignment
- Practical navigation and card layouts

```css
.flex {
  display: flex;
}

/* Lobotomized owl selector for consistent spacing */
.flex > * + * {
  margin-top: 0;
  margin-left: 1.5em;
}
```

### Chapter 6 - Grid Layout

Two-dimensional layouts with CSS Grid:

- Grid containers and grid items
- Grid lines, tracks, and areas
- Responsive grid layouts
  Creating layouts that work across all device sizes:
- Media queries
- Flexible grids
- Mobile-first design

### Chapter 7 - Positioning and Stacking Contexts

Advanced positioning techniques:

- Modal dialogs and overlays
- Dropdown menus with CSS triangles
- Z-index and stacking contexts
- Sticky positioning

```css
/* Creating CSS triangles with borders */
.dropdown-label::after {
  content: "";
  position: absolute;
  border: 0.3em solid;
  border-color: black transparent transparent;
}
```

### Chapter 8 - Responsive design

WIP 🚧

## 💡 Key Concepts

### Flexbox Pattern - Lobotomized Owl Selector

```css
/* Ensures consistent spacing between flex items */
.flex > * + * {
  margin-top: 0;
  margin-left: 1.5em;
}
```

### Stacking Contexts

Elements with `z-index` create new stacking contexts that control layering behavior. Understanding this prevents z-index conflicts.

### Modal Implementation

```css
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 1;
}
```

### CSS Triangles

Created using borders where only one side is visible:

```css
.triangle {
  width: 0;
  height: 0;
  border: 10px solid transparent;
  border-bottom-color: #333;
}
```

## 📚 Resources

- [CSS in Depth Book](https://www.manning.com/books/css-in-depth) - The source material

---

## 📄 License

This project is for educational purposes based on the "CSS in Depth" book. Feel free to use these examples in your own learning and projects.

---

_Happy coding! 🌻_
