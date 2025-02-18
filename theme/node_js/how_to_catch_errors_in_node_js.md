## [How to catch errors in Node.js](#how-to-catch-errors-in-nodejs)

### How to catch errors in Node.js

In Node.js, use try/catch for synchronous code and attach error listeners for asynchronous code.

```javascript
// Synchronous error handling
try {
  const data = fs.readFileSync('/path/to/file');
  console.log(data);
} catch (error) {
  console.error('Error reading file:', error);
}

// Asynchronous error handling
fs.readFile('/path/to/file', (error, data) => {
  if (error) {
    return console.error('Error reading file:', error);
  }
  console.log(data);
});
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Node.js](./theme/node_js), [Error Handling](./theme/error_handling)


