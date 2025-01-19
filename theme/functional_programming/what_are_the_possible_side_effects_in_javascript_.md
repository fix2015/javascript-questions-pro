## [What are the possible side-effects in javascript?](#what-are-the-possible-side-effects-in-javascript)

### What are the possible side-effects in JavaScript?

Side effects occur when a function interacts with or modifies something outside its scope. Examples include:

1. Modifying global variables or objects.
2. Logging to the console.
3. Making network requests (e.g., `fetch`).
4. DOM manipulation.

Example:

```javascript
// Side Effect: Modifying a global variable
let count = 0;
function increment() {
  count++;
}

// Side Effect: Logging to the console
function logMessage(message) {
  console.log(message);
}
```

**Tags**: intermediate, JavaScript, Functional Programming


