# JavaScript DOM Manipulation Documentation

## 📌 What is the DOM?

The **DOM (Document Object Model)** is the structure of an HTML document in memory. JavaScript uses the DOM to dynamically access and manipulate content, structure, and styling.

---

## 🧱 Basic DOM Tasks

| Task                    | Example Used                                  | Description                                              |
| ----------------------- | --------------------------------------------- | -------------------------------------------------------- |
| **Access Elements**     | `getElementById`, `querySelector`             | Select HTML elements using their ID, class, tag, etc.    |
| **Change Content**      | `element.innerHTML = "New Content"`           | Modify the inner HTML or text of an element.             |
| **Change Styles**       | `element.style.backgroundColor = "blue"`      | Directly update the CSS of elements using `.style`.      |
| **Respond to Events**   | `addEventListener("click", function)`         | Run JavaScript when users interact (e.g., click, hover). |
| **Create/Remove Nodes** | `createElement`, `appendChild`, `removeChild` | Dynamically add or remove HTML elements.                 |

---

## 🔍 1. Access Elements

### Examples:

```js
const title = document.getElementById("main-title");
const button = document.querySelector(".btn-primary");
```

---

## ✏️ 2. Change Content

### Example:

```js
document.getElementById("output").innerHTML = "Updated content here!";
```

---

## 🎨 3. Change Styles

### Example:

```js
const box = document.querySelector(".box");
box.style.border = "2px solid red";
box.style.backgroundColor = "lightyellow";
```

---

## 🎯 4. Respond to Events

### Example:

```js
const btn = document.getElementById("clickMe");
btn.addEventListener("click", function() {
  alert("Button was clicked!");
});
```

---

## ➕➖ 5. Create / Remove Elements

### Example - Add Element:

```js
const newPara = document.createElement("p");
newPara.textContent = "This is a new paragraph.";
document.body.appendChild(newPara);
```

### Example - Remove Element:

```js
const oldPara = document.getElementById("old-paragraph");
oldPara.remove();
```

---

## ✅ Summary

The DOM allows JavaScript to make your webpages interactive and dynamic. Mastering the above tasks lets you build powerful, responsive frontends.

---

Would you like to extend this doc to include form handling, animation, or local storage next?
