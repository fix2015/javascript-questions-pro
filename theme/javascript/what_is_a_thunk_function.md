## [What is a thunk function](#what-is-a-thunk-function)

### What is a thunk function?

A thunk function is a function that wraps another function or expression, typically used to delay the execution of the original function. It is often used in functional programming to manage side effects or control execution order.

Example:

```javascript
const add = (a, b) => a + b;
const thunk = (a, b) => () => add(a, b);
const result = thunk(2, 3)();  // Output: 5
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Functional Programming](./theme/functional_programming)


