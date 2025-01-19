## [How to verify if a variable is an array?](#how-to-verify-if-a-variable-is-an-array)

### How to verify if a variable is an array?

You can verify if a variable is an array using `Array.isArray()` method. It returns `true` if the value is an array, otherwise `false`.

Example:

```javascript
const arr = [1, 2, 3];
console.log(Array.isArray(arr)); // true

const obj = { key: 'value' };
console.log(Array.isArray(obj)); // false
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Data Types](./theme/data_types)


