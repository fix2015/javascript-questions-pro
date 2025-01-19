## [What is the difference between shim and polyfill](#what-is-the-difference-between-shim-and-polyfill)

### What is the difference between shim and polyfill?

- **Shim**: A shim is a piece of code that provides functionality that is not natively supported in certain environments. It can add support for missing features, but does not necessarily match the specification exactly.

- **Polyfill**: A polyfill is a more complete implementation of a feature that mimics the behavior of a native feature. It aims to fill in the gaps where the feature is not supported by older browsers or environments.

Example of a polyfill for `Array.prototype.includes`:

```javascript
if (!Array.prototype.includes) {
  Array.prototype.includes = function(value) {
    return this.indexOf(value) !== -1;
  };
}
```

**Tags**: intermediate, JavaScript, Compatibility


