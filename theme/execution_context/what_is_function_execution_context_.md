## [What is function execution context?](#what-is-function-execution-context)

### What is function execution context?

A function execution context is created when a function is invoked. It contains:

1. **`this` Binding**:
   - Depends on how the function is called.

2. **Scope Chain**:
   - Includes variables from the function's scope and its outer lexical environments.

3. **Variable Environment**:
   - Stores function variables and parameters.

Example:

```javascript
function example() {
  var a = 10; // Stored in variable environment
  console.log(this); // Depends on invocation
}
example();
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Execution Context](./theme/execution_context)


