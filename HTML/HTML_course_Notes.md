# HTML TEACHING COURSE
This course is a complete introduction to HTML, the foundational language of the web.
Designed for beginners, it covers the structure and semantics of web pages, from basic document setup to advanced HTML elements and accessibility best practices — without using CSS or JavaScript.
## TEACHING FLOW / Topics to be coverd

1. Basic Introduction
1. HTML Code Structure & Rules
2. Text semantics
3. Links/nav
4. Lists/grouping
5. Sectioning
6. Images
7. Tables
8. Forms
9. Disclosure elements
10. Advanced content models
11. Accessibility-first HTML
12. Validation
13. Capstone site assembly

## Basic Introduction to HTML

- **HTML** is an acronym for a web language called **"HyperText Markup Language"**.  
  It is **not** a programming language — instead, it is a markup language that describes the structure of a web page.

- In this course, we are learning the **latest version** of HTML, which is **HTML5**.

---

> **Callout (Question):** Why do we need this language? What does it do?  
> **Answer:**  
> HTML acts as the **skeleton** of every web page. It tells the browser **what** should be displayed and **in what order** — what comes first, what comes later, and what appears last.  
> It also gives **priority and emphasis** to certain parts of a page — for example, bold and large **headings** for important titles, smaller bold **subheadings** for section topics, and many other ways to mark up your content.

---

> **Question:** Why is that important?  
> **Answer:**  
> A well-structured HTML document is **crucial** for **SEO** (Search Engine Optimization).  
> Search engines like Google read your HTML to understand your page content.  
> If thousands of web pages share similar information, the ones with **better HTML structure** are often ranked higher in search results.  
> Good HTML improves:
> - **SEO ranking** (better position in search results)  
> - **Readability and structure** for visitors  
> - **Accessibility** for screen readers and assistive technologies

---

**In short:** HTML is the foundation of every website.  
Better HTML = Better structure, better SEO visibility, and a better user experience.



## HTML Code Structure & Rules  


## `<!DOCTYPE html>` Declaration in HTML
We are using **HTML5**, not older versions. While a few websites still use older HTML or XHTML doctypes, the browser needs to know which rules to follow.  
### How does the browser know the HTML version?  
The browser looks at the **first line** of the document — the **DOCTYPE declaration** — which tells it the correct rendering mode. For HTML5, use: `<!DOCTYPE html>`  
This differs for older versions, but HTML5 keeps it short and simple. It tells the browser: *Use standards mode (latest rules)*.  
> **Question:** What if I don’t include it?  
> **Anaswer:** The browser may use **quirks mode**, acting like very old browsers, causing inconsistent layouts.  
> **Questin:** What is quirks mode?  
> **Answer:** A legacy compatibility mode that can break design consistency. *Always* include the HTML5 doctype. Bsically it can render your multiple elements , tags in different different version/desgin/ways thats results in inconsistency in file rendering  
### Are these equivalent?  
``<!DOCTYPE html>`` and ``<!doctype html>`` → **Yes** ✅ HTML isn't case-insensitive. It literally means “Document type: html.”  
### Helpful Notes  
- Must be the **first line**, before `<html>`.  
- Not an HTML element; it’s an **instruction**.  
- Older doctypes referenced long DTDs; HTML5’s is intentionally short. 

## `<head>` Tag in HTML

The `<head>` tag is where we put all the stuff about our webpage — details about its setup, settings, and rules — things that **affect the page** but are **not shown directly to the user**.

---

### `<title>` Tag
- The `<title>` tag sets your webpage’s name for the browser.
- This is shown at the **top of your browser tab** (Chrome, Firefox, etc.).
- Also used in bookmarks and search engine results.

---

### `<meta>` Tag
- `<meta>` tags are **invisible to the user**, but they tell the browser how to handle and render your page.
- Common uses:
  - **Viewport settings** → how the page adapts to different screen sizes.
  - **Zoom control** → e.g., start at 100% zoom by default.
  - **Character set** → tells the browser which encoding to use (like `UTF-8` so you can use symbols like `&` and emoji and more).
  - **SEO info** → description, keywords, author name, and more.
- Think of `<meta>` as a set of instructions from the developer to the browser.

---

### `<link>` Tag
- Used to **connect external resources** to your webpage.
- Commonly used to attach:
  - CSS stylesheets.
  - Icons (favicon for browser tabs).
  - External resources
- Example:
  ```html
  <link rel="stylesheet" href="styles.css">
  ```
- This is like giving your webpage a **dress code** from another file.

---

### `<style>` Tag
- Lets you **write CSS directly inside the `<head>`**.
- Affects the appearance of your page.
- Usually for **small or page-specific styles** — larger styles go in a separate CSS file via `<link>`.
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
- Used to add JavaScript to your page.
- Can be **inline** (inside the tag) or linked from an external `.js` file.
- Placed in `<head>` if you want scripts to load **before** the page content runs (but sometimes better at the bottom of `<body>` for speed).
- Example:
  ```html
  <script src="app.js"></script>
  ```

---

💡 **Analogy**:  
The `<head>` is like a control room. You can’t see it when watching the “show” (webpage), but it’s where all the backstage crew — lighting, sound, scripts, and wardrobe — are set up so the performance goes perfectly.


## `<body>` Tag in HTML

The body is the part of an HTML document where all the content goes that can be directly seen by the user in the browser window.

---

### Key Points
- Holds everything visible on the webpage such as text, images, videos, buttons, forms, and more.
- Follows your order and sequence — the content written first will appear first on the page, followed by whatever comes next.
- Can be structured and formatted using HTML elements.

---

### What Can Go Inside
- Headings for titles and subtitles.
- Paragraphs for blocks of text.
- Lists for bullet points or numbered items.
- Links to navigate between pages or websites.
- Media such as images, video, audio, and vector graphics.
- Forms for user input.
- Tables for structured data.
- Interactive elements such as buttons and embedded content.

---

### Behavior
- The browser displays body content in the same order it is written in the HTML document.
- Content can be styled with CSS and made interactive with JavaScript.

---

💡 **Analogy**:  
If an HTML document were a play, the body would be the stage where all the actors (content) perform in the exact order the script describes.

## Strcuture of HTML page

![HTML file Structure](https://media.geeksforgeeks.org/wp-content/uploads/20240610121019/Screenshot-(4).png)

# 📚 Common HTML Tags by Category

---

## 📝 Text Formatting
- `<h1>` to `<h6>` — Headings (h1 is the largest, h6 is the smallest)
- `<p>` — Paragraph
- `<br>` — Line break
- `<hr>` — Horizontal rule (divider line)
- `<b>` — Bold text
- `<strong>` — Important text (semantic bold)
- `<i>` — Italic text
- `<em>` — Emphasized text (semantic italic)
- `<u>` — Underlined text
- `<mark>` — Highlighted text
- `<small>` — Smaller text
- `<sup>` — Superscript
- `<sub>` — Subscript

---

## 📄 Paragraphs & Structure
- `<div>` — Generic container (block-level)
- `<span>` — Generic inline container
- `<pre>` — Preformatted text (preserves spaces and line breaks)
- `<blockquote>` — Quoted section
- `<code>` — Inline code
- `<kbd>` — Keyboard input
- `<samp>` — Sample output
- `<var>` — Variable name in text

---

## 🔗 Links & Navigation
- `<a>` — Anchor/link
  - Attributes:
    - `href` — Destination URL
    - `target="_blank"` — Open in new tab
    - `title` — Tooltip text

---

## 🖼 Images & Multimedia
- `<img>` — Image
  - Attributes:
    - `src` — Image file path/URL
    - `alt` — Alternative text for accessibility
    - `width` / `height` — Size control
- `<figure>` — Container for image and caption
- `<figcaption>` — Caption for an image
- `<audio>` — Audio player
  - Attributes:
    - `src` — Audio file path/URL
    - `controls` — Display play/pause controls
- `<video>` — Video player
  - Attributes:
    - `src` — Video file path/URL
    - `controls` — Display controls
    - `poster` — Image shown before playback starts
- `<source>` — Alternative media source (used inside `<audio>` or `<video>`)
- `<iframe>` — Embed another webpage or video (e.g., YouTube)

---

## 📊 Tables
- `<table>` — Table container
- `<caption>` — Table title
- `<tr>` — Table row
- `<th>` — Table header cell
- `<td>` — Table data cell
- `<thead>` — Table head section
- `<tbody>` — Table body section
- `<tfoot>` — Table footer section
- `<col>` / `<colgroup>` — Column properties

---

## 📝 Forms & Input
- `<form>` — Form container
  - Attributes:
    - `action` — URL to send form data to
    - `method` — HTTP method (`GET` or `POST`)
- `<input>` — Various input fields
  - Common types: `text`, `password`, `email`, `number`, `checkbox`, `radio`, `file`, `submit`, `reset`
- `<textarea>` — Multi-line text input
- `<label>` — Label for form input
- `<select>` — Dropdown menu
- `<option>` — Option inside dropdown
- `<optgroup>` — Group of options inside dropdown
- `<button>` — Clickable button
- `<fieldset>` — Group related form controls
- `<legend>` — Caption for a `<fieldset>`
- `<datalist>` — List of predefined options for input
- `<output>` — Output value from a calculation or script

---









