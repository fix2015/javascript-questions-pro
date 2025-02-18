## [How to catch errors with the Fetch API](#how-to-catch-errors-with-fetch-api)

### How to catch errors with the Fetch API

Use `.catch()` to handle errors when making HTTP requests with the Fetch API.

```javascript
fetch('https://api.example.com/data')
  .then(response => {
    if (!response.ok) {
      throw new Error('Network response was not ok');
    }
    return response.json();
  })
  .then(data => console.log(data))
  .catch(error => console.error('Fetch error:', error));
```

**Tags**: [beginner](./level/beginner), [JavaScript](./theme/javascript), [Fetch API](./theme/fetch_api), [Error Handling](./theme/error_handling)


