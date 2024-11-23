### **What is CSS?**

- **CSS** stands for **Cascading Style Sheets**.
- It is used to control the style and layout of HTML elements, such as colors, fonts, spacing, and positioning.

---

### **Types of CSS**

1. **Inline CSS**

   - Written directly inside an HTML tag using the `style` attribute.
   - Example:
     ```html
     <h1 style="color: red;">Hello World</h1>
     ```

2. **Internal CSS**

   - Written inside the `<style>` tag in the `<head>` section of an HTML document.
   - Example:
     ```html
     <style>
       h1 {
         color: blue;
       }
     </style>
     ```

3. **External CSS**
   - Written in a separate file (e.g., `style.css`) and linked using the `<link>` tag.
   - Example:
     ```html
     <link rel="stylesheet" href="style.css" />
     ```

---

### **CSS Syntax**

```css
selector {
  property: value;
  property: value;
}
```

- **Selector**: Targets the HTML element(s) you want to style.
- **Property**: The style attribute (e.g., color, font-size).
- **Value**: The specific value for the property (e.g., red, 16px).

---

### **Common Selectors**

1. **Universal Selector**: Targets all elements.

   ```css
   * {
     margin: 0;
     padding: 0;
   }
   ```

2. **Type Selector**: Targets specific HTML tags.

   ```css
   h1 {
     color: green;
   }
   ```

3. **Class Selector**: Targets elements with a specific class (use `.`).

   ```css
   .card {
     background-color: #f0f0f0;
   }
   ```

4. **ID Selector**: Targets a specific element with a unique ID (use `#`).

   ```css
   #header {
     text-align: center;
   }
   ```

5. **Group Selector**: Targets multiple elements together.
   ```css
   h1,
   p,
   a {
     font-family: Arial, sans-serif;
   }
   ```

---

### **CSS Properties**

Here are some common CSS properties:

#### 1. **Text and Font**

- `color`: Sets the text color.

  ```css
  p {
    color: blue;
  }
  ```

- `font-size`: Sets the font size.

  ```css
  p {
    font-size: 16px;
  }
  ```

- `font-family`: Sets the font type.

  ```css
  body {
    font-family: Arial, sans-serif;
  }
  ```

- `text-align`: Aligns text (`left`, `center`, `right`, `justify`).
  ```css
  h1 {
    text-align: center;
  }
  ```

#### 2. **Box Model**

- Every element in CSS is a rectangular box and follows this model:

  - **Content** → **Padding** → **Border** → **Margin**.

- `margin`: Space outside the element.

  ```css
  div {
    margin: 20px;
  }
  ```

- `padding`: Space inside the element.

  ```css
  div {
    padding: 10px;
  }
  ```

- `border`: Defines the border around the element.
  ```css
  div {
    border: 2px solid black;
  }
  ```

#### 3. **Background**

- `background-color`: Sets the background color.

  ```css
  body {
    background-color: #f0f0f0;
  }
  ```

- `background-image`: Adds a background image.
  ```css
  body {
    background-image: url("image.jpg");
  }
  ```

---

### **Positioning**

- **Static** (default): Elements are positioned in the normal document flow.
- **Relative**: Position relative to its normal position.

  ```css
  div {
    position: relative;
    top: 10px;
  }
  ```

- **Absolute**: Positioned relative to its nearest positioned ancestor.

  ```css
  div {
    position: absolute;
    top: 50px;
    left: 20px;
  }
  ```

- **Fixed**: Positioned relative to the viewport (doesn’t move when scrolled).

  ```css
  div {
    position: fixed;
    bottom: 0;
  }
  ```

- **Flexbox**: A layout model for arranging elements.
  ```css
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  ```

---

### **Pseudo-Classes**

- Style an element based on its state.

  ```css
  a:hover {
    color: red;
  }

  input:focus {
    border: 2px solid blue;
  }
  ```

---

### **Responsive Design**

- Use **media queries** to apply styles based on screen size.
  ```css
  @media (max-width: 768px) {
    body {
      background-color: lightgray;
    }
  }
  ```

---

### **CSS Units**

- **Absolute**: `px`, `cm`, `mm`, etc.
- **Relative**: `em`, `rem`, `%`, `vh`, `vw`.

---

### **CSS Best Practices**

1. Use external CSS for scalability.
2. Name classes and IDs meaningfully (e.g., `.navbar`, `.footer`).
3. Use shorthand properties (e.g., `margin: 10px 20px;`).
4. Minimize the use of inline styles.
5. Test for cross-browser compatibility.

---
