## [What is call stack](#what-is-call-stack)

### What is a call stack?

The call stack is a stack data structure that stores information about the active execution context of a program. When a function is called, it is added to the stack, and when it finishes executing, it is removed from the stack.

Example:

```javascript
function a() {
  b();
}
function b() {
  console.log('Hello');
}
a();
// Call stack will be: [a(), b()]
```

**Tags**: basic, JavaScript, execution context


