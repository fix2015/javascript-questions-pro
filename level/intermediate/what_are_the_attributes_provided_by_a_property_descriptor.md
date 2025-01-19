## [What are the attributes provided by a property descriptor](#what-are-the-attributes-provided-by-a-property-descriptor)

### What are the attributes provided by a property descriptor?

A property descriptor in JavaScript is an object that describes the attributes of a property in an object. It contains the following attributes:

- **value**: The value of the property.
- **writable**: A boolean that indicates whether the value of the property can be changed.
- **enumerable**: A boolean that indicates whether the property shows up in a `for...in` loop or `Object.keys()`.
- **configurable**: A boolean that indicates whether the property can be deleted or modified.

Example:

```javascript
const person = { name: 'John' };
const descriptor = Object.getOwnPropertyDescriptor(person, 'name');
console.log(descriptor);
// { value: 'John', writable: true, enumerable: true, configurable: true }
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [objects](./theme/objects)


