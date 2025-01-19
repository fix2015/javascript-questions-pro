## [What is the purpose of Error object](#what-is-the-purpose-of-error-object)

### What is the purpose of Error object?

The `Error` object in JavaScript is used to represent runtime errors in the application. It provides a stack trace and error message, helping developers diagnose issues. You can create custom error objects by extending the `Error` class.

Example:

```javascript
try {
  throw new Error('Something went wrong');
} catch (e) {
  console.log(e.message);  // Output: Something went wrong
}
```

**Tags**: basic, JavaScript, Error Handling


