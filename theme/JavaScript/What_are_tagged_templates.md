## [What are tagged templates](#what-are-tagged-templates)

### What are tagged templates?

Tagged templates allow you to parse a template literal with a function. The function is called with the string literals and interpolated expressions as arguments.

Example:

```javascript
function tag(strings, ...values) {
  console.log(strings, values);
}
let name = 'John';
tag`Hello, ${name}!`;  // Output: ['Hello, ', '!'] ['John']
```

**Tags**: advanced, JavaScript, Strings


