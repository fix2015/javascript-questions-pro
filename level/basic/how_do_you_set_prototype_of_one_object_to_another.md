## [How do you set prototype of one object to another](#how-do-you-set-prototype-of-one-object-to-another)

### How do you set prototype of one object to another?

You can set the prototype of one object to another using the `Object.setPrototypeOf()` method. This method allows you to change the prototype chain of an object.

Example:

```javascript
const animal = { speak: function() { console.log('Animal speaks'); } };
const dog = {};
Object.setPrototypeOf(dog, animal);
dog.speak(); // Animal speaks
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [objects](./theme/objects)


