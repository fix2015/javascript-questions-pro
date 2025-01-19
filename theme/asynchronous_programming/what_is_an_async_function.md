## [What is an async function](#what-is-an-async-function)

### What is an async function?

An `async` function is a function that always returns a `Promise`. It allows you to write asynchronous code using the `await` keyword, which pauses the execution until the `Promise` resolves or rejects.

Example:

```javascript
async function fetchData() {
  let response = await fetch('https://api.example.com');
  let data = await response.json();
  console.log(data);
}
fetchData();
```

**Tags**: basic, JavaScript, Asynchronous Programming


