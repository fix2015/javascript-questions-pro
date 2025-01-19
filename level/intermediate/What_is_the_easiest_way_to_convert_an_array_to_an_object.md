## [What is the easiest way to convert an array to an object](#what-is-the-easiest-way-to-convert-an-array-to-an-object)

### What is the easiest way to convert an array to an object?

You can use `reduce()` to convert an array into an object, where each element becomes a key-value pair.

Example:

```javascript
let arr = ['apple', 'banana', 'cherry'];
let obj = arr.reduce((acc, curr, index) => {
  acc[index] = curr;
  return acc;
}, {});
console.log(obj);  // Output: { 0: 'apple', 1: 'banana', 2: 'cherry' }
```

**Tags**: intermediate, JavaScript, Arrays


