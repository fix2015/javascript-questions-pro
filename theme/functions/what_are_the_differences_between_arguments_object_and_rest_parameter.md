## [What are the differences between arguments object and rest parameter](#what-are-the-differences-between-arguments-object-and-rest-parameter)

### What are the differences between arguments object and rest parameter?

- **Arguments Object**:
  - Array-like object available in every non-arrow function.
  - Does not work with arrow functions.
  - Does not support array methods directly.

- **Rest Parameter**:
  - Collects arguments into a real array.
  - Works with all functions, including arrow functions.

Example:

```javascript
function oldStyleFunction() {
  console.log(arguments);  // Array-like
}

const newStyleFunction = (...args) => {
  console.log(args);  // Array
};

oldStyleFunction(1, 2, 3);
newStyleFunction(1, 2, 3);
```

**Tags**: intermediate, JavaScript, Functions


