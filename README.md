# 🏗️ BuildPro Construction Website

A fully-featured, production-quality construction company website built over 3 days (Day 63–65) using **HTML5, CSS3, and Vanilla JavaScript** with **Gemini AI integration**.

---

## 🌟 Features

### Day 63 — Foundation
- ✅ Three-page site: `index.html`, `services.html`, `contact.html`
- ✅ Shared `style.css` for all pages
- ✅ Sticky navigation header with logo and nav links
- ✅ Hero section with full-screen background image + `::before` overlay
- ✅ Services page with Flexbox two-column layout
- ✅ Contact form with `<textarea>`, `<input>` fields, and submit button
- ✅ CSS reset (margin/padding zero-out, `box-sizing: border-box`)
- ✅ Premium Inter + Playfair Display Google Fonts
- ✅ Responsive hamburger menu (hidden on desktop, toggleable on mobile)
- ✅ Service blocks with `box-shadow`, `border`, hover animation (`translateY`)
- ✅ Contact form with `border-radius` and animated `focus` states
- ✅ Gradient submit button with hover effect
- ✅ Mobile media query at `768px` (two-column → stacked)
- ✅ Footer with copyright, contact details, and social media links

### Day 64 — Chatbot & AI-Generated Content
- ✅ Fixed-position chatbot container (bottom-right)
- ✅ Circular toggle button with open/close animation
- ✅ Chatbot UI: header, scrollable message area, input area
- ✅ User and AI message bubbles with distinct colours/alignment
- ✅ Textarea input + Send button
- ✅ **Gemini 2.0 Flash API** integration for real AI responses
- ✅ Typing indicator animation (three bouncing dots)
- ✅ Chat history array maintained for conversation context
- ✅ Auto welcome message on first open
- ✅ `about-us-content` div populated by AI at page load
- ✅ `services-content` div populated by AI at page load
- ✅ Bullet-point services auto-formatted as `<ul><li>` HTML
- ✅ Loading placeholder animation while fetching content
- ✅ `try...catch` error handling with user-friendly error messages

### Day 65 — SEO, Accessibility & Final Polish
- ✅ Semantic HTML5: `<header>`, `<main>`, `<section>`, `<aside>`, `<footer>`
- ✅ SEO meta tags: `<title>`, `<meta name="description">`, `<meta name="keywords">`
- ✅ Canonical `<link>` tags on all pages
- ✅ `aria-label` on all navigation links, buttons, and form elements
- ✅ Logical heading hierarchy (`h1` → `h2` → `h3` → `h4`)
- ✅ `alt` text on all images
- ✅ localStorage autofill for Name and Email on contact form
- ✅ Form `submit` prevention with `event.preventDefault()`
- ✅ Success message on form submission
- ✅ Clean, commented JavaScript with no console.log clutter

---

## 🗂️ Project Structure

```
construction/
├── index.html       — Homepage (hero, about, services preview, chatbot)
├── services.html    — Services page (two-column Flexbox layout)
├── contact.html     — Contact page (form with autofill)
├── style.css        — Shared stylesheet (all pages)
├── hero.png         — AI-generated hero background image
└── README.md        — This file
```

---

## 🚀 How to Run

1. **No server needed** — open any file directly in your browser:
   ```
   Double-click index.html  →  Opens in default browser
   ```

2. **Or use VS Code Live Server** for auto-reload on save:
   - Install the "Live Server" extension
   - Right-click `index.html` → "Open with Live Server"

---

## 🤖 Gemini AI Setup

The chatbot and auto-generated content use the **Gemini 2.0 Flash** model.

The API key is embedded in `index.html` inside the `<script>` tag:
```javascript
const GEMINI_API_KEY = 'YOUR_API_KEY_HERE';
```

> **Note:** For production use, never expose API keys in client-side code. Use a backend proxy instead.

---

## 🎨 Design System

| Token         | Value                    |
|---------------|--------------------------|
| Primary       | `#e87722` (orange)       |
| Accent        | `#f0a500` (gold)         |
| Dark BG       | `#0f1117`                |
| Surface       | `#ffffff`                |
| Font (body)   | Inter (Google Fonts)     |
| Font (heading)| Playfair Display         |
| Border Radius | `12px`                   |
| Transition    | `.3s cubic-bezier()`     |

---

## ♿ Accessibility

- All interactive elements have `aria-label` attributes
- `aria-live="polite"` on chat messages and form feedback
- Keyboard-navigable hamburger menu (Enter/Space to toggle)
- Semantic headings for screen reader navigation
- Sufficient colour contrast ratios

---

## 🔍 SEO

- Unique `<title>` and `<meta name="description">` per page
- `<link rel="canonical">` on each page
- Descriptive `alt` attributes on all images
- Semantic HTML structure (no div soup)
- Single `<h1>` per page

---

*Built as part of a structured web development curriculum — Days 63, 64, and 65.*
