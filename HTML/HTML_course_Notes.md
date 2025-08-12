# HTML TEACHING COURSE
This course is a complete introduction to HTML, the foundational language of the web.  
Designed for beginners, it covers the structure and semantics of web pages, from basic document setup to advanced HTML elements and accessibility best practices — without using CSS or JavaScript.

---

## TEACHING FLOW / Topics to be Covered
1. Basic Introduction  
2. HTML Code Structure & Rules  
3. Text Semantics  
4. Links / Navigation  
5. Lists / Grouping  
6. Sectioning  
7. Images  
8. Tables  
9. Forms  
10. Disclosure Elements  
11. Advanced Content Models  
12. Accessibility-First HTML  
13. Validation  
14. Capstone Site Assembly  

---

## Basic Introduction to HTML
- **HTML** stands for **"HyperText Markup Language"**.  
  It is **not** a programming language — it’s a markup language that describes the structure of a web page.  
- In this course, we will learn the **latest version**, **HTML5**.

---

> **Question:** Why do we need this language? What does it do?  
> **Answer:** HTML acts as the **skeleton** of every web page. It tells the browser **what** to display and **in what order** — what comes first, what comes later, and what appears last.  
> It also gives **priority and emphasis** to certain parts of a page — e.g., large bold **headings** for important titles, smaller bold **subheadings** for topics, and other semantic markup.

---

> **Question:** Why is that important?  
> **Answer:** A well-structured HTML document is **crucial** for **SEO** (Search Engine Optimization). Search engines read HTML to understand your content.  
> If thousands of sites have similar information, the ones with **better HTML structure** often rank higher.  
> Benefits of good HTML:  
> - **SEO ranking** boost  
> - **Readability** for visitors  
> - **Accessibility** for assistive technologies

---

**In short:** HTML is the foundation of every website.  
Better HTML = Better structure, better SEO, and better user experience.

---

## HTML Code Structure & Rules

### `<!DOCTYPE html>` Declaration in HTML
We are using **HTML5**, not older versions. While some older sites still use outdated doctypes, the browser must know which rules to follow.  

---

> **Question:** How does the browser know the HTML version?  
> **Answer:** It looks at the **first line** of the document — the **DOCTYPE declaration** — which tells it the rendering mode.  

---

**For HTML5:**
```html
<!DOCTYPE html>
```
Short and simple — tells the browser: *Use standards mode (latest rules)*.

---

> **Question:** What if I don’t include it?  
> **Answer:** The browser may use **quirks mode**, acting like very old browsers, causing inconsistent layouts. Basically, quirks mode may render elements in different outdated ways, creating design inconsistencies.  

---

> **Question:** What is quirks mode?  
> **Answer:** A legacy compatibility mode meant for very old sites. It can break modern design consistency. Always include the HTML5 doctype.

---

**Notes:**
- `<!DOCTYPE html>` and `<!doctype html>` are equivalent (HTML is case-insensitive).  
- Must be the **first line**, before `<html>`.  
- It’s an **instruction**, not an HTML element.  

---

## `<head>` Tag in HTML
The `<head>` contains **information about the page** — setup, settings, and rules — that **affect the page** but are **not shown directly** to the user.

---

### `<title>` Tag
- Defines the **webpage’s name** in the browser tab.  
- Also used in bookmarks and search engine results.

---

### `<meta>` Tag
- Invisible to users, but controls **how the browser renders** the page.  
- Common uses:  
  - Viewport settings (responsive design).  
  - Zoom control (e.g., 100% default zoom).  
  - Character encoding (UTF-8 for symbols, emoji).  
  - SEO details (description, keywords, author).  

---

### `<link>` Tag
- Connects **external resources** to the page.  
- Commonly used for:  
  - CSS stylesheets  
  - Favicons  
  - Fonts or other resources  
- Example:
```html
<link rel="stylesheet" href="styles.css">
```

---

### `<style>` Tag
- Writes **CSS directly** inside the `<head>`.  
- Best for **small page-specific styles**.  
- Example:
```html
<style>
  body {
    background-color: lightblue;
  }
</style>
```

---

### `<script>` Tag
- Adds JavaScript (inline or external).  
- Example:
```html
<script src="app.js"></script>
```

---

💡 **Analogy:** The `<head>` is the **control room** — unseen by the audience but essential for the “performance” (webpage) to run smoothly.

---

## `<body>` Tag in HTML
The `<body>` contains **all visible content** in the browser window.

---

### Key Points
- Contains all **visible elements** (text, media, forms, tables, etc.).  
- Displays content **in the order written** in the HTML file.  

---

### What Can Go Inside
- Headings  
- Paragraphs  
- Lists  
- Links  
- Images, videos, audio  
- Forms  
- Tables  
- Buttons and interactive elements  

---

💡 **Analogy:** The `<body>` is the **stage** where content “performs” for the user.

---

## Structure of an HTML Page
![HTML file Structure](https://media.geeksforgeeks.org/wp-content/uploads/20240610121019/Screenshot-(4).png)

---

# 📚 Common HTML Tags by Category

## 📝 Text Formatting
- `<h1>` to `<h6>` — Headings  
- `<p>` — Paragraph  
- `<br>` — Line break  
- `<hr>` — Horizontal rule  
- `<b>` — Bold text  
- `<strong>` — Semantic bold  
- `<i>` — Italics  
- `<em>` — Semantic italics  
- `<u>` — Underlined text  
- `<mark>` — Highlighted text  
- `<small>` — Small text  
- `<sup>` — Superscript  
- `<sub>` — Subscript  

---

## 📄 Paragraphs & Structure
- `<div>` — Block container  
- `<span>` — Inline container  
- `<pre>` — Preformatted text  
- `<blockquote>` — Quotation block  
- `<code>` — Inline code  
- `<kbd>` — Keyboard input  
- `<samp>` — Sample output  
- `<var>` — Variable name  

---

## 🔗 Links & Navigation
- `<a>` — Anchor/link  
  - `href` — Destination URL  
  - `target="_blank"` — Open in new tab  
  - `title` — Tooltip text  

---

## 🖼 Images & Multimedia
- `<img>` — Image (`src`, `alt`, `width`, `height`)  
- `<figure>` — Image container  
- `<figcaption>` — Caption text  
- `<audio>` — Audio player (`src`, `controls`)  
- `<video>` — Video player (`src`, `controls`, `poster`)  
- `<source>` — Alternate media source  
- `<iframe>` — Embed another webpage/video  

---

## 📊 Tables
- `<table>` — Table container  
- `<caption>` — Table title  
- `<tr>` — Table row  
- `<th>` — Header cell  
- `<td>` — Data cell  
- `<thead>` — Table head section  
- `<tbody>` — Table body section  
- `<tfoot>` — Table footer section  
- `<col>` / `<colgroup>` — Column properties  

---

## 📝 Forms & Input
- `<form>` — Form container (`action`, `method`)  
- `<input>` — Input fields (text, password, email, etc.)  
- `<textarea>` — Multi-line input  
- `<label>` — Field label  
- `<select>` — Dropdown  
- `<option>` — Dropdown option  
- `<optgroup>` — Option group  
- `<button>` — Button  
- `<fieldset>` — Group related controls  
- `<legend>` — Fieldset caption  
- `<datalist>` — Predefined list for input  
- `<output>` — Output value  
