## [How to use await outside of async function prior to ES2022?](#how-to-use-await-outside-of-async-function-prior-to-es2022)

### How to use await outside of async function prior to ES2022?

Before ES2022, `await` could only be used inside `async` functions. To achieve similar behavior outside of `async` functions, you could use:

1. **Immediately Invoked Async Function Expression (IIAFE):**
   ```javascript
   (async () => {
     const result = await fetch('https://api.example.com');
     console.log(result);
   })();
   ```

2. **Promise Handling with `.then()`:**
   ```javascript
   fetch('https://api.example.com')
     .then(response => response.json())
     .then(data => console.log(data));
   ```

With ES2022, `await` can be used in top-level code in modules.

**Tags**: advanced, JavaScript, Asynchronous Programming


