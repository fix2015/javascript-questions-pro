## [What is the purpose of the this keyword in JavaScript?](#what-is-the-purpose-of-the-this-keyword-in-javascript)

### What is the purpose of the `this` keyword in JavaScript?

The `this` keyword refers to the object that is executing the current function. Its value depends on how the function is called:

1. **In a Method:** Refers to the object the method belongs to.
2. **In a Function (non-strict mode):** Refers to the global object (`window` in browsers).
3. **In a Function (strict mode):** Undefined.
4. **In Arrow Functions:** Inherits `this` from the enclosing scope.

Example:

```javascript
const obj = {
  name: 'Alice',
  greet() {
    console.log(`Hello, ${this.name}`);
  }
};

obj.greet(); // 'Hello, Alice'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Scope](./theme/scope)


