## [How do get query string values in javascript](#how-do-get-query-string-values-in-javascript)

### How do you get query string values in JavaScript?

To get query string values, you can use the `URLSearchParams` object.

```javascript
const params = new URLSearchParams(window.location.search);
console.log(params.get('id')); // Gets the value of the 'id' parameter
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [web navigation](./theme/web_navigation)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7455462347759471905](https://www.tiktok.com/@jsmentoring/photo/7455462347759471905)
