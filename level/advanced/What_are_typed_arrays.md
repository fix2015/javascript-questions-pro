## [What are typed arrays](#what-are-typed-arrays)

### What are typed arrays?

Typed arrays are arrays that allow you to work with binary data. They provide a mechanism for dealing with raw binary data buffers in JavaScript, offering various array-like objects that represent different binary data formats.

Example:

```javascript
let buffer = new ArrayBuffer(16);
let int32View = new Int32Array(buffer);
int32View[0] = 42;
console.log(int32View[0]);  // Output: 42
```

**Tags**: advanced, JavaScript, Arrays


