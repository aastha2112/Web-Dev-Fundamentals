## **1. What is HTML?**

- **HTML (HyperText Markup Language)**: The standard language for creating and structuring content on the web.
- It is used to define the structure of a webpage using **tags**.
- A web browser interprets HTML to render the content as a visually structured webpage.

---

## **2. Basic Structure of an HTML Document**

An HTML document starts with a **declaration** and consists of various **elements**:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is a paragraph of text.</p>
  </body>
</html>
```

### Explanation:

- **`<!DOCTYPE html>`**: Declares the document as HTML5.
- **`<html>`**: The root element containing all content.
- **`<head>`**: Contains metadata like the page title, character encoding, links to CSS, or scripts.
- **`<title>`**: Defines the title shown on the browser tab.
- **`<body>`**: Contains the visible content displayed on the webpage.

---

## **3. Common HTML Tags**

Here are frequently used tags along with their purpose:

### **Text Content**

- **Headings**: `<h1>` to `<h6>` tags represent headings (h1 is the largest, h6 is the smallest).
  ```html
  <h1>Main Heading</h1>
  <h2>Subheading</h2>
  ```
- **Paragraph**: `<p>` defines a block of text.
  ```html
  <p>This is a paragraph.</p>
  ```
- **Line Break**: `<br>` adds a single line break (no closing tag).
- **Bold/Italic**:
  ```html
  <strong>Bold text</strong> <em>Italicized text</em>
  ```

### **Links and Images**

- **Links**: `<a>` creates a hyperlink.
  ```html
  <a href="https://example.com">Visit Example</a>
  ```
- **Images**: `<img>` embeds an image.
  ```html
  <img src="image.jpg" alt="Image description" />
  ```

### **Lists**

- **Unordered List (Bullet points)**:
  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
  </ul>
  ```
- **Ordered List (Numbered)**:
  ```html
  <ol>
    <li>Step 1</li>
    <li>Step 2</li>
  </ol>
  ```

### **Tables**

- Create tables to display data in rows and columns:
  ```html
  <table>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </table>
  ```

### **Forms**

- Forms are used to collect user input.
  ```html
  <form action="/submit" method="POST">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required />
    <button type="submit">Submit</button>
  </form>
  ```

---

## **4. Attributes**

Attributes add extra information to elements. They are written inside the opening tag as `name="value"`.

### Common Attributes:

- **`id`**: Unique identifier for an element.
  ```html
  <div id="header"></div>
  ```
- **`class`**: Groups multiple elements for styling or behavior.
  ```html
  <p class="important">Highlighted Text</p>
  ```
- **`src`**: Specifies the source (for images, videos, etc.).
  ```html
  <img src="image.jpg" alt="Description" />
  ```
- **`href`**: Specifies the link destination (for `<a>` tags).
  ```html
  <a href="https://example.com">Go to Example</a>
  ```
- **`style`**: Inline styling (use CSS for better practice).
  ```html
  <p style="color: blue;">Blue Text</p>
  ```

---

## **5. Semantic HTML**

Semantic tags provide meaningful structure and improve accessibility and SEO:

- **Examples of Semantic Tags**:
  - `<header>`: Defines a page or section header.
  - `<footer>`: Defines the footer of a document or section.
  - `<nav>`: Represents navigation links.
  - `<article>`: Self-contained content.
  - `<section>`: Defines a thematic grouping of content.

```html
<header>
  <h1>Welcome to My Website</h1>
</header>
<nav>
  <a href="#about">About</a>
  <a href="#contact">Contact</a>
</nav>
<section>
  <h2>About Us</h2>
  <p>We provide high-quality services.</p>
</section>
<footer>
  <p>&copy; 2024 My Website</p>
</footer>
```

---

## **6. Multimedia Elements**

HTML supports embedding multimedia like audio and video:

- **Audio**:
  ```html
  <audio controls>
    <source src="audio.mp3" type="audio/mpeg" />
    Your browser does not support the audio element.
  </audio>
  ```
- **Video**:
  ```html
  <video controls width="500">
    <source src="video.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
  ```

---

## **7. Best Practices**

1. **Use Semantic HTML**: Makes your code easier to read and more accessible.
2. **Include Alt Text**: Always provide `alt` attributes for images to describe them.
3. **Avoid Inline Styles**: Keep styling in CSS files for better maintainability.

---
