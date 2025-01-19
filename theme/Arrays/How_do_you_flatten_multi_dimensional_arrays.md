## [How do you flatten multi dimensional arrays](#how-do-you-flattening-multi-dimensional-arrays)

### How do you flatten multi-dimensional arrays?

You can flatten multi-dimensional arrays using the `flat()` method in JavaScript. This method flattens an array up to a specified depth.

Example:

```javascript
let arr = [1, [2, 3], [4, [5, 6]]];
let flattened = arr.flat(2);
console.log(flattened);  // Output: [1, 2, 3, 4, 5, 6]
```

**Tags**: intermediate, JavaScript, Arrays


