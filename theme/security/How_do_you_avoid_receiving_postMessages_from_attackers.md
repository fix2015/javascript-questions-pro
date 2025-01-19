## [How do you avoid receiving postMessages from attackers](#how-do-you-avoid-receiving-postmessages-from-attackers)

### How do you avoid receiving postMessages from attackers?

To prevent receiving messages from attackers, always validate the `origin` property of the message and ensure it matches the trusted source. You can also check the message's content for additional security.

Example:

```javascript
window.addEventListener('message', (event) => {
  if (event.origin !== 'https://trusted.com') {
    return;
  }
  // Process message
});
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Security](./theme/security)


