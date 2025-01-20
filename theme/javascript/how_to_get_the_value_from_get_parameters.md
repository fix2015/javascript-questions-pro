## [How to get the value from get parameters](#how-to-get-the-value-from-get-parameters)

### How to get the value from GET parameters?

You can get the value of a GET parameter in the URL using `URLSearchParams`.

Example:

```javascript
const urlParams = new URLSearchParams(window.location.search);
const value = urlParams.get('param');
console.log(value); // Logs the value of 'param' from the URL
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [URL manipulation](./theme/url_manipulation)


