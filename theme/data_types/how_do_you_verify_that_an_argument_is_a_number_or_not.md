## [How do you verify that an argument is a Number or not](#how-do-you-verify-that-an-argument-is-a-number-or-not)

### How do you verify that an argument is a Number or not?

You can verify if a value is a number by using `typeof` operator or `Number.isNaN()` method.

Example using `typeof`:

```javascript
let value = 25;
console.log(typeof value === 'number');  // Output: true
```
Example using `Number.isNaN()`:

```javascript
let value = NaN;
console.log(Number.isNaN(value));  // Output: true
```

**Tags**: basic, JavaScript, Data Types


