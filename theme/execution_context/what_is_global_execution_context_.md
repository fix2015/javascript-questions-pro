## [What is global execution context?](#what-is-global-execution-context)

### What is global execution context?

The global execution context is the default context in which JavaScript code runs. It is created when a JavaScript file is executed and contains:

1. **Global Object**:
   - In browsers, this is the `window` object.

2. **`this` Keyword**:
   - Refers to the global object in non-strict mode.

3. **Global Variables and Functions**:
   - All declared variables and functions at the top level.

Example:

```javascript
console.log(this); // window in browsers
var a = 10; // Part of global execution context
```

**Tags**: intermediate, JavaScript, Execution Context


