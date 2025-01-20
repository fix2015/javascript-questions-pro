## [What is AJAX](#what-is-ajax)

### What is AJAX?

AJAX (Asynchronous JavaScript and XML) is a technique for creating dynamic web pages. It allows web pages to update asynchronously by exchanging small amounts of data with the server behind the scenes.

Example using `fetch`:

```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data));
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [AJAX](./theme/ajax)


