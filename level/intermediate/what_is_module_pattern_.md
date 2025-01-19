## [What is module pattern?](#what-is-module-pattern)

### What is the Module Pattern?

The Module Pattern is a design pattern used to encapsulate private and public variables and methods. It provides a way to create a namespace and control access to certain parts of code.

Example:

```javascript
const myModule = (function() {
  let privateVar = 'I am private';

  function privateMethod() {
    console.log(privateVar);
  }

  return {
    publicMethod: function() {
      privateMethod();
    }
  };
})();

myModule.publicMethod(); // 'I am private'
console.log(myModule.privateVar); // undefined
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Design Patterns](./theme/design_patterns)


