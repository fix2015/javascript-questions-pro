## [What is pass by value and pass by reference?](#what-is-pass-by-value-and-pass-by-reference)

### What is pass by value and pass by reference?

In JavaScript:

1. **Pass by Value**:
   - For **primitives** (e.g., numbers, strings), the value is copied.
   - Changes to the copied variable do not affect the original.

2. **Pass by Reference**:
   - For **objects and arrays**, a reference to the memory location is passed.
   - Changes to the reference affect the original object.

Example:

```javascript
let x = 10; // Primitive
let y = x;
y = 20;
console.log(x); // 10 (pass by value)

let obj1 = { key: 'value' }; // Non-primitive
let obj2 = obj1;
obj2.key = 'newValue';
console.log(obj1.key); // 'newValue' (pass by reference)
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Memory Management](./theme/memory_management)


