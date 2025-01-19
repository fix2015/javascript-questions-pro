## [How to cancel a fetch request](#how-to-cancel-a-fetch-request)

### How to cancel a fetch request?

You can cancel a fetch request using an `AbortController`. The `AbortController` allows you to abort one or more fetch requests.

Example:

```javascript
let controller = new AbortController();
let signal = controller.signal;

fetch('https://api.example.com/data', { signal: signal })
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(err => console.log('Fetch aborted', err));

// To cancel the request
controller.abort();
```

**Tags**: advanced, JavaScript, Fetch API


