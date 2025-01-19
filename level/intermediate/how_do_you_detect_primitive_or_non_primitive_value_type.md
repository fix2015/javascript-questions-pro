## [How do you detect primitive or non primitive value type](#how-do-you-detect-primitive-or-non-primitive-value-type)

### How do you detect primitive or non-primitive value type?

In JavaScript, you can detect whether a value is primitive or non-primitive by using the `typeof` operator for primitives and checking for `null` or using `instanceof` for non-primitives.

- **Primitive types**: `undefined`, `null`, `boolean`, `number`, `string`, `symbol`, `bigint`
- **Non-primitive types**: `object`, `array`, `function`

Example:

```javascript
let value = 42;
console.log(typeof value);  // Output: 'number'
let obj = {};
console.log(typeof obj);  // Output: 'object'
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Data Types](./theme/data_types)


