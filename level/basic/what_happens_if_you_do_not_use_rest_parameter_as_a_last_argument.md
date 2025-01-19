## [What happens if you do not use rest parameter as a last argument](#what-happens-if-you-do-not-use-rest-parameter-as-a-last-argument)

### What happens if you do not use rest parameter as a last argument?

The rest parameter must always be the last argument in a function. If it is not, JavaScript will throw a syntax error.

Example:

```javascript
function myFunction(a, ...rest, b) { // SyntaxError
}
```

**Tags**: basic, JavaScript, functions


