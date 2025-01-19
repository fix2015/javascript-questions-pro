## [How do you get property descriptors of an object](#how-do-you-get-property-descriptors-of-an-object)

### How do you get property descriptors of an object?

In JavaScript, you can use `Object.getOwnPropertyDescriptor()` to get the descriptor of a specific property on an object. This descriptor contains details about the property such as whether it's writable, enumerable, or configurable.

Example:

```javascript
const person = { name: 'John' };
const descriptor = Object.getOwnPropertyDescriptor(person, 'name');
console.log(descriptor);
// { value: 'John', writable: true, enumerable: true, configurable: true }
```

**Tags**: intermediate, JavaScript, objects


