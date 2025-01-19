## [How to detect if a function is called as a constructor](#how-to-detect-if-a-function-is-called-as-constructor)

### How to detect if a function is called as a constructor?

To detect if a function is called as a constructor, check the value of `this`. In a constructor call, `this` refers to the newly created object.

Example:

```javascript
function MyFunction() {
  if (!(this instanceof MyFunction)) {
    throw new Error('Must be called with new');
  }
  console.log('Called as constructor');
}

new MyFunction();  // Works
MyFunction();  // Throws error
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Functions](./theme/functions)


