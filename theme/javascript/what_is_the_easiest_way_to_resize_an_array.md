## [What is the easiest way to resize an array](#what-is-the-easiest-way-to-resize-an-array)

### What is the easiest way to resize an array?

The easiest way to resize an array is by using the `length` property. You can truncate the array or expand it by setting its length.

Example:

```javascript
let arr = [1, 2, 3];
arr.length = 2;  // Truncate the array
console.log(arr);  // Output: [1, 2]
arr.length = 5;  // Expand the array
console.log(arr);  // Output: [1, 2, <3 empty slots>]

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Arrays](./theme/arrays)


