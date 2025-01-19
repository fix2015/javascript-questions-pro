## [What is the difference between function and class declarations](#what-is-the-difference-between-function-and-class-declarations)

### What is the difference between function and class declarations?

- **Function Declarations**:
  - Can be hoisted, meaning they can be used before they are declared in the code.
  - Syntax: `function functionName() {}`

- **Class Declarations**:
  - Cannot be hoisted, so they must be declared before use.
  - Syntax: `class ClassName {}`

Example:

```javascript
console.log(foo()); // Works because of hoisting
function foo() { return 'Hello'; }

// console.log(new Bar()); // Error: Bar is not defined
class Bar { constructor() { console.log('Bar created'); } }
```

**Tags**: intermediate, JavaScript, Declarations


