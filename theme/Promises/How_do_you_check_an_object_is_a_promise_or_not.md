## [How do you check an object is a promise or not](#how-do-you-check-an-object-is-a-promise-or-not)

### How do you check if an object is a promise or not?

To check if an object is a promise, verify that it is an object with a `then` method that is a function.

Example:

```javascript
function isPromise(obj) {
  return !!obj && typeof obj.then === 'function';
}

console.log(isPromise(Promise.resolve()));  // Output: true
console.log(isPromise({}));  // Output: false
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Promises](./theme/promises)


