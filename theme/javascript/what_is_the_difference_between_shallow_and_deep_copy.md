## [What is the difference between Shallow and Deep copy](#what-is-the-difference-between-shallow-and-deep-copy)

### What is the difference between Shallow and Deep copy?

A shallow copy copies only the top-level properties of an object or array, meaning nested objects or arrays are shared. A deep copy copies all properties, including nested ones, so that no references to the original object exist.

Example of shallow copy:

```javascript
let arr = [1, [2, 3]];
let shallowCopy = arr.slice();
shallowCopy[1][0] = 99;
console.log(arr);  // Output: [1, [99, 3]]
```

Example of deep copy (using `JSON.parse()` and `JSON.stringify()`):

```javascript
let deepCopy = JSON.parse(JSON.stringify(arr));
deepCopy[1][0] = 100;
console.log(arr);  // Output: [1, [99, 3]]
console.log(deepCopy);  // Output: [1, [100, 3]]
```

**Tags**: intermediate, JavaScript, Objects


