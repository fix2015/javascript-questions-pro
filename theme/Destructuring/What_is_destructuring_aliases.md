## [What is destructuring aliases](#what-is-destructuring-aliases)

### What is destructuring aliases?

Destructuring aliases allow you to rename variables when destructuring an object or array. This is useful when the variable names in the object/array do not match your desired variable names.

Example:

```javascript
let person = { name: 'Alice', age: 25 };
let { name: fullName, age: yearsOld } = person;
console.log(fullName);  // Output: 'Alice'
console.log(yearsOld);  // Output: 25
```

**Tags**: intermediate, JavaScript, Destructuring


