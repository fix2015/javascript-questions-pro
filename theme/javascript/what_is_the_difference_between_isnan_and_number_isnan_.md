## [What is the difference between isNaN and Number.isNaN?](#what-is-the-difference-between-isnan-and-numberisnan)

### What is the difference between isNaN and Number.isNaN?

- **`isNaN`**:
  - Converts the input to a number and checks if it's `NaN`.
  - May give misleading results for non-number inputs.

- **`Number.isNaN`**:
  - Checks strictly if the value is `NaN`.
  - Doesn't coerce the input.

Example:

```javascript
console.log(isNaN('hello')); // true (coerced to NaN)
console.log(Number.isNaN('hello')); // false (strict check)
```

**Tags**: basic, JavaScript, Numbers


