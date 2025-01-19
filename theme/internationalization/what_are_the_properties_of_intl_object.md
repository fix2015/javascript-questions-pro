## [What are the properties of Intl object](#what-are-the-properties-of-intl-object)

### What are the properties of the Intl object?

The `Intl` object in JavaScript provides several properties and methods to help with internationalization. Some of the main properties include:

- `Intl.NumberFormat`
- `Intl.DateTimeFormat`
- `Intl.Collator`
- `Intl.ListFormat`
- `Intl.RelativeTimeFormat`

These objects allow you to format numbers, dates, and compare strings based on different locales.

Example:

```javascript
const formatter = new Intl.NumberFormat('en-US', { style: 'currency', currency: 'USD' });
console.log(formatter.format(1000)); // '$1,000.00'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [internationalization](./theme/internationalization)


