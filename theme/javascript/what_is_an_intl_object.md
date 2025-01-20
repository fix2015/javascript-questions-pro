## [What is an Intl object](#what-is-an-intl-object)

### What is an Intl object?

The `Intl` object in JavaScript provides functionality for internationalization, including methods for formatting numbers, dates, and currencies, and for comparing strings according to a specific locale.

Example:

```javascript
const number = 123456.789;
const formatter = new Intl.NumberFormat('en-US');
console.log(formatter.format(number)); // '123,456.789'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [internationalization](./theme/internationalization)


