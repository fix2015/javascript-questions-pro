## [What is collation](#what-is-collation)

### What is collation?

Collation refers to the rules for comparing and sorting strings based on locale-specific conventions. In JavaScript, the `Intl.Collator` object is used to perform locale-sensitive string comparison and sorting.

Example:

```javascript
let collator = new Intl.Collator('en', { sensitivity: 'base' });
let result = collator.compare('apple', 'banana');
console.log(result);  // Output: -1
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Internationalization](./theme/internationalization)


