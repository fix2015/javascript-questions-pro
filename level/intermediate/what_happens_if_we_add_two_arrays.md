## [What happens if we add two arrays](#what-happens-if-we-add-two-arrays)

### What happens if we add two arrays?

In JavaScript, adding two arrays does not perform element-wise addition. Instead, it concatenates them into a new array, but if you add them directly, it will convert them to strings and concatenate those.

Example:

```javascript
let arr1 = [1, 2, 3];
let arr2 = [4, 5, 6];
console.log(arr1 + arr2);  // Output: '1,2,34,5,6'
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays)


