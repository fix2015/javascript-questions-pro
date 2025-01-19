## [What is the difference between get and defineProperty](#what-is-the-difference-between-get-and-defineproperty)

### What is the difference between get and defineProperty?

- `get` is used to define a getter method that returns the value of a property when accessed.
- `Object.defineProperty()` allows you to define or modify a property directly on an object, including setting getters, setters, or other property attributes.

Example:

```javascript
const person = {
  firstName: 'John',
  lastName: 'Doe',
  get fullName() { return this.firstName + ' ' + this.lastName; }
};
console.log(person.fullName); // 'John Doe'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


