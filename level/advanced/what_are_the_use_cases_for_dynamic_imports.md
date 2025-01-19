## [What are the use cases for dynamic imports](#what-are-the-use-cases-for-dynamic-imports)

### What are the use cases for dynamic imports?

Dynamic imports are useful for lazy loading, where modules are loaded only when they are needed, improving the initial load time of a web application. They are also helpful in code splitting and on-demand loading of specific features or components.

Example:

```javascript
if (userWantsFeature) {
  import('./feature.js').then(feature => {
    feature.init();
  });
}
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Modules](./theme/modules)


