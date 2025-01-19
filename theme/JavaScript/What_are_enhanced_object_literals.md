## [What are enhanced object literals](#what-are-enhanced-object-literals)

### What are enhanced object literals?

Enhanced object literals simplify the creation of objects by allowing shorthand for property names and method definitions, as well as the ability to compute property names.

Example:

```javascript
let name = 'John';
let person = {
  name,
  greet() {
    console.log('Hello, ' + this.name);
  }
};
person.greet();  // Output: Hello, John
```

**Tags**: intermediate, JavaScript, Objects


