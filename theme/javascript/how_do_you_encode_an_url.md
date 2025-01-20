## [How do you encode an URL](#how-do-you-encode-an-url)

### How do you encode an URL?

You can use `encodeURIComponent()` to encode individual components of a URL, such as query parameters.

Example:

```javascript
const url = 'https://example.com/?name=John Doe';
const encodedURL = encodeURIComponent(url);
console.log(encodedURL); // 'https%3A%2F%2Fexample.com%2F%3Fname%3DJohn%20Doe'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [encoding](./theme/encoding)


