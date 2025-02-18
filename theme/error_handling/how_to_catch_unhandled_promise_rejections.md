## [How to catch unhandled promise rejections](#how-to-catch-unhandled-rejections)

### How to catch unhandled promise rejections

Listen for unhandled promise rejections to prevent unexpected application crashes.

```javascript
process.on('unhandledRejection', (reason, promise) => {
  console.error('Unhandled Rejection at:', promise, 'reason:', reason);
});

// Example of an unhandled rejection
Promise.reject(new Error('Unhandled error'));
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Promises](./theme/promises), [Error Handling](./theme/error_handling)


