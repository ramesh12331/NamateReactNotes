# React & Web Concepts - Assignment

## 📌 Topics Covered
- What is Emmet?
- Difference between a Library and a Framework
- What is CDN? Why do we use it?
- Why is React known as React?
- What is `crossorigin` in script tag?
- What is the difference between React and ReactDOM?
- What is the difference between `react.development.js` and `react.production.js` files via CDN?
- What is `async` and `defer`?

---

## 🔹 What is Emmet?
Emmet is a **plugin/tool** that helps in writing HTML and CSS faster using short abbreviations that expand into full code snippets.  

👉 Example:  
Typing:
```html
div.container>ul>li*3

<div class="container">
  <ul>
    <li></li>
    <li></li>
    <li></li>
  </ul>
</div>


| Aspect      | Library                              | Framework                                         |
| ----------- | ------------------------------------ | ------------------------------------------------- |
| Control     | You call the library’s functions.    | Framework calls your code (Inversion of Control). |
| Flexibility | More flexible, can be used anywhere. | Less flexible, follows strict rules.              |
| Example     | React (UI library)                   | Angular (full framework)                          |

🔹 What is CDN? Why do we use it?

CDN (Content Delivery Network) is a distributed network of servers that delivers files (like JS, CSS, images) from the nearest server to the user.

✅ Benefits:

Faster load time

Reduces server load

Improves website performance globally

👉 Example:
<script src="https://cdn.jsdelivr.net/npm/react@18/umd/react.development.js"></script>

🔹 Why is React known as React?

React is called React because it reacts to changes in data and updates the UI automatically using its reactive rendering mechanism with the Virtual DOM.

🔹 What is crossorigin in script tag?

The crossorigin attribute is used when loading scripts from another domain (like a CDN).
It defines how browsers handle CORS (Cross-Origin Resource Sharing) for that script.

Types:

anonymous → No credentials sent.

use-credentials → Credentials like cookies sent.

👉 Example:

<script src="https://cdn.example.com/script.js" crossorigin="anonymous"></script>

🔹 Difference between React and ReactDOM

React → Core library for building UI components.

ReactDOM → Provides DOM-specific methods to render React components to the browser.

👉 Example:

import React from "react";
import ReactDOM from "react-dom/client";

const App = () => <h1>Hello World</h1>;
ReactDOM.createRoot(document.getElementById("root")).render(<App />);

🔹 Difference between react.development.js and react.production.js

react.development.js

Larger file size

Includes warnings and error messages

Used for debugging during development

react.production.js

Optimized and minified

No extra warnings

Better performance for deployment

🔹 What is async and defer?

Both are attributes used in <script> tag to control how scripts are loaded.

async

Script loads asynchronously with HTML parsing.

Executes immediately when loaded (can block rendering).

Best for independent scripts (ads, analytics).

defer

Script loads in background while HTML parses.

Executes after HTML parsing is complete.

Best for dependent scripts (like React, main.js).

👉 Example:

<script src="script.js" async></script>
<script src="script.js" defer></script>

📖 Summary

Emmet → Shortcuts for HTML/CSS.

Library vs Framework → Library = freedom, Framework = structure.

CDN → Delivers assets fast worldwide.

React → Named for its reactive UI updates.

crossorigin → Manages CORS for external scripts.

React vs ReactDOM → React = UI, ReactDOM = DOM rendering.

Development vs Production builds → Debugging vs Optimized.

async vs defer → Script loading strategies.

