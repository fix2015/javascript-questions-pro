## [What are the list of cases error thrown from non-strict mode to strict mode](#what-are-the-list-of-cases-error-thrown-from-non-strict-mode-to-strict-mode)

### What are the list of cases error thrown from non-strict mode to strict mode?

In strict mode, JavaScript imposes stricter parsing and error handling. Some common errors that occur when switching from non-strict to strict mode include:
- Assignment to undeclared variables
- Assigning to read-only properties
- Deleting undeletable properties

Example:

```javascript
'use strict';
undeclaredVar = 10;  // Throws ReferenceError
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Strict Mode](./theme/strict_mode)


