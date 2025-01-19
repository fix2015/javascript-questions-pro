## [What are default parameters](#what-are-default-parameters)

### What are default parameters?

Default parameters allow you to set default values for function parameters if no argument is provided when calling the function. This helps in avoiding `undefined` values.

Example:

```javascript
function greet(name = 'Guest') {
  console.log('Hello, ' + name);
}
greet();  // Output: Hello, Guest
greet('John');  // Output: Hello, John
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Functions](./theme/functions)


