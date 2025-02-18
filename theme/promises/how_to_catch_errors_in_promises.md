## [How to catch errors in Promises](#how-to-catch-errors-in-promises)

### How to catch errors in Promises

You can handle errors in promises by appending a `.catch()` method to the promise chain.

```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

**Tags**: [beginner](./level/beginner), [JavaScript](./theme/javascript), [Promises](./theme/promises), [Error Handling](./theme/error_handling)


