## [What is the purpose of uneval](#what-is-the-purpose-of-uneval)

### What is the purpose of uneval?

`uneval()` was used to return a string representation of an object or expression, similar to how `eval()` works. However, `uneval()` is deprecated and not supported in all environments.

Example:

```javascript
const obj = { name: 'John' };
console.log(uneval(obj)); // '({ name: "John" })'
```

**Tags**: basic, JavaScript, eval


