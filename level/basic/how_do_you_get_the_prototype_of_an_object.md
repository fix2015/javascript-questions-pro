## [How do you get the prototype of an object](#how-do-you-get-the-prototype-of-an-object)

### How do you get the prototype of an object?

In JavaScript, you can get the prototype of an object using the `Object.getPrototypeOf()` method. This method returns the prototype (i.e., the internal `[[Prototype]]` property) of the specified object.

Example:

```javascript
const person = { name: 'John' };
const prototype = Object.getPrototypeOf(person);
console.log(prototype); // Outputs the prototype of the object
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


