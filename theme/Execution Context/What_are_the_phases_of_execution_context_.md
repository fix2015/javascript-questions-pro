## [What are the phases of execution context?](#what-are-the-phases-of-execution-context)

### What are the phases of execution context?

1. **Creation Phase:**
   - Memory is allocated for variables and functions.
   - Variables are initialized with `undefined`.
   - Functions are stored as-is.

2. **Execution Phase:**
   - Code is executed line by line.
   - Variables are assigned actual values.

Example:

```javascript
function test() {
  console.log(a); // undefined (creation phase)
  var a = 10;
  console.log(a); // 10 (execution phase)
}

test();
```

**Tags**: intermediate, JavaScript, Execution Context


