## [What happens with negating an array](#what-happens-with-negating-an-array)

### What happens with negating an array?

When you negate an array in JavaScript, it is first converted to a primitive value, which is `true` when the array is non-empty and `false` when the array is empty. Negating it results in `false` for non-empty arrays and `true` for empty arrays.

Example:

```javascript
let arr = [1, 2, 3];
console.log(!arr);  // Output: false
arr = [];
console.log(!arr);  // Output: true
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays)


