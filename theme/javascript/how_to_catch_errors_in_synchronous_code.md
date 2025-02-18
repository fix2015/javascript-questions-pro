## [How to catch errors in synchronous code](#how-to-catch-errors-in-synchronous-code)

### How to catch errors in synchronous code

For synchronous operations, use a try/catch block to handle errors.

```javascript
try {
  const result = riskyOperation();
  console.log(result);
} catch (error) {
  console.error('Caught an error:', error);
}
```

**Tags**: [beginner](./level/beginner), [JavaScript](./theme/javascript), [Error Handling](./theme/error_handling)


