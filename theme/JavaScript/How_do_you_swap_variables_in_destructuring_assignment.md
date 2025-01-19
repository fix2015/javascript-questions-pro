## [How do you swap variables in destructuring assignment](#how-do-you-swap-variables-in-destructuring-assignment)

### How do you swap variables in destructuring assignment?

You can swap the values of two variables using destructuring assignment. This eliminates the need for a temporary variable.

Example:

```javascript
let a = 1, b = 2;
[a, b] = [b, a];
console.log(a, b);  // Output: 2 1
```

**Tags**: intermediate, JavaScript, Destructuring


