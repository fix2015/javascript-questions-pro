## [What are the function parameter rules](#what-are-the-function-parameter-rules)

### What are the function parameter rules?

- Function parameters are the variables listed in a function's declaration.
- JavaScript functions can have default parameters.
- Parameters are passed in the order they are listed.
- A function can accept any number of arguments, but the excess arguments will be ignored unless using the `...rest` parameter.

Example:

```javascript
function greet(name = 'Guest') {
  console.log('Hello, ' + name);
}
greet(); // 'Hello, Guest'
greet('John'); // 'Hello, John'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [functions](./theme/functions)


