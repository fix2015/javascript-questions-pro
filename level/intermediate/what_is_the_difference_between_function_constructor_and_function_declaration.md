## [What is the difference between Function constructor and function declaration](#what-is-the-difference-between-function-constructor-and-function-declaration)

### What is the difference between Function constructor and function declaration?

- **Function Declaration**: A function declared using the `function` keyword and is hoisted, meaning it is available throughout the scope.

```javascript
function greet() { console.log('Hello'); }
```

- **Function Constructor**: A function created using the `Function` constructor. This approach is less commonly used and has a few limitations, such as not allowing for closures.

```javascript
let greet = new Function('console.log("Hello")');
```

**Tags**: intermediate, JavaScript, Functions


