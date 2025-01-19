## [What are the differences between spread operator and rest parameter](#what-are-the-differences-between-spread-operator-and-rest-parameter)

### What are the differences between spread operator and rest parameter?

- **Spread Operator**:
  - Expands elements of an array or object into individual elements.
  - Used in function calls, array literals, or object literals.

- **Rest Parameter**:
  - Collects all remaining arguments into a single array.
  - Used in function definitions.

Example:

```javascript
// Spread Operator
const numbers = [1, 2, 3];
console.log(...numbers); // Output: 1 2 3

// Rest Parameter
function sum(...args) {
  return args.reduce((acc, curr) => acc + curr, 0);
}
console.log(sum(1, 2, 3)); // Output: 6
```

**Tags**: intermediate, JavaScript, Operators


