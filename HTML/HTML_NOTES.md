> 💡 Key APIs in HTML5
> 
> - **Canvas API**
> - **Drag and Drop API**
> - **WebSocket API**

---

## What is HTML?

**HTML (Hypertext Markup Language)** is the standard language used to **structure webpages**. It defines how content on a webpage is structured and displayed.

### Key Features

- **Multimedia Support:** Embed audio/video without plugins.
- **New Form Controls:** Includes input types like `date`, `email`, etc.
- **Web Storage:** Store data offline.
- **Semantic Elements:** Tags like `<header>`, `<footer>` for better structure.
- **Improved Performance:** Optimized for mobile and modern web standards.

---

## Declaration

This tells the browser which **mode** to render the content in:

- **Standards Mode:** Renders per modern specs.
- **Quirks Mode:** Renders like older browsers.

> ⚠️ Note: <!DOCTYPE html> is not a tag and is not case-sensitive.
> 

**Validate HTML** → [W3C Validation Service](https://validator.w3.org/)

---

## 🏗 HTML Basic Document Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Title of the page</title>
  </head>
  <body>
    <!-- Page content here -->
  </body>
</html>

```

- `<html>`: Root element
- `<head>`: Metadata, title, links
- `<title>`: Appears in browser tab
- `<body>`: Visible content

---

## 🧱 HTML Headings

HTML provides 6 heading tags: `<h1>` to `<h6>`

- `<h1>` → Main heading (only one)
- `<h2>` → Sub-heading
- `<h3>` to `<h6>` → Deeper levels

> 🔍 Headings help in SEO and page structure.
> 

---

## 📑 Paragraph & Break

- `<p>` → Paragraph (has closing tag)
- `<br>` → Line break (no closing tag)

---

## ➖ Horizontal Line

- `<hr>` → Inserts a horizontal line (no closing tag)

---

## 💬 HTML Comments

```html
<!-- This is a comment -->

```

Used for documentation, not displayed in browser.

---

## 🖼 Images

```html
<img src="image.jpg" alt="Description">

```

- `src` → Image source
- `alt` → Alternate text

---

## 📊 Tables

```html
<table>
  <tr>
    <th>Heading</th>
    <td>Data</td>
  </tr>
</table>

```

- `<table>` → Table container
- `<tr>` → Table row
- `<th>` → Table header cell
- `<td>` → Table data cell

Other tags:

- `<caption>`
- `<colgroup>` / `<col>`
- `<tfoot>`

---

## 📝 Lists

### 🔹 Unordered List

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

```

### 🔸 Ordered List

```html
<ol>
  <li>Step 1</li>
  <li>Step 2</li>
</ol>

```

### 🔸 Description List

```html
<dl>
  <dt>Term</dt>
  <dd>Description</dd>
</dl>

```

### 🏷 List Tags

| Tag | Description |
| --- | --- |
| `<ul>` | Unordered List |
| `<ol>` | Ordered List |
| `<li>` | List Item |
| `<dl>` | Description List |
| `<dt>` | Term |
| `<dd>` | Description |

### ✅ List Attributes

- **Unordered List**:
    - `type` (circle, square, disc)
- **Ordered List**:
    - `start`, `reversed`, `type` (1, A, a, I, i)

> ⚠️ Note: compact is deprecated in HTML5.
> 

---

## 🧾 HTML Forms

```html
<form action="/submit" method="post">
  <input type="text" name="username">
  <input type="submit">
</form>

```

### 🔑 Form Attributes

- `action` → URL to send data to
- `method` → `get` or `post`
- `target` → where to show response
- `enctype` → encoding (used with `post`)
- `autocomplete` → on/off
- `novalidate` → disables validation

### 🧩 Form Elements

| Tag | Description |
| --- | --- |
| `<label>` | Defines label |
| `<input>` | User input field |
| `<textarea>` | Multi-line text |
| `<button>` | Clickable button |
| `<select>` | Dropdown list |
| `<option>` | Option in dropdown |
| `<optgroup>` | Group in dropdown |
| `<fieldset>` | Groups form elements |
| `<legend>` | Caption for fieldset |
| `<datalist>` | Predefined options |
| `<output>` | Calculation result |

### ✍ Input Types

| Type | Description |
| --- | --- |
| text | One-line text |
| password | Hidden input |
| submit | Submit form |
| reset | Reset form |
| email | Email validation |
| number | Numeric input |
| checkbox | Multi-choice |
| radio | Single choice |
| date | Date picker |
| time | Time picker |
| file | File upload |

---

## 🛠 View HTML Source Code

- Right-click → Inspect / View Page Source
- Or press **`F12`** to open DevTools

---

## HTML Block and Inline Elements

[](data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%2732%27%20height=%2732%27/%3e)

HTML elements are either block-level, which structure the layout and [span](https://www.geeksforgeeks.org/html/html-span-tag/) full width (like [`<div>`](https://www.geeksforgeeks.org/html/div-tag-html/) or [`<p>`](https://www.geeksforgeeks.org/html/html-p-tag/)), or inline, which styles content within blocks without breaking the flow (like `<span>` or `<a>`). This distinction covers 80–90% of common [HTML](https://www.geeksforgeeks.org/html/html-tutorial/) usage.

![image.png](attachment:1fdbfd59-64b3-462c-b43d-4394e6300681:image.png)

---

## HTML File Paths

[](data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%2732%27%20height=%2732%27/%3e)

**HTML file paths** specify the location of files or resources that a webpage needs to access, such as images, videos, scripts, or other HTML documents.

### **Types of File Paths →**

1.  **Absolute File Paths →**
- Point directly to a resource's location on the internet and include the full URL, which consists of the protocol (`http://` or `https://`), domain, and path to the resource.
- Best for resources that are hosted externally. The browser knows exactly where to find them regardless of the current document’s location.

1. **Relative File Paths →**
- Specify the path to a resource in relation to the location of the HTML file currently being viewed.
- Ideal for resources within the same website. Keeps your HTML portable if the domain changes since the path doesn’t need to be updated.

**Relative Path Variants →**

- **Document-relative paths**: As in the above example, the path starts from the directory of the current HTML document.
- **Root-relative paths**: Start with a slash (`/`), which tells the browser to look for the resource starting from the root directory of the server. Example:

---

## HTML Viewport meta tag for Responsive Web Design

**A Browser's viewport** is the area of the web page in which the content is visible to the user. The viewport does not have the same size, it varies with the variation in screen size of the devices on which the website is visible

- The ' **`width=device-width** '` in meta tag sets the width of the page to follow the screen width of the device, which will vary depending on the device.
- The ' **`initial-scale=1.0`** ' in meta tag sets the initial zoom level when the page is first loaded by the browser.

## HTML DOM (Document Object Model)

The **HTML DOM (Document Object Model)** is the foundation of modern web interactivity, enabling over 90% of dynamic behavior seen on [websites](https://www.geeksforgeeks.org/blogs/what-is-a-website/) today.

### **What Does the HTML DOM Look Like?**

**Imagine your webpage as a tree**

- The document is the root.
- HTML tags like <html>, <head>, and <body> are branches.
- Attributes, text, and other elements are the leaves.

### **Why is DOM Required?**

**The DOM is essential because**

- **Dynamic Content Updates:** Without reloading the page, the DOM allows content updates (e.g., form validation, AJAX responses).
- **User Interaction:** It makes your webpage interactive (e.g., responding to button clicks, form submissions).
- **Flexibility:** Developers can add, modify, or remove elements and styles in real-time.
- **Cross-Platform Compatibility:** It provides a standard way for scripts to interact with web documents, ensuring browser compatibility.

### **DOM Data Types**

When working with the DOM (Document Object Model), there are different types of data or building blocks used behind the scenes. Here’s what they mean in everyday terms:

- **Document**: Think of it as the entire webpage. It's like the starting point or the big box that holds everything you see on a website.
- **Node**: Anything on the webpage—like a heading, paragraph, image, or even some hidden parts—is called a node. It’s like a small part or piece of the whole page.
- **Element**: This is a specific type of node. It represents actual tags you write in HTML, like `<div>`, `<p>`, or `<img>`. These are the visible parts of the page.
- **NodeList**: Imagine you ask the page to give you all the buttons or all the paragraphs—it gives you a list of those items. That list is called a NodeList. It's like a group of nodes stored together.

### **Commonly Used DOM Methods**

| Methods | Description |
| --- | --- |
| [getElementById(id)](https://www.geeksforgeeks.org/html/html-dom-getelementbyid-method/) | Selects an element by its ID. |
| [getElementsByClassName(class)](https://www.geeksforgeeks.org/javascript/html-dom-getelementsbyclassname-method/) | Selects all elements with a given class. |
| [querySelector(selector)](https://www.geeksforgeeks.org/html/html-dom-queryselector-method/) | Selects the first matching element. |
| [querySelectorAll(selector)](https://www.geeksforgeeks.org/html/html-dom-queryselectorall-method/) | Selects all matching elements. |
| [createElement(tag)](https://www.geeksforgeeks.org/javascript/html-dom-createelement-method/) | Creates a new HTML element. |
| [appendChild(node)](https://www.geeksforgeeks.org/html/html-dom-appendchild-method/) | Adds a child node to an element. |
| [remove()](https://www.geeksforgeeks.org/html/html-dom-select-remove-method/) | Removes an element from the DOM. |
| [addEventListener(event, fn)](https://www.geeksforgeeks.org/javascript/html-dom-addeventlistener-method/) | Attaches an event handler to an element. |