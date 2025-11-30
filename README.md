# 📘 Stop Using `<div>` Everywhere — Semantic HTML Best Practices

Semantic tags describe the meaning and purpose of each section of your page.  
They make your HTML more readable, SEO-friendly, and accessible.

Below are the most common semantic elements and what they are used for.

---

## 🏠 `<header>`

**Purpose:** Top section of a page or a section  
**Contains:**
- Logo  
- Navigation  
- Page title  
- Hero title  
- Intro text  

**Do NOT put:** The entire website content — only introductory/top content.

---

## 🧭 `<nav>`

**Purpose:** Contains the main navigation links.  
**Contains:**
- Menu items  
- Header navigation  
- Sidebar navigation  

**Do NOT put:**
- “Read more” links  
- Buttons  
- Social icons  
- Article links  

Only put *navigational* links.

---

## 🏷 `<section>`

**Purpose:** A thematic group of related content.  
**Contains:**
- A group of articles  
- Features section  
- Pricing area  
- Services area  

**Notes:**
- Should usually contain its own heading  
- Helps divide the page into meaningful blocks  

---

## 📄 `<article>`

**Purpose:** Self-contained content that can stand alone.  
**Contains:**
- Blog post  
- News article  
- Forum post  
- Product card  
- User review  

**Rule:**  
If you can move the block to another page and it still makes sense → it’s an **article**.

---

## ✍️ `<aside>`

**Purpose:** Secondary content related to the main content.  
**Contains:**
- Sidebars  
- Ads  
- Recommended articles  
- Author info  
- Extra links  

**Should NOT contain:** Main content.

---

## 📌 `<main>`

**Purpose:** The main content of the page.  
**Contains:** Everything that is **not**:
- Header  
- Footer  
- Navigation  
- Sidebar  

**Limit:**  
There must be **only one** `<main>` per page.

---

## 🔽 `<footer>`

**Purpose:** Bottom section of the page.  
**Contains:**
- Copyright  
- Social links  
- Contact info  
- Secondary navigation  
- Footer credits  

---

## 🎨 `<figure>` + `<figcaption>`

**Purpose:** Media content with a caption.  
**Contains:**
- Images  
- Diagrams  
- Code examples  
- Charts  

**Example:**
```html
<figure>
  <img src="image.jpg" alt="Mountain">
  <figcaption>A beautiful mountain at sunset.</figcaption>
</figure>
```

---

## 🖼️ `<picture>`

**Purpose:** Responsive images — loads different image files for different screen sizes.

---

## 📑 `<summary>` + `<details>`

**Purpose:** Expandable/collapsible content.

---

# ❓ Why Not Use `<div>` for Everything?

`<div>` has **no meaning**.  
Semantic tags tell browsers, search engines, and developers what each section represents.

Semantic HTML improves:
- SEO  
- Accessibility  
- Screen reader experience  
- Code readability  
- Maintainability  

---

# ⭐ Summary Table

| Tag         | Purpose               | What it contains                    |
|-------------|-----------------------|-------------------------------------|
| `<header>`  | Top/intro section     | Logo, nav, main heading             |
| `<nav>`     | Navigation links      | Menus                               |
| `<section>` | Thematic grouping     | Related content blocks              |
| `<article>` | Stand-alone content   | Posts, cards, reviews               |
| `<aside>`   | Secondary info        | Ads, sidebars                       |
| `<main>`    | Page’s primary content| Core content only                   |
| `<footer>`  | Bottom info           | Copyright, links                    |
| `<figure>`  | Media block           | Images + captions                   |
| `<picture>` | Responsive images     | Source images                       |
| `<details>` | Toggle content        | FAQs, spoilers                      |

---
