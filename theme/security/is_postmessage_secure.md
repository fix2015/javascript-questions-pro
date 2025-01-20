## [Is PostMessage secure](#is-postmessage-secure)

### Is PostMessage secure?

The `postMessage` API is secure if used correctly. However, it can be vulnerable if not properly handled, as it can expose data to unintended origins. It is crucial to validate the `targetOrigin` and avoid using wildcards to ensure secure messaging.

Example:

```javascript
window.postMessage('message', 'https://example.com');
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Security](./theme/security)


