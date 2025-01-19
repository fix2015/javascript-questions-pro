## [What are the different error names from error object](#what-are-the-different-error-names-from-error-object)

### What are the different error names from error object?

JavaScript provides several types of error objects:

- `Error` – General errors
- `SyntaxError` – Syntax issues in code
- `ReferenceError` – Reference to a non-existent variable
- `TypeError` – Wrong data type used
- `RangeError` – A value is out of range
- `EvalError` – Issues with `eval()` function

Example:

```javascript
try {
  let x = y;
} catch (e) {
  console.log(e instanceof ReferenceError); // true
}
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [errors](./theme/errors)


