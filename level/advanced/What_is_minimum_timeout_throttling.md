## [What is minimum timeout throttling](#what-is-minimum-timeout-throttling)

### What is minimum timeout throttling?

Minimum timeout throttling refers to the browser's behavior of enforcing a minimum delay for `setTimeout` and `setInterval` calls. This is done to avoid excessive resource consumption, especially in high-frequency scenarios like animations or polling.

For example, in modern browsers, the minimum delay is typically 4ms for background tabs and 0ms for the active tab.

```javascript
setTimeout(() => console.log('Executed after delay'), 0);
```

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Performance](./theme/performance)


