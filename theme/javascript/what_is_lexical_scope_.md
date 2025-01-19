## [What is Lexical Scope?](#what-is-lexical-scope)

### What is Lexical Scope?

Lexical scope refers to the scope determined by the physical structure of the code. It is defined at compile time and based on where variables and functions are declared.

#### Key Points:
1. **Inner Functions:**
   - Inner functions can access variables declared in their outer scope.

2. **Compile-Time Binding:**
   - Scope is determined when the code is written, not during execution.

Example:
```javascript
function outer() {
  const outerVar = 'I am outer';

  function inner() {
    console.log(outerVar); // Accessible due to lexical scope.
  }

  inner();
}

outer();
```

**Tags**: basic, JavaScript, Scope


