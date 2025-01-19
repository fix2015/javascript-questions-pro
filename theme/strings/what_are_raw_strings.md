## [What are raw strings](#what-are-raw-strings)

### What are raw strings?

Raw strings in JavaScript are used to access the raw string literals from template literals without escaping special characters like `
` or `	`.

Example:

```javascript
let rawStr = String.raw`Hello
World`; 
console.log(rawStr);  // Output: Hello\nWorld
```

**Tags**: advanced, JavaScript, Strings


