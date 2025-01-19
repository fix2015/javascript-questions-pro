## [Is postMessages synchronous](#is-postmessages-synchronous)

### Is postMessages synchronous?

The `postMessage` API is asynchronous. The message is posted to the message queue and handled later, allowing the rest of the script to continue executing without blocking.

Example:

```javascript
window.postMessage('message', 'https://example.com');
console.log('Message sent');  // Output: Message sent
```

**Tags**: intermediate, JavaScript, Web APIs


