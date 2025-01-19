## [Does the const variable make the value immutable](#does-the-const-variable-make-the-value-immutable)

### Does the `const` variable make the value immutable?

No, `const` only ensures that the variable identifier cannot be reassigned. It does not make the value immutable. If the value is an object or array, its properties or elements can still be modified.

Example:

```javascript
const arr = [1, 2, 3];
arr.push(4);  // Works fine
arr = [4, 5, 6];  // Error: Assignment to constant variable
```

**Tags**: intermediate, JavaScript, Variables


