
# 📘 JavaScript Learning Notes (For Django Developers)

## 📌 1. Basics
- What is JavaScript?
- How to include JS in HTML:
  ```html
  <script src="script.js"></script>
  ```
- Comments:
  ```js
  // Single-line comment
  /* Multi-line comment */
  ```

### ✨ Variables
- `let`, `const`, `var`
  ```js
  let name = "Jack";
  const PI = 3.14;
  ```

### 🎯 Data Types
- String, Number, Boolean, Null, Undefined, Object, Array

### 🔁 Operators
- Arithmetic: `+`, `-`, `*`, `/`, `%`
- Comparison: `==`, `===`, `!=`, `<`, `>`
- Logical: `&&`, `||`, `!`

## 📌 2. Control Structures
### ✅ Conditional Statements
```js
if (condition) { ... }
else if (...) { ... }
else { ... }
```

### 🔁 Loops
```js
for (let i = 0; i < 5; i++) { ... }
while (condition) { ... }
do { ... } while (condition);
```

## 📌 3. Functions
```js
function greet(name) {
  return "Hello " + name;
}
```

- Arrow functions:
```js
const greet = (name) => "Hello " + name;
```

## 📌 4. Arrays
```js
let fruits = ["apple", "banana"];
fruits.push("mango");
fruits.length;
```

- Common methods: `push()`, `pop()`, `shift()`, `unshift()`, `map()`, `filter()`, `forEach()`

## 📌 5. Objects
```js
let person = {
  name: "Jack",
  age: 23,
  speak: function () {
    console.log("Hi!");
  }
};
```

## 📌 6. DOM Manipulation (Essential for Django integration)
```js
document.getElementById("id")
document.querySelector(".class")
element.innerText
element.innerHTML
element.style.color = "blue"
```

- Event Listeners:
```js
button.addEventListener("click", function() {
  alert("Clicked!");
});
```

## 📌 7. Form Handling
- Get input value:
```js
document.getElementById("myInput").value
```
- Validate before submitting.

## 📌 8. Timers
```js
setTimeout(function() {
  alert("Hello after 3 seconds");
}, 3000);

setInterval(function() {
  console.log("Repeats every second");
}, 1000);
```

## 📌 9. JSON and LocalStorage
```js
let user = {name: "Jack", age: 23};
localStorage.setItem("user", JSON.stringify(user));
let data = JSON.parse(localStorage.getItem("user"));
```

## 📌 10. AJAX (With Django Views or APIs)
```js
fetch("/some-url/")
  .then(response => response.json())
  .then(data => {
    console.log(data);
  });
```

## 📌 11. ES6+ Features (Advanced but useful)
- Destructuring
- Spread/rest operators
- Template literals:
  ```js
  let name = "Jack";
  console.log(`Hello, ${name}`);
  ```
- Modules (`import`, `export`)

## 📌 12. (Bonus) Working with Django
- Use `<script>` inside your templates.
- For AJAX: Use Django views to return JSON and update the page without reloading.

## 📌 13. Tools
- Browser Developer Tools (Inspect > Console)
- Code Editor: VSCode
- JS Playground: [jsfiddle.net](https://jsfiddle.net), [codepen.io](https://codepen.io)

## ✅ Final Tip:
Start small—try adding JS to your Django templates (e.g., validating a form or showing a popup). Practice daily!
