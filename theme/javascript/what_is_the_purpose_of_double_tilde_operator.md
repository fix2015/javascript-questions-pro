## [What is the purpose of double tilde operator](#what-is-the-purpose-of-double-tilde-operator)

### What is the purpose of double tilde operator?

The double tilde (`~~`) is a shorthand for converting a number to an integer by applying a bitwise NOT operation twice. It works by discarding the decimal part of the number, effectively performing a floor operation for positive numbers and ceiling for negative numbers.

Example:

```javascript
let num = 4.7;
console.log(~~num);  // Output: 4
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Operators](./theme/operators)


