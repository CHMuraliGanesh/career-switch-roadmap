# Week-01-02 HTML CSS

# 📚 Week 1-2: HTML & CSS Deep Dive

---

## 🔸 HTML5 Core Concepts
- **HTML Boilerplate Setup** (`<!doctype>`, `<html>`, `<head>`, `<body>`)
- **Semantic Elements**: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`
- **Forms**: `<form>`, `<input>`, `<textarea>`, `<button>`, `<select>`, `<option>`, `<label>`, `<fieldset>`, `<legend>`
- **Form Attributes**: `action`, `method`, `name`, `id`, `for`, `placeholder`, `required`, `autocomplete`
- **Tables**: `<table>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>`, `<td>`, `colspan`, `rowspan`
- **Media Tags**: `<img>`, `<video>`, `<audio>`, `<source>`, `<track>`
- **SEO Basics**: Heading hierarchy `<h1>` to `<h6>`, proper `<meta>` tags (description, viewport), `alt` attributes
- **Accessibility (a11y) Basics**: `aria-label`, `role`, `tabindex`, logical tab order, keyboard navigation

## 🔸 HTML5 Advanced
- Custom Data Attributes: `data-*`
- `<details>`, `<summary>`, `<dialog>`
- `<template>` and Shadow DOM Basics
- Progressive Enhancement Concepts

---

## 🔸 CSS Core Concepts
- **Selectors**: Universal (`*`), Type (`h1`), Class (`.class`), ID (`#id`), Descendant (`div p`), Child (`div > p`), Adjacent sibling (`h1 + p`)
- **Box Model**: Content, Padding, Border, Margin
- `box-sizing: border-box`
- **Positioning**: Static, Relative, Absolute, Fixed, Sticky
- **Display**: Block, Inline, Inline-block, None
- **Overflow**: `overflow: hidden; scroll; auto`
- **Units**: `px`, `em`, `rem`, `%`, `vw`, `vh`

## 🔸 CSS Layouts
- **Flexbox**:
  - `display: flex;`
  - Main Axis and Cross Axis
  - Justify Content, Align Items, Flex Direction, Flex Wrap
- **Grid**:
  - `display: grid;`
  - `grid-template-rows`, `grid-template-columns`
  - Gap, Grid Auto Flow

---

## 🔸 CSS Styling
- **Typography**: Font-family, Font-size, Font-weight, Line-height, Text-align
- **Colors**: Named colors, HEX, RGB, RGBA, HSL
- **Backgrounds**: Background-color, Background-image, Background-size, Background-position
- **Borders and Shadows**: Border-radius, Box-shadow, Text-shadow
- **Transitions and Animations** (Intro level)

---

## 🔸 Responsive Web Design
- **Media Queries**:
  ```css
  @media (max-width: 768px) {
    /* Responsive CSS */
  }

Viewport Meta Tag:

html
Copy
Edit
<meta name="viewport" content="width=device-width, initial-scale=1.0">
Mobile First Design Principles

Responsive Images: srcset, sizes

🔸 Best Practices
Use of External CSS vs Inline Styles

Separation of Structure (HTML) and Presentation (CSS)

Accessibility-friendly Forms and Navigation

🔸 Mini Practice Projects
 Create a simple Personal Portfolio webpage (1-page)

 Build a Responsive Navigation Bar

 Create a Login Form (with form validation using required attributes)

 Make a Two-column Layout using Flexbox and Grid

 Clone a simple Landing Page from a famous brand (basic)

📚 Browser, HTML, CSS, and JavaScript Core Knowledge (with Answers)
✅ 1. How the Browser Rendering Pipeline Works (DOM, CSSOM, Render Tree)
Answer:

HTML Parsing → DOM

CSS Parsing → CSSOM

DOM + CSSOM → Render Tree

Layout (Reflow) → Browser calculates position/size

Paint → Fill pixels

Compositing → Final screen render

Diagram:

css
Copy
Edit
HTML → DOM
CSS → CSSOM
DOM + CSSOM → Render Tree → Layout (Reflow) → Paint → Compositing → Display
✅ 2. Critical Rendering Path (CRP) and How to Optimize It
Answer:

Minify CSS/JS

Defer JS: <script defer>

Async JS: <script async>

Inline Critical CSS

Lazy load images and iframes

✅ 3. Differences Between Block, Inline, Inline-Block Elements
Element Type	Behavior
Block	Full width, new line (<div>, <p>)
Inline	Content width, inline (<span>, <a>)
Inline-Block	Inline + width/height (<img>, styled blocks)

✅ 4. Event Loop, Microtasks, Macrotasks (JavaScript Runtime Concept)
Answer:

Call Stack: Executes code

Event Loop: Manages queues

Microtasks: Promise .then, MutationObserver (higher priority)

Macrotasks: setTimeout, setInterval

✅ 5. How CSS Specificity Works (Debugging Styles)
Answer:

swift
Copy
Edit
Inline Styles > IDs > Classes/Pseudo-classes > Elements/Pseudo-elements
Inline: 1000

ID: 100

Class/Pseudo-class: 10

Element: 1

✅ 6. How Browser Caching Works (Cache-Control, ETags)
Answer:

Cache-Control: max-age=3600

ETag: Unique ID for resource

304 Not Modified if unchanged

✅ 7. What Happens on Reflow/Repaint and How to Minimize Them
Answer:

Reflow: Layout changes (costly)

Repaint: Style changes only

Optimization: Use transform: translate() for animations

✅ 8. Responsive Design Principles (Mobile First, Media Queries)
css
Copy
Edit
/* Mobile first */
body {
  font-size: 16px;
}
@media (min-width: 768px) {
  body {
    font-size: 18px;
  }
}
Why Mobile-First? Better performance, progressive enhancement.

✅ 9. Accessibility (ARIA roles, Keyboard Navigation)
Answer:

Use semantic HTML

Provide alt for images

Use aria-label, role, and tabindex properly

Ensure keyboard navigability
