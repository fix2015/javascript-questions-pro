## [What is the difference between uneval and eval](#what-is-the-difference-between-uneval-and-eval)

### What is the difference between uneval and eval?

- `eval()` executes a string of JavaScript code as if it were a part of the script.
- `uneval()` (deprecated) was used to return a string representation of an object, similar to `JSON.stringify()`.

Example:

```javascript
const code = 'console.log("Hello")';
eval(code); // Executes code
```

**Tags**: basic, JavaScript, eval


