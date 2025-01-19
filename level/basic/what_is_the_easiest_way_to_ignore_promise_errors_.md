## [What is the easiest way to ignore promise errors?](#what-is-the-easiest-way-to-ignore-promise-errors)

### What is the easiest way to ignore promise errors?

To ignore promise errors, you can attach an empty `catch` block to the promise chain:

```javascript
fetch('invalid-url')
  .then(response => response.json())
  .catch(() => {}); // Errors are ignored here
```

Alternatively, use `try...catch` in an `async` function and leave the `catch` block empty:

```javascript
async function fetchData() {
  try {
    const response = await fetch('invalid-url');
  } catch {}
}
```

**Tags**: basic, JavaScript, Promises


