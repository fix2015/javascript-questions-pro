## [What is the purpose of using object is method](#what-is-the-purpose-of-using-object-is-method)

### What is the purpose of using Object.is method?

`Object.is()` is used to compare two values to check if they are the same. It is similar to `===` but handles special cases like `NaN` and `-0` differently.

Example:

```javascript
console.log(Object.is(-0, +0)); // false
console.log(Object.is(NaN, NaN)); // true
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


