## [What are the advantages of Getters and Setters](#what-are-the-advantages-of-getters-and-setters)

### What are the advantages of Getters and Setters?

Getters and setters provide a controlled way to access and modify an object's properties. They allow you to define custom logic for setting or getting values and can help in encapsulating the internal state.

Example:

```javascript
const person = {
  _name: 'John',
  get name() { return this._name; },
  set name(value) { this._name = value.toUpperCase(); }
};
person.name = 'Jane';
console.log(person.name); // 'JANE'
```

**Tags**: basic, JavaScript, objects


