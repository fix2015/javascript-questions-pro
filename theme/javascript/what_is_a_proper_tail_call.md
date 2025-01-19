## [What is a Proper Tail Call](#what-is-a-proper-tail-call)

### What is a Proper Tail Call?

A Proper Tail Call (PTC) is a feature where the last action of a function is a call to another function, and the current function's stack frame is removed before executing the called function. This optimization prevents stack overflow errors for recursive calls.

Example:

```javascript
function factorial(n, acc = 1) {
  if (n === 0) return acc;
  return factorial(n - 1, acc * n);  // Tail call
}
console.log(factorial(5));  // Output: 120
```

**Tags**: advanced, JavaScript, Optimization


