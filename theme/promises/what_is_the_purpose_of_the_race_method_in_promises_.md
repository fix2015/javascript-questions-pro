## [What Is the Purpose of the `race` Method in Promises?](#what-is-the-purpose-of-the-race-method-in-promises)

### What Is the Purpose of the `race` Method in Promises?

The `Promise.race()` method returns a promise that resolves or rejects as soon as one of the promises in the iterable resolves or rejects. It is useful when you need to wait for the first promise to settle.

```javascript
Promise.race([promise1, promise2, promise3])
  .then(result => console.log(result))
  .catch(error => console.error(error));
```

**Tags**: intermediate, Promises, JavaScript, asynchronous programming

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7449363438461144353](https://www.tiktok.com/@jsmentoring/photo/7449363438461144353)
