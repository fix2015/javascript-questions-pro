## [What are the problems with postMessage target origin as wildcard](#what-are-the-problems-with-postmessage-target-origin-as-wildcard)

### What are the problems with postMessage target origin as wildcard?

Using `*` as the `targetOrigin` in `postMessage` allows any origin to receive the message, which can expose your data to malicious actors. Always specify the exact origin to ensure secure communication.

Example:

```javascript
window.postMessage('message', '*');  // Insecure
```

**Tags**: advanced, JavaScript, Security


