## [What are the various statements in error handling](#what-are-the-various-statements-in-error-handling)

### What are the various statements in error handling?

In JavaScript, the main statements used for error handling are:

- `try` – Used to wrap the code that may throw an error.
- `catch` – Used to handle errors that occur in the `try` block.
- `finally` – A block of code that runs after `try` and `catch`, regardless of whether an error was thrown.

Example:

```javascript
try {
  throw new Error('Something went wrong');
} catch (e) {
  console.log(e.message);
} finally {
  console.log('This will always run');
}
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [errors](./theme/errors)


