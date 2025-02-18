## [How to catch errors in async/await](#how-to-catch-errors-in-async-await)

### How to catch errors in async/await

Wrap your async code in a try/catch block to handle errors gracefully.

```javascript
async function fetchData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}
fetchData();
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Async/Await](./theme/async_await), [Error Handling](./theme/error_handling)


