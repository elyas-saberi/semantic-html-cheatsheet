# 📘 Stop Using `<div>` Everywhere — Semantic HTML Best Practices

Semantic tags describe the meaning and purpose of each section of your page.  
They make your HTML more readable, SEO-friendly, and accessible.

---

## 📑 Table of Contents
- [Header](#header)
- [Nav](#nav)
- [Section](#section)
- [Article](#article)
- [Aside](#aside)
- [Main](#main)
- [Footer](#footer)
- [Figure + Figcaption](#figure-figcaption)
- [Picture](#picture)
- [Summary + Details](#summary-details)
- [Why Not Use `<div>`](#why-not-use-div)
- [Summary Table](#summary-table)

---
<a id="header"></a>
## 🏠 `<header>`

**Purpose:** Top section of a page or a section.

**Contains:**
- Logo  
- Navigation  
- Page title  
- Hero title  
- Intro text  

**Do NOT put:** The entire website content — only introductory/top content.

**Example:**
```html
<header>
  <h1>My Website</h1>
  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
  </nav>
</header>
```

---
<a id="nav"></a>
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

**Example:**
```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/blog">Blog</a></li>
    <li><a href="/contact">Contact</a></li>
  </ul>
</nav>
```

---
<a id="section"></a>
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

**Example:**
```html
<section>
  <h2>Our Services</h2>
  <p>We provide web development services...</p>
</section>
```

---
<a id="article"></a>
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

**Example:**
```html
<article>
  <h2>How to Learn HTML</h2>
  <p>HTML is the backbone of web development...</p>
</article>
```

---
<a id="aside"></a>
## ✍️ `<aside>`

**Purpose:** Secondary content related to the main content.  
**Contains:**
- Sidebars  
- Ads  
- Recommended articles  
- Author info  
- Extra links  

**Should NOT contain:** Main content.

**Example:**
```html
<aside>
  <h3>Related Posts</h3>
  <ul>
    <li><a href="#">Semantic HTML Tips</a></li>
    <li><a href="#">CSS Tricks</a></li>
  </ul>
</aside>
```

---
<a id="main"></a>
## 📌 `<main>`

**Purpose:** The main content of the page.

**Contains:** Everything that is **not**:
- Header  
- Footer  
- Navigation  
- Sidebar  

**Limit:**  
There must be **only one** `<main>` per page.

**Example:**
```html
<main>
  <h1>Welcome to Our Site</h1>
  <p>Main content goes here...</p>
</main>
```

---
<a id="footer"></a>
## 🔽 `<footer>`

**Purpose:** Bottom section of the page.  
**Contains:**
- Copyright  
- Social links  
- Contact info  
- Secondary navigation  
- Footer credits  

**Example:**
```html
<footer>
  <p>&copy; 2025 My Website</p>
  <nav>
    <a href="/privacy">Privacy</a>
  </nav>
</footer>
```

---
<a id="figure-figcaption"></a>
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
<a id="picture"></a>
## 🖼️ `<picture>`

**Purpose:** Responsive images — loads different image files for different screen sizes.

**Example:**
```html
<picture>
  <source media="(min-width: 1024px)" srcset="large.jpg">
  <source media="(min-width: 768px)" srcset="medium.jpg">
  <img src="small.jpg" alt="Example image">
</picture>
```

---
<a id="summary-details"></a>
## 📑 `<summary>` + `<details>`

**Purpose:** Expandable/collapsible content.

**Example:**
```html
<details>
  <summary>Click to expand</summary>
  <p>Hidden content appears here!</p>
</details>
```

---
<a id="why-not-use-div"></a>
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
<a id="summary-table"></a>
# ⭐ Summary Table

| Tag         | Purpose                 | What it contains                    |
|-------------|-------------------------|-------------------------------------|
| `<header>`  | Top/intro section       | Logo, nav, main heading             |
| `<nav>`     | Navigation links        | Menus                               |
| `<section>` | Thematic grouping       | Related content blocks              |
| `<article>` | Stand-alone content     | Posts, cards, reviews               |
| `<aside>`   | Secondary info          | Ads, sidebars                       |
| `<main>`    | Page’s primary content  | Core content only                   |
| `<footer>`  | Bottom info             | Copyright, links                    |
| `<figure>`  | Media block             | Images + captions                   |
| `<picture>` | Responsive images       | Source images                       |
| `<details>` | Toggle content          | FAQs, spoilers                      |

---
