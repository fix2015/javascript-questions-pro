## [How do you compare scalar arrays](#how-do-you-compare-scalar-arrays)

### How do you compare scalar arrays?

To compare scalar arrays (arrays with primitive data types) in JavaScript, you need to check if both arrays have the same length and if each element is equal. You can do this using loops or `Array.prototype.every()`.

Example:

```javascript
const arr1 = [1, 2, 3];
const arr2 = [1, 2, 3];
const areArraysEqual = arr1.length === arr2.length && arr1.every((val, index) => val === arr2[index]);
console.log(areArraysEqual); // true
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [arrays](./theme/arrays)


