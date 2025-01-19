## [What is the difference between map and forEach functions?](#what-is-the-difference-between-map-and-foreach-functions)

### What is the difference between `map` and `forEach` functions?

1. **Return Value:**
   - `map` returns a new array with the results of the callback function.
   - `forEach` does not return anything (undefined).

2. **Purpose:**
   - `map` is used when you want to transform each element in an array.
   - `forEach` is used when you want to perform side effects like logging or updating an external variable.

Example:
```javascript
const numbers = [1, 2, 3];

// map
const doubled = numbers.map(num => num * 2);
console.log(doubled); // [2, 4, 6]

// forEach
numbers.forEach(num => console.log(num * 2)); // Logs: 2, 4, 6
```

**Tags**: basic, JavaScript, Array Methods


