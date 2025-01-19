## [How do you get unique values of an array](#how-do-you-get-unique-values-of-an-array)

### How do you get unique values of an array?

To get unique values from an array, you can use `Set`, which stores only unique values. You can also use `filter()` and `indexOf()` to remove duplicates.

Example:

```javascript
let arr = [1, 2, 2, 3, 4, 4, 5];
let uniqueArr = [...new Set(arr)];
console.log(uniqueArr);  // Output: [1, 2, 3, 4, 5]
```

**Tags**: intermediate, JavaScript, Arrays


