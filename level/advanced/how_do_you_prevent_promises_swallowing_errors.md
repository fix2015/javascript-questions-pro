## [How do you prevent promises swallowing errors](#how-do-you-prevent-promises-swallowing-errors)

### How do you prevent promises from swallowing errors?

To prevent promises from swallowing errors, ensure that you handle rejections using `.catch()` or use `try-catch` with `async-await` syntax. Additionally, always return or throw errors explicitly.

Example:

```javascript
Promise.resolve()
  .then(() => { throw new Error('Error occurred'); })
  .catch(error => console.error('Caught error:', error));

async function asyncFunction() {
  try {
    await Promise.reject('Error occurred');
  } catch (error) {
    console.error('Caught error:', error);
  }
}
asyncFunction();
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Promises](./theme/promises)


