## [How do you determine two values same or not using object](#how-do-you-determine-two-values-same-or-not-using-object)

### How do you determine two values same or not using object?

You can use `Object.is()` to determine if two values are the same. It checks both values for equality, including `NaN` and `-0`.

Example:

```javascript
console.log(Object.is(5, 5)); // true
console.log(Object.is(5, '5')); // false
console.log(Object.is(NaN, NaN)); // true
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457684535661137185](https://www.tiktok.com/@jsmentoring/photo/7457684535661137185)
