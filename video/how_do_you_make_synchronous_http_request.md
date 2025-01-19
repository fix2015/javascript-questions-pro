## [How do you make synchronous HTTP request](#how-do-you-make-synchronous-http-request)

### How do you make synchronous HTTP request?

You can make a synchronous HTTP request using `XMLHttpRequest` with `open()` and `send()` methods, and setting the `async` parameter to `false`.

Example:

```javascript
const xhr = new XMLHttpRequest();
xhr.open('GET', 'https://api.example.com', false);
xhr.send();
console.log(xhr.responseText);
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [HTTP requests](./theme/http_requests)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457614380205739296](https://www.tiktok.com/@jsmentoring/photo/7457614380205739296)
