## [What is an environment record?](#what-is-an-environment-record)

### What is an environment record?

An environment record is an internal data structure that holds variables and function declarations in a particular scope. It is part of the execution context and includes:

1. **Declarative Environment Record**:
   - Stores variables and functions declared with `var`, `let`, and `const`.

2. **Object Environment Record**:
   - Stores bindings for global objects or `with` statements.

Example:

```javascript
function example() {
  let a = 10; // Stored in Declarative Environment Record
  var b = 20; // Stored in Declarative Environment Record
}
```

**Tags**: advanced, JavaScript, Execution Context


