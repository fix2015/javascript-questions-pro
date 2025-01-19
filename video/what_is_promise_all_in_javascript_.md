## [What Is `Promise.all` in JavaScript?](#what-is-promise-all-in-javascript)

### What Is `Promise.all` in JavaScript?

`Promise.all` is a method that accepts an array of promises and returns a single promise that resolves when all the promises in the array are resolved. If any of the promises reject, the returned promise will reject immediately.

```javascript
Promise.all([promise1, promise2, promise3])
  .then(results => console.log(results))
  .catch(error => console.error(error));
```

**Tags**: [intermediate](./level/intermediate), [Promises](./theme/promises), [JavaScript](./theme/javascript), [asynchronous programming](./theme/asynchronous_programming)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7449321820743847200](https://www.tiktok.com/@jsmentoring/photo/7449321820743847200)
