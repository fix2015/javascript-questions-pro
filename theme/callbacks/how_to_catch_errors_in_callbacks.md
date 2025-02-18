## [How to catch errors in callbacks](#how-to-catch-errors-in-callbacks)

### How to catch errors in callbacks

When working with callbacks, ensure that errors are passed as the first argument to the callback function.

```javascript
function performAsyncOperation(callback) {
  // Simulate error
  const error = new Error('Something went wrong');
  callback(error, null);
}

performAsyncOperation((error, result) => {
  if (error) {
    return console.error('Callback error:', error);
  }
  console.log(result);
});
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Callbacks](./theme/callbacks), [Error Handling](./theme/error_handling)


