## [What are nesting templates](#what-are-nesting-templates)

### What are nesting templates?

Nesting templates allows you to embed template literals inside another template literal. This is useful for constructing more complex strings with dynamic content.

Example:

```javascript
let name = 'John';
let message = `Hello, ${`Mr. ${name}`}!`;
console.log(message);  // Output: Hello, Mr. John!
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Strings](./theme/strings)


