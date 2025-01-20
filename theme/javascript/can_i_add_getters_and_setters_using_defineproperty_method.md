## [Can I add getters and setters using defineProperty method](#can-i-add-getters-and-setters-using-defineproperty-method)

### Can I add getters and setters using defineProperty method?

Yes, you can add getters and setters using `Object.defineProperty()`. This allows you to define custom getter and setter methods for specific properties.

Example:

```javascript
const person = {};
Object.defineProperty(person, 'name', {
  get() { return this._name; },
  set(value) { this._name = value.toUpperCase(); }
});
person.name = 'John';
console.log(person.name); // 'JOHN'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


