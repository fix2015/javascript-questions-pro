## [How do you decode an URL](#how-do-you-decode-an-url)

### How do you decode an URL?

You can use `decodeURIComponent()` to decode a URL-encoded string back into its original format.

Example:

```javascript
const encodedURL = 'https%3A%2F%2Fexample.com%2F%3Fname%3DJohn%20Doe';
const decodedURL = decodeURIComponent(encodedURL);
console.log(decodedURL); // 'https://example.com/?name=John Doe'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [encoding](./theme/encoding)


