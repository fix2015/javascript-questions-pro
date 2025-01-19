## [What is referential transparency?](#what-is-referential-transparency)

### What is referential transparency?

A function is referentially transparent if it can be replaced with its output value without changing the program's behavior. It is a key property of pure functions.

Example:

```javascript
// Referentially Transparent
function add(a, b) {
  return a + b;
}

const result = add(2, 3); // Can replace 'add(2, 3)' with 5
console.log(result); // 5

// Not Referentially Transparent
let count = 0;
function increment() {
  return ++count;
}
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Functional Programming](./theme/functional_programming)


