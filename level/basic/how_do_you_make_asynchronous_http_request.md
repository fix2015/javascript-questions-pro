## [How do you make asynchronous HTTP request](#how-do-you-make-asynchronous-http-request)

### How do you make asynchronous HTTP request?

You can make an asynchronous HTTP request using `XMLHttpRequest` with `open()` and `send()` methods, and setting the `async` parameter to `true`.

Example:

```javascript
const xhr = new XMLHttpRequest();
xhr.open('GET', 'https://api.example.com', true);
xhr.send();
xhr.onload = function() {
  console.log(xhr.responseText);
};
```

**Tags**: basic, JavaScript, HTTP requests

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457281321589656864](https://www.tiktok.com/@jsmentoring/photo/7457281321589656864)
