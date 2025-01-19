## [What are javascript accessors](#what-are-javascript-accessors)

### What are JavaScript accessors?

Accessors are methods that allow you to get or set the value of an object's property. In JavaScript, accessors are usually implemented using `get` and `set` methods.

Example:

```javascript
const person = {
  firstName: 'John',
  lastName: 'Doe',
  get fullName() { return this.firstName + ' ' + this.lastName; },
  set fullName(name) { const parts = name.split(' '); this.firstName = parts[0]; this.lastName = parts[1]; }
};
console.log(person.fullName); // 'John Doe'
person.fullName = 'Jane Smith';
console.log(person.firstName); // 'Jane'
```

**Tags**: basic, JavaScript, objects


