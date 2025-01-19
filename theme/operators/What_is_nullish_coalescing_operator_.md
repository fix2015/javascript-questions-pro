## [What is nullish coalescing operator (??)?](#what-is-nullish-coalescing-operator-)

### What is nullish coalescing operator (??)?

The `??` operator returns the right-hand operand if the left-hand operand is `null` or `undefined`. It is useful for providing default values.

Example:

```javascript
const value = null;
console.log(value ?? 'default'); // Output: 'default'

const number = 0;
console.log(number ?? 42); // Output: 0
```

**Tags**: basic, JavaScript, Operators


