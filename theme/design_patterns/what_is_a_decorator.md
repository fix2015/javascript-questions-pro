## [What is a decorator](#what-is-a-decorator)

### What is a decorator?

A decorator is a function that takes another function or method and adds additional functionality to it without modifying the original function. Decorators are commonly used in JavaScript to modify or enhance behavior in a reusable way.

Example:

```javascript
function log(target, key, descriptor) {
  const original = descriptor.value;
  descriptor.value = function(...args) {
    console.log('Calling ' + key);
    return original.apply(this, args);
  };
  return descriptor;
}
class MyClass {
  @log
  myMethod() {
    console.log('Method executed');
  }
}
const obj = new MyClass();
obj.myMethod(); // Logs: 'Calling myMethod' and 'Method executed'
```

**Tags**: basic, JavaScript, design patterns


