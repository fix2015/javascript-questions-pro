## [What are compose and pipe functions?](#what-are-compose-and-pipe-functions)

### What are compose and pipe functions?

**Compose** and **pipe** are utility functions used in functional programming to combine multiple functions.

1. **Compose**:
   - Executes functions from right to left.

2. **Pipe**:
   - Executes functions from left to right.

Example:

```javascript
const add = x => x + 1;
const multiply = x => x * 2;

// Compose
const compose = (...fns) => x => fns.reduceRight((acc, fn) => fn(acc), x);
const composed = compose(multiply, add);
console.log(composed(5)); // 12

// Pipe
const pipe = (...fns) => x => fns.reduce((acc, fn) => fn(acc), x);
const piped = pipe(add, multiply);
console.log(piped(5)); // 12
```

**Tags**: advanced, JavaScript, Functional Programming


