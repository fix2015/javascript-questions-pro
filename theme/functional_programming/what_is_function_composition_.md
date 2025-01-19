## [What is Function Composition?](#what-is-function-composition)

### What is Function Composition?

Function composition is the process of combining two or more functions to produce a new function. The output of one function becomes the input of the next.

Example:

```javascript
const add = x => x + 1;
const multiply = x => x * 2;

const compose = (...fns) => x => fns.reduceRight((acc, fn) => fn(acc), x);

const composed = compose(multiply, add);
console.log(composed(5)); // 12
```

**Tags**: advanced, JavaScript, Functional Programming


