## [What are dynamic imports](#what-are-dynamic-imports)

### What are dynamic imports?

Dynamic imports allow you to load modules at runtime, rather than at the start of the script. This is useful for code splitting and loading modules on demand.

Example:

```javascript
import('module').then(module => {
  module.someFunction();
});
```

**Tags**: advanced, JavaScript, Modules


