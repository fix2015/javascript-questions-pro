## [What are the differences between pure and impure functions?](#what-are-the-differences-between-pure-and-impure-functions)

### What are the differences between pure and impure functions?

**Pure Functions**:
- Always return the same output for the same input.
- No side effects (e.g., modifying global variables or external state).

**Impure Functions**:
- Output depends on external factors or internal state.
- May produce side effects.

Example:

```javascript
// Pure Function
function add(a, b) {
  return a + b;
}

// Impure Function
let count = 0;
function increment() {
  count++;
  return count;
}
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Functional Programming](./theme/functional_programming)


