## [How do you remove falsy values from an array](#how-do-you-remove-falsy-values-from-an-array)

### How do you remove falsy values from an array?

You can use the `filter()` method to remove falsy values (e.g., `false`, `null`, `undefined`, `0`, `NaN`, `""`) from an array.

Example:

```javascript
let arr = [0, 1, false, 2, '', 3, null];
let filteredArr = arr.filter(Boolean);
console.log(filteredArr);  // Output: [1, 2, 3]
```

**Tags**: basic, JavaScript, Arrays


