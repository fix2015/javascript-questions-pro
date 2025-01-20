## [Why do you need to avoid with statement](#why-do-you-need-to-avoid-with-statement)

### Why do you need to avoid `with` statement?

The `with` statement is considered problematic because it makes the code harder to understand and maintain. It adds variables from an object to the scope, which can lead to confusion and unexpected behavior, especially in larger programs.

It is recommended to avoid using `with` in modern JavaScript.

Example:

```javascript
with (Math) {
  console.log(sqrt(16));  // Works, but avoid it
}
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Best Practices](./theme/best_practices)


