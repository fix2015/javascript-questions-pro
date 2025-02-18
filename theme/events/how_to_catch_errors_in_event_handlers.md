## [How to catch errors in event handlers](#how-to-catch-errors-in-event-handlers)

### How to catch errors in event handlers

Wrap event handler code in a try/catch block to ensure errors do not crash the application.

```javascript
document.getElementById('myButton').addEventListener('click', () => {
  try {
    // Code that might throw an error
    performAction();
  } catch (error) {
    console.error('Error during click event:', error);
  }
});
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Error Handling](./theme/error_handling), [Events](./theme/events)


