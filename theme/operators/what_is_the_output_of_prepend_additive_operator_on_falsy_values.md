## [What is the output of prepend additive operator on falsy values](#what-is-the-output-of-prepend-additive-operator-on-falsy-values)

### What is the output of prepend additive operator on falsy values?

The `+` operator is used to convert values to strings. When you use it with falsy values like `false`, `0`, `null`, `undefined`, or `NaN`, the result will be their string representation.

Example:

```javascript
console.log(+false);  // Output: 0
console.log(+0);  // Output: 0
console.log(+null);  // Output: 0
console.log(+undefined);  // Output: NaN
console.log(+NaN);  // Output: NaN
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Operators](./theme/operators)


